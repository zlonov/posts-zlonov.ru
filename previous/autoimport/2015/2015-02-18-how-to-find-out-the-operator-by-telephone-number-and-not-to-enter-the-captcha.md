---
layout: zlonov/old_post
title: Как узнать оператора по номеру телефона (и не вводить капчу)
date: 2015-02-18 20:55
author: admin
category: autoimport
tags: [адресная строка, база данных, взлом, информационная безопасность, номер телефона, ошибка реализации, сайт, ЦНИИС]
---
После отмены "мобильного рабства" пользователи массово начали переходить от одного оператора к другому с сохранением своего телефонного номера. Уже на начало февраля таких абонентов <a href="http://nag.ru/news/newsline/26894/million-abonentov-izbavilis-ot-mobilnogo-rabstva.html" target="_blank">стало более миллиона</a> (более подробная статистика по числу переходов представлена <a href="http://www.zniis.ru/bdpn/statistics" target="_blank">на сайте ЦНИИС</a> - официального оператора базы данных перенесенных абонентских номеров на основании распоряжения Правительства РФ от 9 октября 2013г. № 1832-р).

Таким образом, со временем всё сложнее будет по коду абонента определить его сотового оператора: 903 - теперь не обязательно будет Билайн, а 926 - может и не означать Мегафон. Честно говоря, не очень представляю себе практической ценности от такого рода знаний (разве что это может быть важно при наличии в тарифном плане льготной опции при звонке на телефонные номера конкретного оператора), но, тем не менее, на сайте ЦНИИС соответствующий раздел присутствует: <a href="http://www.zniis.ru/bdpn/check" target="_blank">Узнать оператора по номеру телефона</a>.

<a href="/assets/uploads/ToKnowOperator.png"><img class="aligncenter size-full wp-image-6175" src="/assets/uploads/ToKnowOperator.png" alt="Узнать оператора по номеру телефона" width="716" height="388" /></a>

Для защиты от "роботов" данная форма запроса традиционно защищена капчей (CAPTCHA), но, как оказалось, её можно совсем просто обойти. Сейчас расскажу как именно.

Моё <a href="https://zlonov.ru/2013/05/hack-the-gartner-via-address-ba/" target="_blank">традиционное внимание к адресной строке браузера</a> было вознаграждено и в этот раз. Вот как выглядит результат на странице сайта после ввода корректной капчи:

<a href="/assets/uploads/success.png"><img class="aligncenter size-full wp-image-6176" src="/assets/uploads/success.png" alt="Успешно. Узнать оператора по номеру телефона" width="467" height="259" /></a>

Ничего необычного: указан номер, выведен оператор, а поле капчи изменено на новое... А вот адресная строка выглядит гораздо интереснее:

<a href="/assets/uploads/bar.png"><img class="aligncenter size-full wp-image-6177" src="/assets/uploads/bar.png" alt="Адресная строка. Узнать оператора по номеру телефона" width="536" height="32" /></a>

Как видно, в качестве параметров используются три переменные: <strong>num</strong>, <strong>number</strong> и <strong>r</strong>. Собственно, вполне очевидно, что <strong>num</strong> - это введённый пользователем номер телефона, оператора которого он хочет проверить.

Простые эксперименты и некоторые логические умозаключению показали, что <strong>number</strong> - это то, что пользователь указал в поле капчи, а <strong>r</strong> - специальный проверочный параметр, вычисленный заранее. Получается, что алгоритм проверки просто делает расчёт некоторого значения на основании того, что ввёл пользователь (назовём это значение <strong>r2</strong>), и сравнивает <strong>r2 </strong>с эталонным <strong>r</strong>, передавая при этом само <strong>r </strong>зачем-то в запросе.<strong> </strong>Вот такая странная реализация.

Тут можно было бы подумать, что для обхода алгоритма капчи нужно будет проводить анализ и выяснять принцип вычисления <strong>r</strong>, но всё оказалось гораздо проще: <strong>r</strong> никак не зависит от номера телефона, а вычисляется только из символов правильной капчи. На практике это означает, что если у нас есть одна пара соответствующих друг другу параметров <strong>number</strong> и <strong>r</strong>, то меня <strong>num</strong>, можно получать желаемый результат для любого другого телефонного номера.

Пара примеров. Вот например, ссылка, которая получается после правильно введённых пользователем символов капчи:

<em>http://www.zniis.ru/bdpn/check?num=<strong>9031234567</strong>&amp;number=<strong>3f52ce28</strong>&amp;r=<strong>366172</strong></em>

Здесь параметры <strong>number</strong> (то, что пользователь ввёл в поле капчи) и <strong>r</strong> (проверочное значение, которое должно получаться из number, если оно правильное) соответствуют друг другу, поэтому в качестве параметра <strong>num</strong> (проверяемый номер телефона) можно передавать всё, что угодно:

<em>http://www.zniis.ru/bdpn/check?num=<strong>9099999999</strong>&amp;number=<strong>3f52ce28</strong>&amp;r=<strong>366172</strong></em>
<em> http://www.zniis.ru/bdpn/check?num=<strong>9033333333</strong>&amp;number=<strong>3f52ce28</strong>&amp;r=<strong>366172</strong></em>
<em> http://www.zniis.ru/bdpn/check?num=<strong>9266666666</strong>&amp;number=<strong>3f52ce28</strong>&amp;r=<strong>366172</strong></em>

Не могу сказать, что это какая-то очень опасная уязвимость. Максимум, что она позволяет сделать - это написать скрипт, который выкачает целиком всю базу соответствий номеров телефонов и текущих операторов, к которым эти номера приписаны. Тем не менее,  уведомление администрации сайта на указанный в разделе Контакты адрес info@zniis.ru ещё на прошлой неделе я всё же направил.

Никакой реакции, ожидаемо, не последовало. Правда, те примеры (с парой <strong>number</strong> и <strong>r</strong>), которые были указаны в моём письме, больше не работают. Возможно, что это и есть реакция (смайл) - просто исключили пару проверенных мной <strong>number</strong> и <strong>r</strong>, а может <strong>r</strong> вычисляется каждый день заново и уже завтра примеры из этого поста тоже работать не будут, но пока не поменяется сам принцип проверки, не поменяется и принцип обхода капчи при проверке оператора по номеру телефона на сайте официального оператора базы данных перенесенных абонентских номеров на основании распоряжения Правительства РФ от 9 октября 2013г. № 1832-р.
