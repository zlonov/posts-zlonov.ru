---
layout: zlonov/old_post
title: Почему DLP-система не защитила банк Санкт-Петербург от утечки?
date: 2015-07-29 05:12
author: admin
category: autoimport
tags: [DLP, PR, Solar Dozor, Solar Security, банк, Дозор-Джет, ИнфоВотч, информационная безопасность, Инфосистемы Джет, утечка]
---
На прошлой неделе <a href="http://www.interfax.ru/business/455640" target="_blank">стало известно</a> о хакерской атаке на банк Санкт-Петербург, в результате которой "<em>злоумышленникам стала доступна информация о нескольких тысячах карточных счетов - ФИО, номер счета и номер карты</em>".

Атака примечательна тем, что монетизировать украденную информацию хакеры попытались сразу же - путём вымогательства 29 миллионов рублей в обмен на нераскрытие украденной информации.

Шантаж не удался, банк на сделку не согласился, так как по мнению его представителей "<em>никакой угрозы для клиентов нет</em>". Более того, и в СМИ банк, судя по всему, обратился самостоятельно, опередив злоумышленников, которые угрожали публичной оглаской.

Второй любопытный момент с этой атакой - банк выявил взлом, но не пресёк его, а <a href="http://www.fontanka.ru/2015/07/23/059/" target="_blank">перевёл в контролируемый режим</a>:
<blockquote>...нами была своевременно обнаружена нетипичная для поведения клиентов активность в информационной базе. Специалисты банка изучили ситуацию и пришли к выводу, что данные, получаемые хакерами, не являются критичными для клиентов и не могут повлечь за собой возможность проведения мошеннических операций по их счетам. В результате было принято решение сразу не блокировать их доступ к этой информации, а дождаться, когда правоохранительные органы смогут найти улики, дающие возможность задержать преступников в будущем.
Наконец, вишенку на торт истории данного взлома положили коллеги из компании ИнфоВотч, <a href="http://www.infowatch.ru/analytics/leaks_monitoring/15684" target="_blank">опубликовав на официальном сайте</a> более умеренный текст и без упоминания конкурентов, но при этом <a href="http://infowatch.livejournal.com/463272.html" target="_blank">разместив в ЖЖ</a> пост с важным пикантным добавлением:
<blockquote>Примечательно, что в банке отношение к информационной безопасности сложно назвать наплевательским. В банке <a href="http://jet.su/upload/iblock/dc8/jet584.pdf" target="_self">внедрена</a> DLP-система «Дозор-Джет» для защиты от утечек данных, отслеживаются сообщения сотрудников по электронной почте, на форумах, в соцсетях. «Мы не настолько богаты, чтобы покупать дешевые решения, - заявил Анатолий Скородумов Коммерсанту, - инвестиции в ИБ – это инвестиции в репутацию компании.
С моей лёгкой(?) руки в <a href="https://twitter.com/zlonov/status/626063112249212928" target="_blank">Twitter</a> и <a href="https://www.facebook.com/komarov.alexey/posts/812108095576273" target="_blank">Facebook</a> развернулась оживлённая дискуссия на тему того, что DLP-система не предотвратила эту утечку. Заодно были обсуждены и мои таланты в области "черного PR", но это к сути поста не относится =)

Несмотря на использованный мной довольно провокационный тезис, вырванный из контекста поста ИнфоВотч ("<em>В банке Санкт-Петербург, допустившем утечку персональных данных 300 тыс клиентов, была внедрена DLP-система Дозор-Джет</em>"), на мой взгляд, вины <a href="http://solarsecurity.ru" target="_blank">вендора</a> и <a href="http://www.jet.msk.su" target="_blank">интегратора</a> (на момент самого внедрения, как я понимаю, это было одно и то же) в случившемся нет.

Попробую объяснить почему.

Во-первых, DLP-система, как и любое средство защиты информации, не даёт 100% гарантии отсутствия утечек (продавцы, утверждающие обратное, мягко говоря, преувеличивают). Речь может идти только о снижении вероятности. Сколько утечек успешно ранее предотвратил Дозор-Джет - мы не знаем, поэтому выводы о его эффективности на основании одного случая сделать не получится.

Во-вторых, DLP-система призвана отслеживать лишь ограниченное число потенциальных каналов утечки, а не все мыслимые и немыслимые. Сокращение числа лишних каналов как раз одна из задач при внедрении DLP - в статье Коммерсанта, например, <a href="http://jet.su/upload/iblock/dc8/jet584.pdf" target="_blank">говорится</a> о контроле доступа сотрудников в Интернет с той самой целью сокращения числа каналов утечки. Каким конкретно каналом воспользовались хакеры - не известно, вполне вероятно, что его DLP как раз и не отслеживала.

В-третьих, несмотря на то, что в контролируемость самой утечки не так просто поверить, мы имеем официальное заявление банка об этом, сделанное в СМИ, так что DLP-система могла быть просто отключена самими сотрудниками банка.

Наконец, надо отметить, что противостояние внешнему взлому не является функцией DLP-системы, поэтому проникшие в сеть банка хакеры могли деактивировать DLP или, выявив её присутствие, воспользоваться какой-либо техникой обхода (для опытного специалиста вряд ли такое будет нерешаемой задачей).

Кстати, в статье Коммерсанта, на которую ссылаются коллеги из ИнфоВотч, упоминания конкретного продукта нет, но вроде бы никто из представителей Инфосистем Джет или Solar Security не отрицает факт использования именно DLP-системы Дозор-Джет (текущее название - <a href="http://solarsecurity.ru/products/solar_dozor/" target="_blank">Solar Dozor</a>).

В любом случае, дать адекватную оценку эффективности используемых в банке Санкт-Петербург средств защиты информации можно только обладая полной информацией о случившемся. Было бы здорово, если банк обнародовал результаты внутреннего расследования причин случившегося - полагаю, открытость в данном вопросе нивелировала бы хотя бы частично урон, нанесённый его репутации.

Ведь персональные данные всё-таки утекли и не очень правильно будет просто закрыть на это глаза, тут с коллегами из ИнфоВотч соглашусь.
<p style="text-align: right;"><sub><em><a href="http://planet-today.ru/media/k2/items/cache/20d6a30007c9cf7d1f34dd14baf7c807_XL.jpg?t=-2147483648" target="_blank">Изображение</a></em></sub>