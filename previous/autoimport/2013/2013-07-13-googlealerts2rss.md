---
layout: zlonov/old_post
title: Создание RSS-ленты из оповещений Google Alerts
date: 2013-07-13 19:41
author: admin
category: autoimport
tags: [Google, RSS, инструмент, конкурентная разведка, полезное, полезное, электронная почта]
---
Неприятной неожиданностью 1 июля 2013 года для меня оказалось то, что вместе с Google Reader была заблокирована возможность перенаправления результатов работы Google Alerts в RSS-ленту.

<img class="aligncenter size-full wp-image-3477" alt="google_alerts_no_longer_supports_RSS" src="/assets/uploads/google_alerts_no_longer_supports_RSS.png" width="707" height="60" />О сервисе Google Alerts я не так давно <a href="https://zlonov.ru/2013/02/legal_methods_of_competitive_intelligence/">писал</a> - он очень удобен для отслеживания появления новых страниц с интересующими вас ключевыми словами (бренды, имена людей, понятия и т.п.). Когда Google индексирует новую страницу, на которой находит заданные вами слова и/или выражения, он отправляет вам соответствующее уведомление (можно задать частоту: сразу, раз в день, раз в неделю). Ранее уведомления либо отправлялись на электронную почту, либо транслировались в RSS-ленту, а с 1 июля осталась только почта.

Про отключение Google Reader было известно заранее и желающие успели подготовиться (я, например, <a href="https://zlonov.ru/2013/03/5_reasons_to_choose_feedly_for_google_reader_users/">перешёл на Feedly</a>), а про такой вот нюанс работы Google Alerts если и сообщалось, то, видимо, где-то глубоко в недрах сервиса. Внезапно оказавшись без удобного привычного инструмента, испытал чувство дискомфорта и почти две недели пытался найти выход из сложившейся ситуации. Нет, читать часть сообщений в почте, а часть в новостной ленте мне решительно не хотелось.

Чего я только не перепробовал! Начал с поиска аналогичного сервиса у Яндекса. Оказалось, что что-то похожее есть, но только для <a href="http://help.yandex.ru/blogs/#1112097" target="_blank">Поиска по блогам</a>. Ума не приложу, что мешает организовать аналогичное для основного поиска...

Далее была гениальная, на мой скромный взгляд (смайл), идея подписаться на страницу результата поиска как на любую другую при помощи <a href="https://zlonov.ru/2013/02/legal_methods_of_competitive_intelligence/#page2rss">сервиса Page2RSS</a>. Однако, сервис Яндекс не позволил это сделать и лента стала наполняться малоинформативными:
<blockquote><em>ой...</em>

<em>Нам очень жаль, но запросы, поступившие с вашего IP-адреса, похожи на автоматические. По этой причине мы вынуждены временно заблокировать доступ к поиску.</em>

<em>Чтобы продолжить поиск, пожалуйста, введите символы с картинки в поле ввода и нажмите «Отправить».</em>
Стало понятно, что использовать получится только штатные методы самих поисковиков. Таким образом, пришлось вернуться к Google Alerts, но попытаться решить задачу трансляции почтовых сообщений в RSS-ленту.

Если ещё не пробовали - посмотрите на достаточно любопытный <a href="https://ifttt.com/" target="_blank">сервис IFTTT.com</a>, работающий по принципу создания рецептов (recipe): <em>If <strong>THIS</strong> than <strong>THAT</strong></em> или <em>Если <strong>ЭТО</strong>, то <strong>ТО</strong></em>. Где под <em><strong>THIS (ЭТО)</strong></em> подразумевается триггер - т.е. некое событие в любом из каналов (channels), а под <strong><em>THAT (ТО)</em> </strong>- действие, которое нужно предпринять опять-таки в каком-либо из каналов. Каналов можно настроить множество: почта, блог, профиль в социальной сети и т.д. - список большой и, как я понимаю, будет только пополняться. Вот для понимания парочка популярных рецептов:
<p style="text-align: center;"><img class="aligncenter  wp-image-3468" alt="recipes" src="/assets/uploads/recipes.png" width="549" height="218" />
Первый автоматически меняет картинку профиля в Твиттере при изменении её в Facebook, а второй автоматически создаёт твиты на основе RSS-ленты.

Собственно, канал RSS может использоваться только как триггер, но зато есть замечательный канал Blogger.com. Очередная гениальная, опять же - на мой скромнейший взгляд (смал, смайл), идея заключалась в том, чтобы по получению почтового сообщения от Google Alerts (оно приходит с ящика <em>googlealerts-noreply@google.com</em>) создавать в блоге запись с содержимым письма, а самому подписаться на RSS-ленту блога. К сожалению, этот рецепт так и не заработал, хотя другие варианты использования почты в качестве триггера и блога в качестве канала действия запускались без проблем. Неделя общения с техподдержкой задачу не решила, да и к тому же у такого подхода был неприятный побочный эффект - вся лента оказывалась публичной за счёт публикации в блог. Быть может, конечно, такой блог даже стал бы со временем мегапопулярным, но по каким-то техническим причинам ничего так и не получилось. Мой рецепт не заработал.
<p style="text-align: center;"><img class="aligncenter  wp-image-3493" alt="genius_recipe" src="/assets/uploads/genius_recipe1.png" width="539" height="158" />
Выход всё же в итоге был найден в виде <a href="http://emails2rss.appspot.com/" target="_blank">сервиса Emails to RSS</a>. Найти его было сложно, но работать с ним оказалось на удивление просто.

<strong>Шаг 1.</strong> Регистрируемся с использованием своего Google-аккаунта (ссылка login на <a href="http://emails2rss.appspot.com/" target="_blank">главной странице</a>).
<p style="text-align: center;"><img class="aligncenter  wp-image-3469" alt="001" src="/assets/uploads/001.png" width="569" height="179" />
<strong>Шаг 2</strong>. После регистрации получаем уникальный адрес электронной почты в домене <em>@emails2rss.appspotmail.com</em> и связанную с этим адресом RSS-ленту.
<p style="text-align: center;"><img class="aligncenter  wp-image-3470" alt="002" src="/assets/uploads/002.png" width="703" height="131" />
<p style="text-align: left;"><strong>Шаг 3</strong>. В Gmail отправляемся в <em>Настройки -&gt; Пересылка и POP/IMAP -&gt; Добавить адрес пересылки</em>, где указываем сгенерированный на предыдущем шаге уникальный адрес. Теперь адрес требуется подтвердить - Google отправляет на него соответствующее письмо с кодом подтверждения. В сам ящик зайти нельзя, но всё его содержимое автоматически публикуется в RSS-ленту, поэтому, подписавшись на неё, требуемый код подтверждения увидим в RSS-ридере.
<p style="text-align: center;"><img class="aligncenter  wp-image-3471" alt="003" src="/assets/uploads/003.png" width="532" height="136" />
<p style="text-align: left;"><strong>Шаг 4</strong>. Осталось настроить автоматическую переадресацию того, что мы хотим читать в виде RSS, на наш уникальный почтовый адрес. В моём случае все поступающие от <em>googlealerts-noreply@google.com</em> письма автоматически убираются в Архив и переадресовываются. Делается это здесь: <em>Настройки -&gt; Фильтры -&gt; Создать новый фильтр -&gt; Заполняем поле От -&gt; Создать фильтр в соответствии с этим запросом</em>. Далее всё, в общем-то, понятно.
<p style="text-align: center;"><img class="aligncenter  wp-image-3472" alt="004" src="/assets/uploads/004.png" width="402" height="358" />
<p style="text-align: left;">Теперь все письма, попадающие под критерии фильтра, будут переадресовываться на почтовый ящик, автоматически синхронизируемый с RSS-лентой.
<p style="text-align: left;">Приятно, что Email to RSS позволяет создать несколько мостов (bridges), т.е. связок <em>почтовый адрес &lt;-&gt; RSS-лента</em>. К основному уникальному имени (<em>%UNIQUE_NAME%</em>) через "_" вы сами добавляете произвольные символы и получаете, например, адрес <em>%UNIQUE_NAME%_discounts@emails2rss.appspotmail.com</em>, который можно использовать для всех рассылок со спецпредложениями или <em>%UNIQUE_NAME%_partnernews@emails2rss.appspotmail.com </em>для всевозможных входящих партнёрских рассылок. Каждый из этих адресов нужно активировать по выше приведённой схеме и создать соответствующие фильтры с опцией по пересылке.
<p style="text-align: left;">Остаётся только сердечно поблагодарить автора сервиса Email to RSS <a href="https://plus.google.com/114834583851544375518/posts" target="_blank">Володимира Штеновича</a>, живущего в Кракове и учившегося в Львовском Национальном Университете, и в очередной раз попенять мировым гигантам, отнимающим у рядовых пользователей удобные им инструменты из-за желания "<em>сфокусироваться на основных продуктах и улучшить их</em>".
