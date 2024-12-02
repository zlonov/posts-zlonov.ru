---
layout: single
classes: wide

title: "Как перестроить индекс Spotlight в macOS?"
date: 2024-01-09
tags: [Apple, macOS, ошибка, 'Spotlight', 'поиск', 'индекс']
categories: ['HowTo']

excerpt: "Решение проблемы с неправильно работающим поиском."

header:
    teaser: /assets/images/2024/spotlight.jpg
    overlay_image: /assets/images/2024/spotlight.jpg
    show_overlay_excerpt: true
    overlay_filter: 0.25 # same as adding an opacity of 0.5 to a black background
---
Когда при поиске на компьютере Mac не получается найти нужную информацию, она выдаётся с ошибками, неполная либо с какими-либо иными результатами, отличными от ожидаемых, помогает переиндексация (повторная индексация) Spotlight.

Официальная справка от Apple [рекомендует](https://support.apple.com/ru-ru/102321) сначала добавить проблемную область поиска (в принципе, это может быть и весь диск целиком) в исключения Spotlight, а потом убрать из исключений.

К сожалению, иногда этот способ не помогает. В таких случаях на помощь приходит встроенная в macOS утилита `mdutil`.

Полный список ключей и опций этой утилиты традиционно доступен по команде `man mdutil`, а краткая справка приведена в конце поста. 

Из всех доступных опций нам потребуются флаги `-E` для удаления текущих метаданных Spotlight (т.е. ранее построенного проблемного индекса) и `-a` для того, чтобы команда применилась ко всем хранилищам на всех дисках.

В принципе, можно ограничиться явным указанием конкретного диска, но проще уж перестроить все индексы без исключений.

Запускать команду надо от имени администратора, поэтому используем `sudo` и вводим пароль:

```console
sudo mdutil -E -a
```
В Интернете можно ещё найти рекомендацию использовать такой вариант:

```console
sudo mdutil -E /
```

Эта команда перестраивает индекс для всех подключенных/смонтированных дисков, но конкретно мне мой вариант помог больше.

___

### Краткая справка команды mdutil

```console
Usage: mdutil -pEsa -i (on|off) -d volume ...
       mdutil -t {volume-path | deviceid} fileid
	Utility to manage Spotlight indexes.
	-i (on|off)    Turn indexing on or off.
	-d             Disable Spotlight activity for volume (re-enable using -i on).
	-E             Erase and rebuild index.
	-s             Print indexing status.
	-a             Apply command to all stores on all volumes.
	-t             Resolve files from file id with an optional volume path or device id.
	-p             Publish metadata.
	-V vol         Apply command to all stores on the specified volume.
	-v             Display verbose information.
	-r plugins     Ask the server to reimport files for UTIs claimed by the listed plugin.
	-L volume-path List the directory contents of the Spotlight index on the specified volume.
	-P volume-path Dump the VolumeConfig.plist for the specified volume.
	-X volume-path Remove the Spotlight index directory on the specified volume.  Does not disable indexing.
	               Spotlight will reevaluate volume when it is unmounted and remounted, the
	               machine is rebooted, or an explicit index command such as 'mdutil -i' or 'mdutil -E' is
	               run for the volume.
NOTE: Run as owner for network homes, otherwise run as root.
```