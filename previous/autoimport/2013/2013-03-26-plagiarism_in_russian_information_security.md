---
layout: zlonov/old_post
title: Плагиат в отечественных продуктах ИБ - где грань?
date: 2013-03-26 07:03
author: admin
category: autoimport
tags: [JaCarta, АльтЭль, информационная безопасность, Информзащита, Код Безопасности, мошенничество, НПО Эшелон]
---
<div dir="ltr">

Пока вход в Интернет по паспорту не стал реальностью и есть ещё <a href="https://zlonov.ru/2012/09/a_bit_of_anonymity_in_this_chilly_autumn_evening/">возможности для анонимного комментирования</a>, читатели блога продолжают раскрывать неизвестные подробности о рассматриваемых мной продуктах.

<img class="size-full wp-image-2370 aligncenter" alt="CopyPaste" src="/assets/uploads/2013/03/CopyPaste.jpg" width="600" height="400" />
<div>Так, например, некто Фыва <a href="http://zlonov.blogspot.ru/2011/05/who-is-mr-altell.html#comment-824182225">сообщает</a>, что: "<i>Altell neo - это модифицированная vyatta</i>" и уточняет: "<i>Естественно, они злостно нарушают лицензию</i>". Комментарий приведён к моему посту <a href="http://zlonov.blogspot.ru/2011/05/who-is-mr-altell.html">Who is Mr. ALTELL?</a>, посвящённому продукту одноимённой компании. Оставим за рамками отношения между работодателем и сотрудниками, но сам сценарий использования стороннего готового продукта (исходный код которого <a href="http://www.vyatta.org/downloads/source-code">доступен для свободного скачивания</a>) с последующей сертификация во ФСТЭК представляется вполне реалистичным. В конце концов, для одного из своих проектов <a href="http://zlonov.blogspot.ru/2012/10/6.html#vyatta">Микротест сертифицировал именно Vyatta</a>. Присвоение чужих наработок также могло бы объяснить и удивившую меня скорость появления новых продуктов.</div>
С другой стороны, сам ALTELL NEO вживую мне не встречался и оценить его схожесть с Vyatta не берусь. Опять-таки, локализация, техподдержка, наконец, сертификация - это то, что стоит денег и в продаже open-source по такой схеме нет ничего злостного. Нарушение GPL (если таковое, конечно, здесь имеется) в российских юридических реалиях - тоже <a href="http://ru.wikipedia.org/wiki/GNU_General_Public_License#.D0.A1.D0.BE.D0.BE.D1.82.D0.B2.D0.B5.D1.82.D1.81.D1.82.D0.B2.D0.B8.D0.B5_.D0.B7.D0.B0.D0.BA.D0.BE.D0.BD.D0.BE.D0.B4.D0.B0.D1.82.D0.B5.D0.BB.D1.8C.D1.81.D1.82.D0.B2.D1.83">вопрос всё ещё дискуссионный</a>, хоть и с давней историей.

В конце концов, <i>горячо любимая</i> мною компания НПО Эшелон два года спустя <a href="http://habrahabr.ru/post/112611/">после начала обсуждения на Хабре</a> их поделия Сканер ВС более-менее обосновала легальность данного продукта <a href="http://s3r.ru/04/03/2013/prikolyi/egocentricity/">у себя в блоге</a>, со свойственной им, правда, аргументацией ad hominem.

Создание собственных ИБ-продуктов на базе open-source в России распространено ничуть не меньше, чем в мире. Например, АПКШ Континент базируется на FreeBSD и вендор <a href="http://yandex.ru/yandsearch?text=freebsd%20site%3Ahttp%3A%2F%2Fwww.securitycode.ru%2F&amp;lr=213">особо этого не скрывает</a>. Вот только не совсем понятно, выполняется ли на практике требование <a href="http://www.freebsd.org/copyright/freebsd-license.html">лицензии The FreeBSD Project</a>:
<blockquote><i>Copyright 1992-2013 The FreeBSD Project. All rights reserved. </i><i>[…] должно оставаться указанное выше уведомление об авторском праве, этот список условий и последующий отказ от гарантий.</i>
Можно также вспомнить канувший в лету другой продукт (купленный в своё время Информзащитой) - <a href="http://distrowatch.com/table.php?distribution=linuxxp">Linux XP</a> (трансформировашийся, как я понимаю, теперь в <a href="http://www.rosalab.ru/products/">семейство решений от К</a><a href="http://www.rosalab.ru/products/">омпании РОСА</a>), который до конца так и не оправился от ранее <a href="http://linuxopen.ru/2008/06/03/bojjkot-distributiva-linux-xp.html">объявленного бойкота</a> со стороны linux-сообщества за нарушение GPL (хотя позднее вменяемые в вину создателям недостатки и были устранены).

Стоит признать, тем не менее, что умышленное или по недосмотру нарушение GPL и/или BSD лицензий всё равно у нас в стране вряд ли может привести к серьёзным сложностям со сбытом, особенно если рассматривать сертифицированные продукты. А вот использование этих формальных нарушений в качестве инструмента конкурентной борьбы при столкновении конфликтующих лоббистских интересов, на мой взгляд, вполне даже реалистично.

Нужно, правда, согласиться, что процесс доказательства плагиата и незаконного использования чужого исходного кода не так прост, тогда как клонирование аппаратных решений - вещь более наглядная и очевидная.
<p style="text-align: center;">Переходя от программных заимствований к аппаратным, можно вспомнить "ДжаКарту" (JaCarta),  которая <a href="http://zlonov.blogspot.ru/2012/02/jacarta-etoken.html#comment-436750297">по слухам</a> является клоном <a href="http://www.athena-scs.com/products-solutions/enterprise/pki#IDProtect%20Key%20LASER">IDProtect Key LASER</a> компании Athena и совершенно шедевральный, по моему скромному мнению, сертифицированный как межсетевой экран <a href="http://zlonov.blogspot.ru/2012/06/5.html#RSOS6850">коммутатор RSOS6850</a>:<img class="size-full wp-image-2373 aligncenter" alt="RSOS6850" src="/assets/uploads/2013/03/RSOS6850.jpg" width="675" height="426" />

<div></div>
В целом же, жаль, конечно, что искажённая в кривом зеркале сертификации российская ИБ-действительность, накладывает свои отпечатки в восприятии реальности и от отечественных поставщиков решений по безопасности никто даже и не ждёт кристальной честности. Так мы скоро, глядишь, и до своих <a href="http://izvestia.ru/news/545711">СПАРТАН 300</a> и <a href="http://naviny.by/rubrics/economic/2010/04/27/ic_articles_113_167592/">INTEGRAL</a> докатимся.

UPD. 26.03.2013 Простое сопоставление скриншотов из <a href="http://www.altell.ru/support_line/downloads.html">документации Altell</a> (в ней Vyatta не упоминается) и <a href="http://commons.wikimedia.org/wiki/File:Vyatta_web_interface.png?uselang=ru">описания Vyatta на Википедии</a>:
<p style="text-align: center;"><img class="size-full wp-image-2372 aligncenter" alt="Altell - Vyatta" src="/assets/uploads/2013/03/Altell-Vyatta.png" width="886" height="651" />
<p style="text-align: right;"><i>Изображение http://sobaka.com.ua/c/olds/sobaka/1218103376_20080807011555297_12.jpg</i>

</div>