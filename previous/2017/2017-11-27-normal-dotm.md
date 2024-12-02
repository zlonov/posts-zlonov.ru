---
layout: single
classes: wide

title: "Как исправить ошибку с открытием шаблона Normal.dotm в Microsoft Office 2016 для Mac?"

date: 2017-11-27
redirect_from:
  - /2017/11/normal-dotm/
AllowComments: true
category: 'HowTo'
tags: ['HowTo', 'macOS', 'Microsoft Office 2016 для Mac', 'Microsoft Word для Mac', 'Normal.dotm', 'ошибка']
LinkedLinks: ""
---

**Симптом**: при открытии Microsoft Word для Mac возникает ошибка: _Не удается открыть существующий общий шаблон (Normal.dotm)_.

{% include one_image_new2.html picture_name="Не удается открыть существующий шаблон Normal.dotm" picture_path="2017/Ошибка шаблона.png" %}

Ошибки возникают также и при закрытии документов Word (невозможность сохранить _Normal.dotm_ и проч.).

**Решение**:
  - Закрыть _Microsoft Word для Mac_.
 	- Перейти в папку `~/Library/Group Containers/UBF8T346G9.Office/User Content/Templates/`, для чего надо в Finder нажать `Cmd+Shift+G` и ввести этот путь к папке `~/Библиотеки/Group Containers/UBF8T346G9.Office/Содержимое пользователя/Шаблоны/` (обратите внимание - для русской и английской версий пути различаются).
 	- Удалить файл _Normal.dotm_ из папки - желательно не удалять его сразу безвозвратно, а сначала временно просто переместить из этой папки, например, на рабочий стол, и проверить, что решение помогло.
  - Желательно перезагрузить Mac.
 	- Запустить _Microsoft Word для Mac_ и создать новый докуент, файл _Normal.dotm_ должен при этом создаться автоматически.

В большинстве случаев должно помочь.
