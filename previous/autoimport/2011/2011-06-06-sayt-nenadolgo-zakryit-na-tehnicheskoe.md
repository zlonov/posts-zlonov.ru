---
layout: zlonov/old_post
title: Сайт ненадолго закрыт на техническое обслуживание. Зайдите через минуту.
date: 2011-06-06 18:41
author: admin
category: autoimport
tags: [WordPress, информационная безопасность, ошибка, сайтоведение]
---
<img class="aligncenter" title="http://pics.livejournal.com/kinouho/pic/001sqs83" src="https://pics.livejournal.com/kinouho/pic/001sqs83" alt="http://pics.livejournal.com/kinouho/pic/001sqs83" width="160" height="144" />

WordPress - хороший движок для сайта, да ещё и бесплатный, но с ним бывают иногда сложности. Например, сегодня при обновлении плагина, сайт "взбрыкнул" и ушёл в режим обслуживания. Надпись "Сайт ненадолго закрыт на техническое обслуживание. Зайдите через минуту." красовалась не только вместо главной страницы, но и при попытке входа в консоль администрирования.

К счастью, проблема лечится просто - достаточно зайти в корневую папку сайта (через ftp или файловый менеджер хостинг-центра) и удалить файл<em> .maintenance</em>

<em><a href="/assets/uploads/2011/06/maintenance.png"><img class="aligncenter size-medium wp-image-1027" title="maintenance" src="https://i1.wp.com/zlonov.ru/wp-content/uploads/2011/06/maintenance.png?fit=222%2C300&#038;ssl=1" alt="" width="222" height="300" /></a></em>

Повторная попытка обновления плагина прошла успешно.
