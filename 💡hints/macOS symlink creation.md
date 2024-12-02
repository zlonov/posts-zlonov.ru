---
title: Создание символьных ссылок (symlink) в macOS
tags:
  - macOS
  - file_system
---
> [!info] По мотивам: [Symlink Tutorial in Linux – How to Create and Remove a Symbolic Link](https://www.freecodecamp.org/news/symlink-tutorial-in-linux-how-to-create-and-remove-a-symbolic-link)

Создание в папке `iCloud Drive/Obsidian/Zettelkästen/` ссылки на папку `~/Git/hub.zlonov.ru/content/` с именем `hub`:
```console
cd ~/Library/Mobile\ Documents/iCloud\~md\~obsidian/Documents/Zettelkästen
ln -s ~/Git/hub.zlonov.ru/content hub
```

