---
layout: zlonov/old_post
title: 12/1001. Что не так со Skype?
date: 2010-12-22 02:54
author: admin
category: autoimport
tags: ['1001', ICQ, Skype, интернет, информационная безопасность]
---
<div dir="ltr">
<div><a href="http://4.bp.blogspot.com/-lwOTlgBlBCs/UKOy2wIHfuI/AAAAAAAABeQ/fD8MGJA3OkA/s1600/skypenaroducyrlogo.png"><img alt="" src="https://4.bp.blogspot.com/-lwOTlgBlBCs/UKOy2wIHfuI/AAAAAAAABeQ/fD8MGJA3OkA/s400/skypenaroducyrlogo.png" width="400" height="312" border="0" /></a></div>
В  двух первых ночах проекта Тысяча и одна ночь безопасности уже рассматривался (<a href="http://zlonov.blogspot.com/2009/12/blog-post.html">1/1001</a>, <a href="http://zlonov.blogspot.com/2009/12/blog-post_23.html">2/1001</a>) сервис обмена мгновенных сообщений <strong>ICQ</strong>. Его слабость с точки зрения вопросов информационной безопасности может служить хорошим поводом для перехода на альтернативные варианты, например, на <strong>Skype</strong>, который давно уже не воспринимается как средство только для голосовой и видео связи. Однако, не всё так радужно и с этим вариантом общения по сети.
<a name="more"></a>
Что мы чаще всего слышим про Skype и его безопасность?
<ul>
	<li>Весь трафик Skype надёжно зашифрован</li>
	<li>Skype сложно/невозможно заблокировать администраторам сети</li>
	<li>Skype не любят спецслужбы, т.к. не могут его перехватывать/Skype создали спецслужбы, чтобы следить за всеми</li>
</ul>
Что-то из этого правда, что-то - не совсем, но есть некоторые важные и неоспоримые факты, которые нужно учитывать, даже если их трактовка может быть различная.

<strong>Skype использует закрытые алгоритмы</strong>

Спор о том, что лучше с точки зрения безопасности - открытые исходные коды или наоборот - можно вести долго, но суть дела это не меняет. Надёжность закрытых систем можно определить только с помощью реинжиниринга (процесс "обратного" анализа работы алгоритма) или экспериментально. Верить рекламным заявлениям производителя о высокой безопасности никто ведь, надеюсь, не собирается?

Skype в вопросе закрытости пошёл настолько дальше, насколько это только возможно. И следующий важный факт:

<strong>Skype использует закрытые протоколы</strong>

Что это означает на практике? Никто не может написать стороннего клиента для Skype без дополнительных усилий. Клиентов для ICQ много и, хотя пользователи альтернативных клиентов периодически испытывают проблемы с подключениями, в целом, процесс выпуска альтернатив отлажен. Для Skype альтернатив практически нет. Зачем нужны альтернативы, спросите Вы? Ну хотя бы для того, чтобы не зависеть от разработчика при выборе платформы (Mac, PC, Android, iOS и т.п.) или иметь возможность использовать аггрегированные сервисы обмена сообщений. Единственный сервис, поддерживающй среди прочих популярных протоколов и Skype, который мне удалось найти - это <a href="https://imo.im/" target="_blank">imo.im</a>, принцип работы которого, к своему стыду я пока не понял. При вводе логина и пароля от Skype Вы получаете полный доступ к своему Skype-чату с единственной обнаруженной мной неработающей "фишкой" - групповые чаты.

Почему же для Skype нет альтернативных клиентов? Разработчики не только не опубликовали стандарта протокола, но и постарались максимально усложнить жизнь реинженерам, которые несмотря на все препятствия, сумели обойти защиту и понять принципы работы Skype.  Очень хорошая статья на эту тему есть <a href="http://www.computerra.ru/own/kiwi/546763/">здесь</a>.

<strong>Skype строит Империю</strong>

Выше уже говорилось о сервисах аггрегации служб обмена сообщений, несомненным перимуществом которых является возможность общения в рамках одного приложения со всеми контактами изо всех контакт-листов разных сервисов обмена мгновенных сообщений (ICQ, Skype, Jabber и т.д.)

К нашему (пользователей) сожалению, Skype посследовательно рассорился с <a href="http://www.fring.com/newsroom/skypeblocksfring.asp" target="_blank">Fring</a>, <a href="http://www.3dnews.ru/software-news/nimbuzz-prekrashchaet-podderzhku-servisov-skype/" target="_blank">Nimbuzz</a> и, наверняка, другими крупными игроками. На сегодняшний день, если Вы хотите в "едином окне" общаться с Вашими друзьями из  Skype-чата и любого другого контакт-листа, приготовьтесь к сложностям, ограничениям (в том числе и по платформам) и прочим неприятностям.

Всё вышеописанное может означать только одно - Skype в наш век "объединения всех со всеми во имя Пользователя" пытается построить свою собственную вселенную, в которой не место остальным. Не являясь провидцем, всё же сочту такую позицию неверной. Вселенная Apple в виде iPhone, вселенная Microsoft в виде приложения от Apple, работающего на рабочем (это, вроде, не тафтология или да?) Windows 7, и вселенная Google, в виде возможности синхронизации в вышеупомянутом приложении контактов Gmail и Mobile Me, умеют найти общий язык между собой. Skype же предпочитает использовать свой собственный язык, досконально известный только ему самому.

<strong>Заключение</strong>

Непростой получился пост, как для читателей, так и для автора. Готовых и всеми одобренных ответов на большинство поднятых вопросов пока нет. Skype, вне всякого сомнения, удобен, но (c) меня терзают смутные сомнения...

<em>И первые лучи солнца озарили подборку статей про Skype...</em>
<ul>
	<li><a href="http://www.xakep.ru/post/38543/?page=9" target="_blank">Skype: скрытая угроза</a></li>
	<li><a href="http://habrahabr.ru/blogs/infosecurity/98546/" target="_blank">Раскрыт самый большой секрет Skype (Habrahabr)</a></li>
	<li><a href="http://www.skype.com/intl/ru/security/online-safety" target="_blank">Информационная безопасность в Skype (Skype)</a></li>
	<li><a href="http://ru.wikipedia.org/wiki/Skype#.D0.9A.D1.80.D0.B8.D1.82.D0.B8.D0.BA.D0.B0" target="_blank">Skype - Критика (Википедия)</a></li>
	<li><a href="http://lurkmore.ru/Skype#.D0.A1.D0.B5.D0.BA.D1.80.D0.B5.D1.82.D1.8B.E2.84.A2_.D1.81.D0.BA.D0.B0.D0.B9.D0.BF.D0.B0" target="_blank">Секреты Skype (Lurkmore)</a> =)</li>
</ul>
</div>