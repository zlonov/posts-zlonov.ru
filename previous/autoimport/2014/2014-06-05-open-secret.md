---
layout: zlonov/old_post
title: Secret Полишинеля
date: 2014-06-05 23:34
author: admin
category: autoimport
tags: [iPhone, Secret, анонимность, информационная безопасность, разоблачение, социальные сети]
---
Топ-чарты приложений в App Store удобны, в частности, тем, что позволяют отыскивать любопытные приложения без особых усилий. Так я, например, наткнулся на социальную сеть, само название которой не могло не вызвать моего интереса. Речь о приложении Secret.

Secret представляет собой анонимную социальную сеть. Суть её в том, что вы не знаете, кто именно написал то или иное сообщение. Все комментарии тоже анонимны. Выбрать и добавить друзей самостоятельно нельзя: приложению нужно предоставить доступ к списку контактов и тогда оно самостоятельно по адресам электронной почты и телефонам подберёт тех ваших друзей/знакомых, которые уже присутствуют в сети.

Из деанонимизирующих признаков присутствует только явное указание, если пост оставил кто-то из ваших прямых друзей. Остальные посты помечаются как принадлежащие друзьям друзей или только географической отметкой, с указанием того, где они были написаны, если это сообщение друга друга друга, друга друга друга друга и т.д.

Такой подход по задумке создателей предполагает откровенность в общении и действительно, чего только там не начитаешься =) На самом деле, если вы хорошо знаете своих друзей (и/или их будет не очень много), то авторство многих постов угадать довольно просто, но, конечно, такие предположения бездоказательны, ведь кто-то может специально копировать манеру другого человека, например.

Тем не менее, немного поэкспериментировав с принципами работы приложения, довольно быстро отыскал простой сценарий чтения "секретных" постов конкретного человека. Для успеха нам потребуются следующие ингредиенты:
<ul>
	<li>телефон с пустым списком контактов;</li>
	<li>точный адрес электронной почты или телефон, который использовал этот человек для регистрации.</li>
</ul>
Оказалось, что процесс регистрации в сети Secret до удивления примитивен - нужно только указать адрес электронной почты и пароль. Всё. При этом на указанный адрес приходит запрос на подтверждение, но подтверждение не обязательно. Адрес вообще может быть несуществующим. Аналогичная история и с номером телефона - на самом деле его не проверяют. Итак, сценарий для получения доступа ко всем постам конкретного человека в сети Secret может быть, например, такой.

Берём телефон с пустой адресной книгой (как вариант, можно для iPhone временно отключить синхронизацию контактов с iCloud и удалить все контакты) и создаём там контакт интересующего нас человека. Да, это самое сложное - надо точно знать, какой адрес он(а) использовал(а) при регистрации. С другой стороны, скорее всего это будет личный ящик на mail.ru или google.com и вы наверняка его знаете.

Теперь регистрируемся в этой (якобы) совершенно анонимной социальной сети Secret с любым придуманным адресом электронной почты и соглашаемся, чтобы приложение поискало в своей базе нашего единственного друга. Для этого приложению нужно предоставить доступ к контактам.
<p style="text-align: center;"><a href="/assets/uploads/Secret-Find-Friend.png"><img class="size-medium wp-image-5559" src="/assets/uploads/Secret-Find-Friend-200x300.png" alt="Secret-Find-Friend" width="200" height="300" /></a>  <a href="/assets/uploads/Secret-Access-To-Contacts.png"><img class="size-medium wp-image-5560" src="/assets/uploads/Secret-Access-To-Contacts-200x300.png" alt="Secret-Access-To-Contacts" width="200" height="300" /></a>
<p style="text-align: left;">Однако, приложение не хочет показывать посты (секреты) от друзей, пока вы не введёте свой номер телефона. Никаких проблем - ввести можно всё, что угодно, никаких проверок на достоверность номера не делается.<a href="/assets/uploads/Secret-1-Friend.png">
</a>
<p style="text-align: left;"><a href="/assets/uploads/Secret-Need-Phone.png"><img class="size-medium wp-image-5561 aligncenter" src="/assets/uploads/Secret-Need-Phone-200x300.png" alt="Secret-Need-Phone" width="200" height="300" /></a> Следующее затруднение - приложение уведомляет, что для просмотра сообщений от друзей их должно быть как минимум трое. Ничего страшного - достаточно придумать два любых адреса электронной почты и поочерёдно зарегистрироваться с ними в соцсети Secret. Далее надо лишь добавить эти адреса в контакты на нашем телефоне и приложение при обновлении увеличит счётчик друзей (по сути, это и есть основной трюк - "фейковые" друзья, которых вы создаёте сами).
<p style="text-align: center;"><a href="/assets/uploads/Secret-1-Friend.png"><img class="size-medium wp-image-5562" src="/assets/uploads/Secret-1-Friend-200x300.png" alt="Secret-1-Friend" width="200" height="300" /></a>  <a href="/assets/uploads/Secret-3-Friends.png"><img class="size-medium wp-image-5563" src="/assets/uploads/Secret-3-Friends-200x300.png" alt="Secret-3-Friends" width="200" height="300" /></a>
<p style="text-align: left;">Как видно на скриншоте выше - при наличии трёх друзей приложение соглашается показывать посты от них, но не помечает их как сделанные именно друзьями. Так что нужно ещё два адреса. На самом деле, сначала я пытался регистрировать реальные специально свежесозданные электронные адреса, но когда выяснилось, что их реальность не проверяется, дело пошло быстрее. В общем, обеспечить любое количество псевдодрузей совсем несложно.
<p style="text-align: left;"><a href="/assets/uploads/Secret-Contats.png"><img class="size-medium wp-image-5564 aligncenter" src="/assets/uploads/Secret-Contats-267x300.png" alt="Secret-Contats" width="267" height="300" /></a>
<p style="text-align: left;">Собственно, вот и всё. У вашего аккаунта в соцсети Secret теперь один единственный реальный друг, которого вы достоверно знаете и все посты от которого помечаются как <em>сделанные другом</em>. Следите на здоровье =)
Можно ли обычному пользователю как-то справиться с этим <em>конструктивным недостатком</em> соцсети Secret? Да, можно в настройках приложения поменять адрес электронной почты и телефон на ненастоящие или никому неизвестные, никакие друзья при этом не пропадут, но описанный выше сценарий к вам никто применить не сможет. Конечно, если все пользователи будут использовать поддельные контактные данные, число друзей ни у кого расти не будет, но... вы действительно хотите рассказывать (пусть и анонимно) реальные свои секреты тем людям, которых знаете? Тогда какое вам вообще дело до анонимности? =)

В приложении ещё есть опция по "отвязыванию" любых прошлых постов и комментариев от вашего аккаунта, но в деталях её не тестировал и не знаю, какая от неё практическая польза.

Вообще же, в таких случаях я всегда вспоминаю правило Миранды для цифрового мира, <a href="http://zl.lc/163s9" target="_blank">сформулированное несколько лет назад Михаилом Емельянниковым</a>: «<em>Все, что вы указали о себе в социальной сети, блоге, форуме, чате, любом общедоступном сервисе, будет храниться там вечно и всегда может быть использовано против вас</em>». Так что будьте аккуратны в своих <em>анонимных</em> откровениях =)

&nbsp;