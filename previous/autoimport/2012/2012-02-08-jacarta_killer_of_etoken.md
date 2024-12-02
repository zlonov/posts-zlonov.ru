---
layout: zlonov/old_post
title: JaCarta - убийца eToken?
date: 2012-02-08 05:51
author: admin
category: autoimport
tags: [Aladdin, SafeNet, бизнес, информационная безопасность, сертификация, токен]
---
Всегда с интересом читаю пресс-релизы, касающиеся вопросов, в которых я в силу своего рода занятий немного разбираюсь. Вдумчивое изучение текстов, вышедших из-под пера PR-менеджеров, и дальнейшее активное "гугление" порой дают неожиданные результаты.

Сегодня применим этот метод к новости о том, что "<a href="http://safe.cnews.ru/news/line/index.shtml?2012/02/06/476242"><i>Встраиваемый модуль безопасности TSM от «Аладдин Р.Д.» сертифицирован ФСТЭК</i></a>".

Текст содержит интересный пассаж о (внимание!) трёхфакторной аутентификации:
<blockquote><i>TSM обеспечивает защиту от несанкционированного доступа с помощью трехфакторной аутентификации, осуществляемой по наличию аппаратного идентификатора (eToken, iButton), присутствию на нем специального логического идентификатора и знанию пользователем PIN-кода доступа.</i>
Оставим, впрочем, на совести автора тот факт, что при краже аппаратного идентификатора злоумышленник заодно получает и записанный на нём логический идентификатор, что, вообще говоря, не позволяет говорить о двух разных факторах.

[box type="info" style="rounded"]UPD. 24.07.2012 На сайте "трехфакторной" поменяли на "двухфакторной", но перечисляется по-прежнему три сущности.[/box]

Меня больше заинтересовало, почему пресс-релиз не совместный с Kraftway (ведь сертифицированный модуль работает только на их компьютерах)? Быть может, они выпустили отдельный пресс-релиз?

В <a href="http://www.kraftway.ru/press/">пресс-центре</a> на сайте Kraftway данной новости обнаружено не было, но упоминание самого модуля есть в описании моделей с его поддержкой (например, <a href="http://www.kraftway.ru/products/product.php?SECTION_ID=261&amp;PRODUCT_ID=1938">Kraftway Credo KC38</a> и <a href="http://www.kraftway.ru/products/product.php?SECTION_ID=550&amp;PRODUCT_ID=2141">Kraftway Credo VV18</a>). Как оказалось, поддержка данных модулей реализована <a href="http://www.kraftway.ru/press/release/?ID=396450&amp;phrase_id=591636">уже достаточно давно</a>, а сотрудничество в этом направлении компании и вовсе <a href="http://www.kraftway.ru/press/release/?ID=335854&amp;phrase_id=591636">ведут с конца 2010 года</a>.

Есть на сайте Kraftway и <a href="http://www.kraftway.ru/upload/iblock/c57/aladdin-tsm.jpg">сертификат на TSM</a>, но особый интерес вызывает, конечно же, <a href="http://www.kraftway.ru/clean/info.php?SECTION_ID=2258&amp;print=Y">подробное описание характеристик и функционала TSM</a>, взятое, судя по всему, из технический условий или паспорта изделия. Буквально в самом начале видим:
<blockquote><i>TSM взаимодействует с идентифицирующими устройствами (ИУ), в качестве которых выступают ключи eToken или JaCarta в форм-факторе USB-ключа или смарт-карты. </i><b>(См. Update в конце поста.)</b>
Ключи <b>eToken </b>- понятное дело, но, позвольте, а что за зверь такой <b>JaCarta</b>? В пресс-релизе Аладдин Р.Д. такое не упоминается. Google и Яндекс по запросу "jacarta" выдают явно не относящиеся к делу ссылки, да ещё и предлагают исправить написание на "jakarta", что уж совсем не из нашей оперы.

"Помощь пришла откуда не ждали" - упоминание JaCarta <a href="http://www.aladdin-rd.ru/search/?q=jacarta">нашлось на сайте Аладдин Р.Д.</a> И пусть ссылка не открывается, нам теперь понятно, что искать дальше.

<a href="/assets/uploads/JaCarta_._..png"><img class="aligncenter size-medium wp-image-4270" alt="JaCarta_._." src="/assets/uploads/JaCarta_._.-300x212.png" width="300" height="212" /></a>

Опущу лишние подробности и тонкости поиска, перейдя сразу к фактам.
<ul>
	<li>Домен jacarta.ru <a href="http://www.ableo.ru/jacarta.ru">был зарегистрирован</a> 04 апреля 2011 года на "Aladdin Software Security R.D. Ltd.", читай - ЗАО "Аладдин Р.Д."</li>
	<li>На официальном сайте Аладдин Р.Д. действительно присутствует (присутствовал) раздел "/catalog/jacarta/", но его <a href="http://www.aladdin-rd.ru/robots.txt">поисковая индексация запрещена</a>.</li>
	<li>Сайт <a href="http://jacarta.ru/">jacarta.ru</a> (набирать без www) наполнен смесью контента с официального сайта Аладдин Р.Д. и содержит упоминание некоей ООО "Алеро-Сервис" <a href="http://jacarta.ru/contacts/">с контактами самого</a> Аладдин Р.Д.</li>
	<li>У Алеро-Сервис <a href="http://aleros.ru/">есть свой сайт</a> (заполненный пока всё тем же промежуточным контентом) и даже логотип.</li>
	<li>ООО "Алеро-Сервис" 06 октября 2011 года получило <i>Лицензию на деятельность по разработке и (или) производству средств защиты конфиденциальной информации</i>, что отражено в соответствующем <a href="http://clck.yandex.ru/redir/AiuY0DBWFJ4ePaEse6rgeAjgs2pI3DW99KUdgowt9Xs7e_DEZHQ5W7tN_TIWqbl_p4cZYDQ4E8c-OJa_F7uryv0qvkuovT5lL47FmD5qmx8kSvngSDEUuLmJXinQt-zRFl4YDD8pE6m3SSWdSgyvbv_9LHhUBWYiKeTBWOsOgnnlava7A_jElw?data=UlNrNmk5WktYejR0eWJFYk1LdmtxaUpCYWxISlBzYW5XdzRhUnVQTEltaG12RTB2WExvZGhDZnhyb0VseXhMaVJjSGdoeXVCeXYxcTk2ZndXU3dVLXpyMGl6REZTVHE4VW1RYmdMQ1pUbmRZSS01bVBLSmdIaVRQc3JJLVZvdkE2cnhjOU5sWnlvUC14OVZmSzlZa1l3&amp;b64e=2&amp;sign=388727a65f37a7025e232f84b0193cd0&amp;keyno=8&amp;l10n=ru&amp;mc=5329&amp;i=7">реестре ФСТЭК</a>.</li>
	<li>Сама компания <a href="http://www.rusprofile.ru/id/3382687">зарегистрирована ещё 03 августа 2007 года</a> и её генеральным директором является Груздев Сергей Львович (его полный тёзка является генеральным директором ЗАО "Аладдин Р.Д.")</li>
	<li>У компаний ООО "Алеро-Сервис" и ЗАО "<a href="http://docsystem.ru/">Документальные Системы</a>" есть <a href="http://globalstat.ru/company/4026510">дочернее предприятие</a> ООО "СИС" (<a href="http://www.c-i-s.ru/">Сертифицированные информационные системы</a>).</li>
	<li>[box type="info" style="rounded"]UPD. 14.02.2014 Об актуальном способе получения информации о факте аффилированности этих компаний рассказал по просьбе читателя в посте <a href="https://zlonov.ru/2014/02/read-between-the-address-bars-or-how-to-know-the-founders-of-the-legal-entity">Читаем между адресных строк или Как узнать учредителей юридического лица</a>.[/box]</li>
</ul>
<div><a href="/assets/uploads/Alero_Logo.jpg"><img class="aligncenter size-full wp-image-4271" alt="Alero_Logo" src="/assets/uploads/Alero_Logo.jpg" width="229" height="85" /></a></div>
<span>Что же получается? В свете <a href="https://zlonov.ru/2010/11/tolko-faktyi-i-odin-sluh/">непростой ситуациии</a> в России с дистрибьюцией ключей eToken и использованием торговой марки "Aladdin" руководство Аладдин Р.Д. через ООО "Алеро-Сервис" подготовило себе запасной аэродром в виде доли в ООО "СИС" </span>с одной стороны (напомню, что именно эту компанию SafeNet, купивший бизнес eToken, <a href="http://publishernews.ru/PressRelease/PressReleaseShow.asp?id=100951">сделал российским дистрибьютором по данному направлению</a>) и разработки аналога под названием JaCarta с другой?

<span>Что ж, если это так, то ход вполне себе закономерный: кормясь от продаж eToken, инвестировать в конкурирующую разработку, прописывать её потихоньку в сертификаты, с тем, чтобы со временем получить возможность полностью переключиться на новый носитель JaCarta и убить рынок сертифицированных eToken за счёт контроля над всеми сертификатами eToken и своих связей с заказчиками и партнёрами.</span>

Возможно, конечно, что у вас сложится свой взгляд на картину происходящего, но факты остаются фактами - дело только за их интерпретацией.

Интересно, глаза кому и на чьи маленькие секреты и хитрости откроет этот пост? =)

[box type="info" style="rounded"]UPD. 09.02.2012 Данный пост, очевидно, <a href="http://www.aladdin-rd.ru/company/mediakit/photo/">прочитали</a> и сайт http://jacarta.ru более недоступен (редиректится). Предвидя такой поворот событий, сохранил пару скриншотов. Вот они:

<a href="/assets/uploads/21.png"><img class="aligncenter size-medium wp-image-4272" alt="_-2" src="/assets/uploads/21-300x144.png" width="300" height="144" /></a>
<div></div>
<div><a href="/assets/uploads/jacarta.ru_.png"><img class="aligncenter size-medium wp-image-4273" alt="_jacarta.ru" src="/assets/uploads/jacarta.ru_-300x210.png" width="300" height="210" /></a></div>
Кстати, из результатов поиска на aladdin-rd.ru убрали всякое упоминание о "jacarta", но скриншот с тем, что выдавалось ещё буквально вчера, есть выше в самом посте.

Вас такое тщательное заметание следов не наводит на мысль о верности сделанного выше предположения? [/box]

<!--?xml version="1.0" encoding="UTF-8" standalone="no"?--> [box type="info" style="rounded"]UPD. 20.02.2012 Слушайте, всё становится ещё интереснее: теперь с сайта Kraftway убрали упоминание о поддержке JaCarta в модуле TSM! Вот так всё выглядело раньше:

<a href="/assets/uploads/TSM.png"><img class="aligncenter size-medium wp-image-4274" alt="_TSM" src="/assets/uploads/TSM-300x174.png" width="300" height="174" /></a>
<div>А вот <a href="/assets/uploads/2012/02/%D0%92%D1%81%D1%82%D1%80%D0%B0%D0%B8%D0%B2%D0%B0%D0%B5%D0%BC%D1%8B%D0%B9-%D0%BC%D0%BE%D0%B4%D1%83%D0%BB%D1%8C-%D0%B1%D0%B5%D0%B7%D0%BE%D0%BF%D0%B0%D1%81%D0%BD%D0%BE%D1%81%D1%82%D0%B8-TSM.htm">здесь целиком исходный текст страницы в html-виде</a>. Кэш Яндекса пока тоже <a href="http://hghltd.yandex.net/yandbtm?text=jacarta%20kraftway&amp;url=http%3A%2F%2Fwww.kraftway.ru%2Fclean%2Finfo.php%3FSECTION_ID%3D2283%26print%3DY&amp;fmode=inject&amp;mime=html&amp;l10n=ru&amp;sign=cccaa779ac12a233ab8f356d9fc2340d&amp;keyno=0">выдаёт вариант с JaCarta</a>, но, боюсь, это временно.[/box]</div>
<div style="text-align: right;"><i><span>Изображение: http://recuerdosinventados.blogspot.com/2008/03/killer-cat-periodismo-patritico.html</span></i></div>
