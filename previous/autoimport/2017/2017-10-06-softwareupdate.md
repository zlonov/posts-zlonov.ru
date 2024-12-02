---
layout: zlonov/old_post
title: '[HowTo] Как обновить macOS через команды в Терминале?'
date: 2017-10-06 14:50
author: admin
category: autoimport
tags: [HowTo, macOS, macOS High Sierra, macOS Sierra, softwareupdate, обновление, Терминал]
---
Замечено, что при плохом (медленном) Интернет-соединении и большом размере обновлений штатное графическое приложение macOS может существенно "подтормаживать" и нередко прерывает процесс скачивания обновления (например, операционной системы) без возможности его возобновить - процесс приходится запускать заново.

[caption id="attachment_11125" align="aligncenter" width="1024"]<a href="/assets/uploads/Нет-доступных-обновлений.png"><img class="size-large wp-image-11125" src="/assets/uploads/Нет-доступных-обновлений-1024x191.png" alt="Нет доступных обновлений" width="1024" height="191" /></a> Нет доступных обновлений[/caption]

В таких случаях будет полезно воспользоваться возможностями Терминала (командной строки). В большинстве ситуаций достаточно будет вот таких простых команды:

<hr />

Проверка доступных обновлений:
<pre>softwareupdate -l</pre>
&nbsp;

Установка всех доступных обновлений:
<pre>sudo softwareupdate -ia</pre>
&nbsp;

Более подробную справку про утилиту <strong>softwareupdate</strong> можно получить командой:
<pre>softwareupdate -h</pre>

<hr />
