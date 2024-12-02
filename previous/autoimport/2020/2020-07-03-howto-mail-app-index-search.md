---
layout: zlonov/old_post
title: "Как исправить проблемы с поиском в почтовом клиенте Mail App в macOS?"
date: 2020-07-03 12:55
category: HowTo
category: autoimport
tags: [HowTo, macOS, Mail App, индекс, поиск, почта, сообщение, электронная почта]
---

<strong>Суть проблемы</strong>: письмо точно есть, но Mail App его не может найти.



<strong>Варианты решения</strong>:


<!-- wp:list {"ordered":true} -->
<ol><li>Убедиться, что самые очевидные варианты не помогают: <a href="https://support.apple.com/ru-ru/guide/mail/mlhlp1192/mac">Если при поиске не удается найти нужные письма в приложении «Почта» на компьютере Mac</a></li><li>Выбрать проблемный почтовый ящик на левой боковой панели (или несколько) и перестроить его (<em>Ящик -> Перестроить</em>), вот официальная справка: <a href="https://support.apple.com/ru-ru/guide/mail/mlhlp1227/mac">Восстановление почтовых ящиков в приложении «Почта» на Mac</a></li><li>Перестроить индекс Spotlight: <a href="https://support.apple.com/ru-ru/HT201716">Повторная индексация Spotlight на компьютере Mac</a></li><li><a href="https://apple.stackexchange.com/questions/230239/mail-search-not-finding-messages-but-spotlight-does">Переиндексировать всю почту </a>- самый долгий, но самый эффективный способ:<ol><li>Закрыть Mail App.</li><li>Перейти в папку <em>~/Library/Mail/V7/MailData</em> (для других версий macOS вместо <em>V7</em> могут быть другие цифры).</li><li>Удалить (а лучше - временно перенести в другое место) все файлы, начинающиеся с <em>Envelope Index</em>.</li><li>Запустить Mail App и дождаться завершения импорта всех сообщений (может быть весьма долго).</li></ol></li></ol>




