---
title: Ввод спецсимволов Unicode в macOS
tags:
  - macOS
  - Unicode
---
Ссылка: https://habr.com/ru/articles/12223/
Ссылка: https://ladedu.com/how-to-enter-unicode-characters-on-a-mac/

Алгоритм:
1. Добавить Unicode-раскладку
2. Выбрать эту раскладку
3. В нужном месте зажать `Options (⌥)` и, не отпуская, ввести код символа.

Пример:
- Спец-символ: `&#x202E;`
- Ввод: `⌥` + `202e`
- Результат: `А роза упала на лапу Азора` -> `‮А роза упала на лапу Азора`

---
Примеры символов (коды другие):
> [!info] [Where can I find the unicode symbols for Mac functional keys? (Command, Shift, etc.)](https://apple.stackexchange.com/questions/55727/where-can-i-find-the-unicode-symbols-for-mac-functional-keys-command-shift-e)

```
HTML Entity     GLYPH  NAME
&#63743;              Apple
&#8984;         ⌘      Command, Cmd, Clover, (formerly) Apple
&#8963;         ⌃      Control, Ctl, Ctrl
&#8997;         ⌥      Option, Opt, (Windows) Alt
&#8679;         ⇧      Shift
&#8682;         ⇪      Caps lock
&#9167;         ⏏      Eject
&#8617;         ↩      Return, Carriage Return
&#8629; &crarr; ↵      Return, Carriage Return
&#9166;         ⏎      Return, Carriage Return
&#8996;         ⌤      Enter
&#9003;         ⌫      Delete, Backspace
&#8998;         ⌦      Forward Delete
&#9099;         ⎋      Escape, Esc
&#8594; &rarr;  →      Right arrow
&#8592; &larr;  ←      Left arrow
&#8593; &uarr;  ↑      Up arrow
&#8595; &darr;  ↓      Down arrow
&#8670;         ⇞      Page Up, PgUp
&#8671;         ⇟      Page Down, PgDn
&#8598;         ↖      Home
&#8600;         ↘      End
&#8999;         ⌧      Clear
&#8677;         ⇥      Tab, Tab Right, Horizontal Tab
&#8676;         ⇤      Shift Tab, Tab Left, Back-tab
&#9250;         ␢      Space, Blank
&#9251;         ␣      Space, Blank
```