---
layout: single
title: 'Как исправить проблему с USB-модемом Мегафона в OS X El Capitan, macOS Sierra?'
classes: wide

comments: true
tags: ['3G', 'El Capitan', 'Huawei', 'macOS Sierra', 'USB-модем', 'OS X', 'Мегафон', 'модем', 'macOS']
category: HowTo
AllowComments: true
LinkedLinks: ""
---
Иногда возникает проблема с тем, что в среде OS X El Capitan или macOS Sierra не виден USB-модем (в моём случае - Мегафон модель E352). При подключении к Windows-машине всё корректно работает, а в среде Mac OS индикатор мигает, встроенное в модем ПО устанавливается без ошибок, но в самом приложении от Мегафона модем не виден - "`Нет устройства/Устройство не подключено`".

{% include one_image_new2.html picture_name="Мегафон - Нет устройства" picture_path="2016/No device.jpg" %}

Решение проблемы (в моём случае помогло):

 - Выполнить полную деинсталяцию всего ПО от Мегафона
   - Дополнительно можно вручную удалить все упоминания _"megafon"_ и _"huawei"_ в папках `Library/System/Extensions`, `~/Library/LaunchAgents` и `Library/LaunchAgents`
 - Скачать с сайта [Мегафона](http://svr.shop.megafon.ru/modems/79727.html?archVal=1#files) свежую версию ПО для модема (в моём случае - [Connection Manager (2013) - Обновление ПО для работы с MAC OS](http://svr.shop.megafon.ru/get_binary.php?type=a&amp;cid=10&amp;gid=62188&amp;pos=7))
 - Перезагрузить компьютер в Режиме восстановления (Recovery mode) удержанием `Cmd+R` при старте.
 - Открыть Терминал и ввести команду `csrutil disable`.
 - Перезагрузиться.
 - Установить скачанное ПО от Мегафона.
 - Подключить 3G-модем к USB-порту и убедиться, что всё работает.
 - Ещё раз перегрузиться в Режиме восстановления, открыть Терминал и ввести команду `csrutil enable`.
 - Перезагрузиться и наслаждаться работой.

Данная команда (`csrutil`) включает/отключает работу службы System Integrity Protection (подробнее про неё: [https://support.apple.com/en-us/HT204899](https://support.apple.com/en-us/HT204899)), которая не даёт корректно устанавливаться корявым драйверам от Huawei/Мегафона.
