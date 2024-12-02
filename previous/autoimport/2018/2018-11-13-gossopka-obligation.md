---
layout: zlonov/old_post
title: Обязательность подключения к ГосСОПКА
date: 2018-11-13 12:57
author: admin
category: autoimport
tags: [187-ФЗ, ГосСОПКА, информационная безопасность, КИИ, НКЦКИ, приказ 239]
---

Нетрудно понять производителей средств, которые могут использоваться для подключения к ГосСОПКА, в их попытке не то чтобы обмануть или ввести заказчиков в заблуждение, а скорее - не совсем корректно расставить акценты в обосновании обязательности использования их решений.



Вот примерно такие рассуждения можно порой встретить в презентациях, статьях и на вебинарах:



...многие предприятия <em>%ОТРАСЛЬ_ПРОМЫШЛЕННОСТИ% </em>попали под действие 187-ФЗ и должны будут подключаться к системе ГосСОПКА.  <em>%КЛАСС_СИСТЕМ% </em>— это основные системы, которые будут категорироваться как объекты КИИ, и в ГосСОПКА необходимо будет отправлять инциденты в первую очередь из них. <em>%НАЗВАНИЕ_ПРОДУКТА%</em> тут незаменим.



Между прочим, в <a href="https://www.youtube.com/watch?v=thrZPNf5WCI&amp;list=PLvxhSg-LXXAegQk0N9Q7ymPfd7QLTAxRG&amp;index=4&amp;t=0s">третьей серии вебинаров УЦСБ про безопасность КИИ</a> (на 26 минуте) есть тоже весьма неоднозначный слайд по этой теме:


<!-- wp:image {"id":72661,"align":"center"} -->
<div class="wp-block-image"><figure class="aligncenter"><img src="https://i0.wp.com/zlonov.ru/wp-content/uploads/Обязательность-ГосСОПКА.jpg?fit=1024%2C585&amp;ssl=1" alt="" class="wp-image-72661"/><figcaption>Обязательность ГосСОПКА</figcaption></figure></div>
<!-- /wp:image -->


Тут, правда, хотя бы речь про 1 и 2 категорию значимости, но опять же: "Обязательно". Давайте разбираться, что и кто имеет (должен иметь) в виду на самом деле.



Начать разумнее всего, понятно, с самого&nbsp;<a href="https://zlonov.ru/kii/187-%D1%84%D0%B7/">Федерального закона 187-ФЗ "О безопасности КИИ"</a>, где и определена ГосСОПКА (статья 5 часть 1):



1. Государственная система обнаружения, предупреждения и ликвидации последствий компьютерных атак на информационные ресурсы Российской Федерации представляет собой <strong>единый территориально распределенный комплекс</strong>, включающий <strong>силы</strong> и <strong>средства</strong>, предназначенные <strong>для обнаружения, предупреждения</strong> и <strong>ликвидации последствий </strong>компьютерных атак и <strong>реагирования</strong> на компьютерные инциденты. В целях настоящей статьи под информационными ресурсами Российской Федерации понимаются информационные системы, информационно-телекоммуникационные сети и автоматизированные системы управления, находящиеся на территории Российской Федерации, в дипломатических представительствах и (или) консульских учреждениях Российской Федерации.



Впрочем, для поставленного вопроса не так важно, что такое ГосСОПКА: важнее понять, какие обязанности есть у субъектов КИИ в отношении неё. Обязанности эти определены в статье 9 того же 187-ФЗ и определены для всех субъектов КИИ в части 2 и субъектов КИИ с значимыми объектами в части 3 (ниже выдержка конкретно про ГосСОПКА):



2. <strong>Субъекты</strong>критической информационной <strong>обязаны</strong>: 1) <strong>незамедлительно информировать</strong> о <strong>компьютерных инцидентах</strong> федеральный орган исполнительной власти, уполномоченный в области обеспечения функционирования государственной системы обнаружения, предупреждения и ликвидации последствий компьютерных атак на информационные ресурсы Российской Федерации, а также Центральный банк Российской Федерации (в случае, если субъект критической информационной инфраструктуры осуществляет деятельность в банковской сфере и в иных сферах финансового рынка) <strong>в установленном</strong> указанным федеральным органом исполнительной власти <strong>порядке</strong> (в банковской сфере и в иных сферах финансового рынка указанный порядок устанавливается по согласованию с Центральным банком Российской Федерации)



3. <strong>Субъекты</strong> критической информационной инфраструктуры, <strong>которым</strong> на праве собственности, аренды или ином законном основании <strong>принадлежат значимые объекты</strong> критической информационной инфраструктуры, наряду с выполнением обязанностей, предусмотренных частью 2 настоящей статьи, <strong>также обязаны</strong>: 1) <strong>соблюдать требования по обеспечению безопасности</strong> значимых объектов критической информационной инфраструктуры, установленные федеральным органом исполнительной власти, уполномоченным в области обеспечения безопасности критической информационной инфраструктуры Российской Федерации;



С частью 2 (пункт 1) всё понятно: "<em>обязаны незамедлительно информировать о компьютерных инцидентах</em>", - речь явно про ГосСОПКА. А вот часть 3 (тоже пункт 1) для его связи с ГосСОПКА надо дополнить ещё цитатами - из статьи 10 187-ФЗ:



1. <strong>В целях обеспечения безопасности значимого объекта</strong> критической информационной инфраструктуры <strong>субъект</strong> критической информационной инфраструктуры <strong>в соответствии с требованиями</strong> к созданию систем безопасности таких объектов и обеспечению их функционирования, утвержденными федеральным органом исполнительной власти, уполномоченным в области обеспечения безопасности критической информационной инфраструктуры Российской Федерации, <strong>создает систему безопасности </strong>такого объекта <strong>и обеспечивает ее функционирование</strong>.<br />2. Основными <strong>задачами системы безопасности</strong> значимого объекта критической информационной инфраструктуры <strong>являются</strong>:<br />...<br />4) <strong>непрерывное взаимодействие с государственной системой обнаружения, предупреждения и ликвидации последствий компьютерных атак на информационные ресурсы Российской Федерации</strong>.



Итак, все субъекты обязаны информировать о компьютерных инцидентах в установленном порядке (статья 9 часть 2), а субъекты с значимыми объектами КИИ обязаны создать систему безопасности, одной из задач которой является непрерывное взаимодействие с ГосСОПКА (статья 10 часть 3 и статья 10 части 1 и 2).



Для начала определимся с тем, какой именно порядок <em>установлен</em>для информирования о компьютерных инцидентах. Устанавливать его должен федеральный орган исполнительной власти (ФОИВ), <a href="https://zlonov.ru/kii/%D1%83%D0%BA%D0%B0%D0%B7-%D0%BF%D1%80%D0%B5%D0%B7%D0%B8%D0%B4%D0%B5%D0%BD%D1%82%D0%B0-%D1%80%D1%84-%E2%84%96-620-%D0%BE%D1%82-22-12-2017/">уполномоченный в области ГосСОПКА - т.е. ФСБ России</a> (статья 6 часть 4 пункты 5 и 6 187-ФЗ).



Данный ФОИВ возложенную на него задачу выполнил, издав&nbsp;<a href="https://zlonov.ru/kii/%D0%BF%D1%80%D0%B8%D0%BA%D0%B0%D0%B7-%D1%84%D1%81%D0%B1-%D1%80%D0%BE%D1%81%D1%81%D0%B8%D0%B8-%E2%84%96367-%D0%BE%D1%82-24-07-2018/">Приказ ФСБ России №367 от 24.07.2018 «Об утверждении Перечня информации, представляемой в ГосСОПКА и Порядка представления информации в ГосСОПКА»</a>.&nbsp;



В Приложении №1 (<em>Перечень...</em>) к этому приказу в пункте 5 речь идёт как раз про информацию "<em>о компьютерных инцидентах, связанных с функционированием объектов критической информационной инфраструктуры</em>", а в Приложении №2 в пункте 3 в свою очередь с одной стороны действительно написано:



3. <strong>Информация</strong>, указанная в пункте 5 Перечня, <strong>представляется субъектами</strong> критической информационной инфраструктуры <strong>в ГосСОПКА</strong> путем ее направления в НКЦКИ в соответствии с определенными НКЦКИ форматами <strong>с использованием технической инфраструктуры НКЦКИ</strong>, предназначенной для отправки, получения, обработки и хранения и запросов в рамках информационного взаимодействия критической информационной инфраструктуры, а также являющимися субъектами критической информационной уведомлений с субъектами с иными не инфраструктуры органами и организациями, в том числе иностранными и международными (далее - техническая инфраструктура НКЦКИ).



Но в следующем же пункте сразу сделано послабление:



4. <strong>В случае отсутствия подключения к технической инфраструктуре НКЦКИ информация направляется посредством почтовой</strong>, <strong>факсимильной</strong> или <strong>электронной связи</strong> на адреса (телефонные номера) НКЦКИ, указанные <strong>на официальном сайте</strong> в информационно-телекоммуникационной сети «Интернет» по адресу: «<strong>http://cert.gov.ru</strong>».



Таким образом получается, что информировать можно как через техническую инфраструктуру НКЦКИ ("подключение к ГосСОПКА"), так и без неё.



Хорошо - абсолютно всем субъектам КИИ подключаться к ГосСОПКА не надо, с частью 2 статьи 9 разобрались. Теперь можно вернуться к части 3 статьи 9 и статье 10, где речь про субъектов КИИ с значимымим объектами.



Как уже приводилось выше, непосредственно в самом 187-ФЗ есть только требование по непрерывному взаимодействию с ГосСОПКА. Можно только предполагать, что законодатель скрыл за этим требованием. Формально, выделенный человек, отправляющий письма об инцидентах с задержкой не менее, чем в 24 часа, как это установлено в Приказе ФСБ №367, а также регулярно читающий информационные рассылки (или какой там механизм будет предусмотрен для обратной связи от ГосСОПКА?), вполне может считаться вариантом непрерывного взаимодействия. Хотя, конечно, ситуация с ручным выполнением этих операций уже начинает выглядеть несколько надуманной и натянутой.



Ещё более очевидной необходимость использовать именно технические средства становится при изучении приказов ФСТЭК, устанавливающих требования к созданию систем безопасности (<a href="https://zlonov.ru/kii/%D0%BF%D1%80%D0%B8%D0%BA%D0%B0%D0%B7-%D1%84%D1%81%D1%82%D1%8D%D0%BA-%D1%80%D0%BE%D1%81%D1%81%D0%B8%D0%B8-%E2%84%96235-%D0%BE%D1%82-21-12-2017/">Приказ ФСТЭК №235</a>) и требования по обеспечению безопасности (<a href="https://zlonov.ru/kii/%D0%BF%D1%80%D0%B8%D0%BA%D0%B0%D0%B7-%D1%84%D1%81%D1%82%D1%8D%D0%BA-%D1%80%D0%BE%D1%81%D1%81%D0%B8%D0%B8-%E2%84%96239-%D0%BE%D1%82-25-12-2017/">Приказ ФСТЭК №239</a>) значимых объектов КИИ.



Приказ №235 ещё раз фиксирует, что:



6. <strong>Системы безопасности должны обеспечивать</strong>:...<strong>непрерывное взаимодействие с государственной системой обнаружения, предупреждения и ликвидации последствий компьютерных атак на информационные ресурсы Российской Федерации</strong>, которое осуществляется в соответствии со статьей 5 Федерального закона «О безопасности критической информационной инфраструктуры Российской Федерации».



А в Приказе №239 в свою очередь можно найти целый ряд требований, которые логичнее/целесообразнее/удобнее (подберите нужное слово) выполнять именно техническими средствами:


<!-- wp:image {"id":72662,"align":"center"} -->
<div class="wp-block-image"><figure class="aligncenter"><img src="https://i2.wp.com/zlonov.ru/wp-content/uploads/АУД.5.png?fit=1024%2C377&amp;ssl=1" alt="" class="wp-image-72662"/><figcaption>АУД.5</figcaption></figure></div>
<!-- /wp:image -->

<!-- wp:image {"id":72663} -->
<figure class="wp-block-image"><img src="https://i0.wp.com/zlonov.ru/wp-content/uploads/СОВ.1.png?fit=1024%2C248&amp;ssl=1" alt="" class="wp-image-72663"/><figcaption>СОВ.1</figcaption></figure>
<!-- /wp:image -->

<!-- wp:image {"id":72664} -->
<figure class="wp-block-image"><img src="https://i0.wp.com/zlonov.ru/wp-content/uploads/ИНЦ.6.png?fit=1024%2C396&amp;ssl=1" alt="" class="wp-image-72664"/><figcaption>ИНЦ.6</figcaption></figure>
<!-- /wp:image -->


Собственно, вот и вся разгадка про обязательность подключения к ГосСОПКА. Как всё на том же упоминавшемся выше вебинаре ответил мой коллега Константин Саматов, "<strong>грубо говоря</strong>, для объектов первой и второй категории необходимо организовать подключение к техническим средствам ГосСОПКа": <a href="https://youtu.be/thrZPNf5WCI?t=2604">https://youtu.be/thrZPNf5WCI?t=2604</a> (с 43 минуты 24 секунды).


<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->


<strong>Резюме</strong>: В текущих версиях опубликованных нормативно-правовых актов нет однозначного требования об обязательности подключения к ГосСОПКА и использования для взаимодействия с нею каких-либо технических средств. Вместе с тем для эффективной реализации требований по непрерывности взаимодействия для сколько-нибудь крупных объектов КИИ, а особенно для реализации мер из состава набора мер в Приказе ФСТЭК №239 для значимых объектов 1 и 2 категории, на практике использовать технические средства скорее всего всё равно придётся.



Кстати, <a href="https://zlonov.ru/meeting-with-fstec/">на встрече ФСТЭК с блогерами</a> прозвучало, что "<em>у нас в стране всё теперь средства ГоСОПКА</em>" =) Действительно, прочтите ещё раз определение из части 3 статьи 5 187-ФЗ и попробуйте подобрать <a href="https://zlonov.ru/catalog/">какое-либо средство защиты информации</a>, под него не попадающее:



3. <strong>Средствами</strong>, предназначенными для обнаружения, предупреждения и ликвидации последствий компьютерных атак и реагирования на компьютерные инциденты, <strong>являются технические</strong>, <strong>программные</strong>, <strong>программно-аппаратные</strong> и <strong>иные средства</strong> для <strong>обнаружения</strong> (в том числе для поиска признаков компьютерных атак в сетях электросвязи, используемых для организации взаимодействия объектов критической информационной инфраструктуры), <strong>предупреждения</strong>, <strong>ликвидации</strong> последствий компьютерных атак <strong>и (или) обмена информацией</strong>, необходимой субъектам критической информационной инфраструктуры при обнаружении, предупреждении и (или) ликвидации последствий компьютерных атак, <strong>а также криптографические средства защиты такой информации</strong>.

