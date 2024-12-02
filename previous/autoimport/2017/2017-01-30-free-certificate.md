---
layout: zlonov/old_post
title: Выбор бесплатного сертификата для собственного домена
date: 2017-01-30 15:25
author: admin
category: autoimport
tags: [Firefox, Fornex, Google, HTTPS, Let's Encrypt, SSL, StartSSL, домен, информационная безопасность, сайтоведение, сертификат, хостинг]
---
В январе Google обрадовал меня как владельца сайта, что скоро отдельные страницы блога будут помечаться как небезопасные с выводом соответствующего предупреждения посетителям.

Проблема оказалась со страницами, где запрашивается пароль для доступа к квадра(н)там Гартнера (такую меру пришлось ввести <a href="https://zlonov.ru/2016/05/copyright/">после общения с Gartner в прошлом году</a>).

Давно собирался озаботиться переходом на протокол https, но вот теперь Google решил мне придать дополнительный стимул. В новостях к тому же встретил статью про аналогичный подход от Firefox: <a href="https://threatpost.ru/firefox-51-begins-warning-users-of-insecure-http-connections/20284/">Firefox начал предупреждать о HTTP</a>.

[caption id="attachment_10113" align="aligncenter" width="479"]<a href="/assets/uploads/Проблемы-с-безопасностью-на-ZLONOV.ru_.jpg"><img class="wp-image-10113" src="/assets/uploads/Проблемы-с-безопасностью-на-ZLONOV.ru_.jpg" alt="Проблемы с безопасностью на ZLONOV.ru" width="479" height="492" /></a> Проблемы с безопасностью на ZLONOV.ru[/caption]

С учётом того, что сертификат для собственного домена сейчас без проблем можно получить бесплатно, решил не откладывать задачу в долгий ящик. Первой нашлась тематическая статья на Хабре: <a href="https://habrahabr.ru/post/127643/">Получаем бесплатный SSL сертификат</a>. Сервис StartSSL, про который в ней идёт речь оказался простым и понятным, никаких проблем с регистрацией не возникло. В статье на Хабре, правда, чуть устаревшие скриншоты - интерфейс у сервиса поменялся, но всё прошло гладко. Проблема внезапно возникла уже после того, как сертификат был сгенерирован и установлен в панели управления хостингом: отдельные браузеры сообщали, что сертификат не является доверенным.

[caption id="attachment_10114" align="aligncenter" width="479"]<a href="/assets/uploads/Неверный-издатель-сертификта-StartSSL.jpg"><img class="size-full wp-image-10114" src="https://i1.wp.com/zlonov.ru/wp-content/uploads/2011/06/utchk329.jpg?fit=130%2C93&#038;ssl=1" alt="Неверный издатель сертификта StartSSL" width="130" height="93" /></a> Неверный издатель сертификта StartSSL[/caption]

[caption id="attachment_10115" align="aligncenter" width="479"]<a href="/assets/uploads/Незащищённое-подключение-с-сертификатом-StartSSL.jpg"><img class="wp-image-10115" src="/assets/uploads/Незащищённое-подключение-с-сертификатом-StartSSL.jpg" alt="Незащищённое подключение с сертификатом StartSSL" width="479" height="565" /></a> Незащищённое подключение с сертификатом StartSSL[/caption]

[caption id="attachment_10116" align="aligncenter" width="479"]<a href="/assets/uploads/Сертификат-StartSSL-аннулирован.jpg"><img class="wp-image-10116" src="/assets/uploads/Сертификат-StartSSL-аннулирован.jpg" alt="Сертификат StartSSL аннулирован" width="479" height="570" /></a> Сертификат StartSSL аннулирован[/caption]

В общем, эффект получился прямо противоположный. Оказалось, что у сервиса StartSSL действительно проблемы с доверием к их сертификатам:

<blockquote><em>Mozilla and Google decided to distrust all StartCom root certificates as of 21<sup>st</sup> of October, this situation will have an impact in the upcoming release of Firefox and Chrome in January. StartCom will provide an interim solution soon and will replace all the issued certificates from that date in case of requested. Meanwhile StartCom is updating all their systems and will generate new root CAs as requested by Mozilla to regain the trust in these browsers.
</em><a href="https://www.startssl.com/NewsDetails?date=20161103">StartCom paused the charged validation service</a>

Возможно, со временем проблему решат и сертификатами от StartSSL снова можно будет пользоваться, но пока пришлось искать другую альтернативу. Техподдержка <a href="https://fornex.com/?server=18987">моего хостинг провайдера</a> (качество работы которого хвалить не устану) предложила попробовать сертификат от бесплатного сервиса <a href="https://letsencrypt.org">Let's Encrypt</a>.

Далее, по аналогии со статьёй на Хабре, предполагалась статься со скриншотами, но в моём случае ничего делать вообще не пришлось - специалисты техподдержки настроили всё сами. Сертификат от Let's Encrypt выдаётся на три месяца, но в дальнейшем все его обновления будут опять-таки происходить без моего участия.

Собственно, такой вариант - обращение к своему хостинг-провадйеру рекомендуется и самим сервисом Let's Encrypt: <a href="https://letsencrypt.org/getting-started/">https://letsencrypt.org/getting-started/</a> Полный список провайдеров, которые уже предлагают услугу по автоматической установке бесплатного сертификата от Let's Encrypt доступен здесь: <a href="https://community.letsencrypt.org/t/web-hosting-who-support-lets-encrypt/6920">https://community.letsencrypt.org/t/web-hosting-who-support-lets-encrypt/6920</a>

[caption id="attachment_10117" align="aligncenter" width="479"]<a href="/assets/uploads/Сертификат-от-Lets-Encrypt-для-ZLONOV.ru_.jpg"><img class="wp-image-10117" src="/assets/uploads/Сертификат-от-Lets-Encrypt-для-ZLONOV.ru_.jpg" alt="Сертификат от Let's Encrypt для ZLONOV.ru" width="479" height="492" /></a> Сертификат от Let's Encrypt для ZLONOV.ru[/caption]

В общей сложности потратил на решение задачи буквально пару дней. Как тут <a href="https://zlonov.ru/2017/01/minenergo-project/">не вспомнить</a> портал <em>https://regulation.gov.ru</em>, у которого сертификат истёк больше четырёх месяцев назад? =)

<a href="/assets/uploads/Истёк-сертификат-regulation.gov_.ru_.jpg"><img class="aligncenter size-full wp-image-9971" src="/assets/uploads/Истёк-сертификат-regulation.gov_.ru_.jpg" alt="Истёк сертификат regulation.gov.ru" width="478" height="394" /></a>
