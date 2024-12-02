---
layout: single
classes: wide

title: Как повторно установить некорректно удалённое приложение в macOS?
date: 2017-08-02
redirect_from:
  - /2017/08/howto-reinstall-app-in-macos/
AllowComments: true
category: HowTo
tags: [Check Point, Check Point Endpoint Security VPN, HowTo, InstallHistory.plist, macOS, macOS Sierra, pkgutil]
LinkedLinks: ""
---
Иногда при некорректном (например, ручном) удалении приложения не получается установить его повторно. На примере _Check Point Endpoint Security VPN_ ошибка может быть такой:

![Endpoint Security VPN build 860200405 is already installed on this computer](/assets/images/2017/Endpoint-Security-VPN-build-860200405-is-already-installed-on-this-computer.jpg)

Информацию о ранее установленных пакетах macOS хранит в файле `InstallHistory.plist`, расположенном в папке `/Library/Receipts/`. Перейти в папку можно нажав в Finder сочетание клавиш `Cmd+Shift+G` и введя её адрес `/Library/Receipts/`.

В файле `InstallHistory.plist` можно найти информацию о пакете простым поиском. Например, для _Check Point Endpoint Security VPN_ соответствующие строки будут выглядеть так:

```
<dict>
   <key>date</key>
   <date>2017-06-02T16:32:05Z</date>
   <key>displayName</key>
   <string>Endpoint Security VPN</string>
   <key>displayVersion</key>
   <string>860200405</string>
   <key>packageIdentifiers</key>
   <array>
      <string>com.checkpoint.pkg.epc</string>
   </array>
   <key>processName</key>
   <string>Installer</string>
</dict>
```

Просто так отредактировать `InstallHistory.plist`, открыв его в текстовом редакторе, не получится. Нужно воспользоваться _Терминалом_, для которого предусмотрена специальная команда по удалению из `InstallHistory.plist` информации об установленном пакете:

> `sudo pkgutil --forget packageIdentifier`

_packageIdentifier_ - это название требуемого пакета из `InstallHistory.plist`. Например, для того же _Check Point Endpoint Security VPN_ нужна команда:

> `sudo pkgutil --forget com.checkpoint.pkg.epc`

Так как используется `sudo`, то потребуется ввести пароль. Теперь повторная установка должна пройти без проблем.

Документация для утилиты _pkgutil_ доступна [здесь](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/pkgutil.1.html).
