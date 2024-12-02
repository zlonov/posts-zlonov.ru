---
layout: zlonov/old_post
title: 'Виды электронных подписей в России и требования к Средствам ЭП'
date: 2016-11-02
featured-image: /2016/подпись.jpg
excerpt: При копировании файлов (особенно файлов больших размеров) с компьютеров Mac на внешние или сетевые диски с другой, чем в Mac файловой системой, могут возникать ошибки
comments: true
tags: ['63-ФЗ', 'законодательство', 'приказ 796', 'требования', 'ФСБ России', 'ФСТЭК России', 'электронная подпись', 'ЭП']
category: security
AllowComments: true
LinkedLinks: ""
---

Принятый ещё в апреле 2011 года Федеральный закон N 63-ФЗ "<a href="http://base.garant.ru/12184522/">Об электронной подписи</a>" определил следующие два вида электронной подписи (ЭП): простая ЭП и усиленная ЭП, из которых вторая в свою очередь бывает неквалифицированной и квалифицированной.

Простая ЭП, по большому счёту, даже и не совсем электронная подпись в классическом математическом понимании - в качестве простой ЭП можно использовать хоть одноразовые коды, хоть и вовсе пароли:

> Простой электронной подписью является электронная подпись, которая посредством использования кодов, паролей или иных средств подтверждает факт формирования электронной подписи определенным лицом.

Усиленная же электронная подпись обязательно использует криптографические преобразования. Вот требования для усиленной неквалифицированной ЭП (или просто неквалифицированной ЭП):

>1) получена в результате криптографического преобразования информации с использованием ключа электронной подписи;\
2) позволяет определить лицо, подписавшее электронный документ;\
3) позволяет обнаружить факт внесения изменений в электронный документ после момента его подписания;\
4) создается с использованием средств электронной подписи.

Как видно, усиленная ЭП в отличие от простой ЭП должна позволять обнаруживать изменения в электронном документе (понятно, что с помощью пароля такое не реализовать), а формировать её нужно с использованием Средств ЭП:

> средства электронной подписи - шифровальные (криптографические) средства, используемые для реализации хотя бы одной из следующих функций - создание электронной подписи, проверка электронной подписи, создание ключа электронной подписи и ключа проверки электронной подписи;

Понятие _Средство электронной подписи_ - очень важное и к нему мы ниже ещё вернёмся. Пока же продолжим разбираться с видами электронных подписей. Осталось рассмотреть квалифицированную усиленную подпись - от неквалифицированной усиленной она отличается двумя принципиальными дополнительными требованиями:

>1) ключ проверки электронной подписи указан **в квалифицированном сертификате**;\
2) для создания и проверки электронной подписи используются средства электронной подписи, **имеющие подтверждение соответствия требованиям, установленным в соответствии с настоящим Федеральным законом**.

Другими словами для квалифицированной ЭП, абы какой сертификат не годится - нужен именно квалифицированный:

> квалифицированный сертификат - сертификат ключа проверки электронной подписи, **соответствующий требованиям, установленным настоящим Федеральным законом** и иными принимаемыми в соответствии с ним нормативными правовыми актами, и **созданный аккредитованным удостоверяющим центром либо федеральным органом исполнительной власти, уполномоченным в сфере использования электронной подписи**;

Далее по тексту закона приведён исчерпывающий перечень сведений, которые должен содержать квалифицированный сертификат и указано, что создаётся он только с использованием средств аккредитованного удостоверяющего центра.

Используемое для создания и проверки квалифицированной электронной подписи _Средство ЭП_ тоже подойдёт не любое, а только то, которое имеет подтверждение соответствия установленным требованиям.

Понятия _"ключ проверки электронной подписи"_,  _"сертификат"_, _"удостоверяющий центр"_ и т.п. в этом посте отдельно рассматривать не буду (можно посмотреть начало вот этого поста, например:<a href="https://zlonov.ru/2013/12/private-keys-keepers-evolution/"> https://zlonov.ru/2013/12/private-keys-keepers-evolution/</a>), если это необходимо - напишите в комментариях, раскрою всю терминологию отдельно.

Вот такая получается таблица, кратко поясняющая основные различия между видами электронных подписей в соответствии с 63-ФЗ:

{% include one_image_new2.html picture_name="Виды электронных подписей (ЭП) и их особенности" picture_path="2016/Виды-ЭП-и-их-особенности.jpg" %}

Теперь вернёмся к понятию _Средство ЭП_. Из приведённого выше определения следует, что _Средства ЭП_ - это определённый вид шифровальных (криптографических) средств, которые используются для какой-либо одной или любой комбинации из функций:

 - создание электронной подписи,
 - проверка электронной подписи,
 - создание ключа электронной подписи и ключа проверки электронной подписи.

Замечу на полях, что создание ключа ЭП и ключа проверки ЭП возможно лишь в паре (те самые открытый и закрытый ключи в [асимметричной криптографии](https://ru.wikipedia.org/wiki/Криптосистема_с_открытым_ключом)).

Сами же шифровальные средства определены в Постановлении Правительства РФ от 16 апреля 2012 г. N 313 "[Об утверждении Положения о лицензировании деятельности...](http://base.garant.ru/70164728/)", вот выдержка из определения:

> К шифровальным (криптографическим) средствам (средствам криптографической защиты информации), включая документацию на эти средства, относятся:\
...\
в) средства электронной подписи;

По мне, так имеем рекурсивное зацикленное определение понятия через само себя =) Ну, да не будем казуистам. По сути, под понятие _средство ЭП_ попадают в том числе чисто программные, программно-технические средства и даже целые комплексы и системы.

Вернёмся к 63-ФЗ и посмотрим, какие требования есть для Средств ЭП. Вот что они должны делать:

> 1) позволяют установить факт изменения подписанного электронного документа после момента его подписания;\
2) обеспечивают практическую невозможность вычисления ключа электронной подписи из электронной подписи или из ключа ее проверки.

Про факт отслеживания изменений уже было выше в требованиях к усиленной ЭП, ну, а практическая невозможность вычисления ключа ЭП из ЭП или из ключа проверки ЭП - это понятное и разумное требование (закрытый ключ не должен вычисляться из открытого или из самой электронной подписи).

Продолжим.

Для случаев подписи документов, содержащих гостайну, или при работе Средства ЭП в системах, содержащих гостайну, требуется подтверждение соответствия обязательным требованиям по защите сведений соответствующей степени секретности. Вполне логично, так как Гостайна у нас регулируется отдельно и требования там тоже свои отдельные.

Есть ещё важная оговорка про подпись документов, содержащих информацию ограниченного доступа (в том числе персональные данные): Средства ЭП не должны нарушать конфиденциальность такой информации. Насколько я понимаю, тут идёт речь про то, что для такой информации нельзя, например, использовать облачные незащищённые в соответствии с требованиями законодательства сервисы электронной подписи.

Если средство электронной подписи используется для автоматического создания и (или) автоматической проверки электронных подписей в информационной системе, то на этом требования к нему заканчиваются. Автоматическое создание, например, может применяться при оказании государственных услуг. Тогда в сертификате вовсе может быть не указано конкретное физическое лицо, а создание ЭП осуществляется, скажем, системой принятия отчётности (для подтверждения того факта, что отчётность была получена в срок, например).

В случаях же неавтоматического создания и проверки электронной подписи к Средствами ЭП предъявляются дополнительные требования.

При создании электронной подписи Средства ЭП должны:

>1) показывать самостоятельно или с использованием программных, программно-аппаратных и технических средств, необходимых для отображения информации, подписываемой с использованием указанных средств, лицу, осуществляющему создание электронной подписи, содержание информации, подписание которой производится;\
2) создавать электронную подпись только после подтверждения лицом, подписывающим электронный документ, операции по созданию электронной подписи;\
3) однозначно показывать, что электронная подпись создана.

Первое требование означает, что сам по себе, например, токен не может быть Средством ЭП - требуется некая _обвязка_ вокруг него, которая будет показывать подписываемый документ. Второе требование запрещает создание подписи без подтверждения человеком. Наконец, третье требование указывает, что нужно недвусмысленно дать понять, что подпись была создана.

При проверке электронной подписи Средство ЭП должно:

>1) показывать самостоятельно или с использованием программных, программно-аппаратных и технических средств, необходимых для отображения информации, подписанной с использованием указанных средств, содержание электронного документа, подписанного электронной подписью;\
2) показывать информацию о внесении изменений в подписанный электронной подписью электронный документ;\
3) указывать на лицо, с использованием ключа электронной подписи которого подписаны электронные документы.

Должно быть чётко видно и понятно - что подписано, были ли внесены изменения и кто подписывал.

Таковы, вкратце, основные требования к Средствам ЭП в 63-ФЗ. Однако, в нём также содержится статья про полномочия федеральных органов исполнительной власти в сфере использования электронной подписи, где указано:

>Федеральный орган исполнительной власти в области обеспечения безопасности:\
1) устанавливает требования к форме квалифицированного сертификата;\
2) устанавливает **требования к средствам электронной подписи** и средствам удостоверяющего центра;\
3) **осуществляет подтверждение соответствия средств электронной подписи** и средств удостоверяющего центра **требованиям, установленным в соответствии с настоящим Федеральным законом**, и публикует перечень таких средств;\
4) по согласованию с уполномоченным федеральным органом устанавливает дополнительные требования к порядку реализации функций аккредитованного удостоверяющего центра и исполнения его обязанностей, а также к обеспечению информационной безопасности аккредитованного удостоверяющего центра.

Таким органом является ФСБ РФ, которая 27 декабря 2011 г. издала приказ № 796 "[Об утверждении Требований к средствам электронной подписи и Требований к средствам удостоверяющего центра](http://www.garant.ru/products/ipo/prime/doc/70039150/)".

Прежде всего данный приказ ФСБ устанавливает требования в части разработки, производства, реализации и эксплуатации Средств ЭП:

> предъявляются требования, закрепленные Положением о разработке, производстве, реализации и эксплуатации шифровальных (криптографических) средств защиты информации (Положение ПКЗ-2005), утвержденным приказом ФСБ России от 9 февраля 2005 г. N 66 (с изменениями, внесенными приказом ФСБ России от 12 апреля 2010 г. N 173 для шифровальных (криптографических) средств защиты информации с ограниченным доступом, не содержащей сведений, составляющих государственную тайну.

ПКЗ-2005 - основополагающий регламент для всех разработчиков криптографических средств, что и не удивительно, раз Средства ЭП - это, в первую очередь, средство шифрования. К слову, в ПКЗ-2005 есть вот такое определение для средств электронной цифровой подписи:

>средства электронной цифровой подписи - аппаратные, программные и аппаратно-программные средства, обеспечивающие на основе криптографических преобразований реализацию хотя бы одной из следующих функций:
>- создание электронной цифровой подписи с использованием закрытого ключа электронной цифровой подписи,
>- подтверждение с использованием открытого ключа электронной цифровой подписи подлинности электронной цифровой подписи,
>- создание закрытых и открытых ключей электронной цифровой подписи.

Да, речь здесь про Средства ЭЦП, а не ЭП, но мы же уже решили не быть казуистами =)

Вернёмся к требованиям к Средствам ЭП, которым в приказе ФСБ посвящен весь раздел II (статьи с 8 по 39). Статьи 8-10 дублируют то, что есть в 63-ФЗ в части требований при создании и проверке ЭП при неавтоматической работе, за исключением того, что согласно требованиям ФСБ Средство ЭП должно данные требования выполнять самостоятельно, а не "_с использованием программных, программно-аппаратных и технических средств, необходимых для отображения информации_" .

Статья 11 определяет, что :

>Статья 11. Средства ЭП должны противостоять угрозам, представляющим собой целенаправленные действия с использованием аппаратных и (или) программных средств с целью нарушения безопасности защищаемой средством ЭП информации или с целью создания условий для этого (далее - атака).

В последующих статьях 12-18 определяются классы Средств ЭП КС1, КС2, КС3, КВ2, КА1 в зависимости от их способности противостоять таким атакам.

В дальнейших статьях 19-39 сформулированы ещё более детальные требования к составу Средств ЭП для разных классов и к особенностям их работы, из которых особо выделю статьи 20, 22 и 38:

>Статья 20. При разработке средств ЭП должны использоваться криптографические алгоритмы, утвержденные в качестве государственных стандартов или имеющие положительное заключение ФСБ России по результатам их экспертных криптографических исследований

>Статья 22. В средстве ЭП должны быть реализованы только заданные в ТЗ на разработку (модернизацию) средства ЭП алгоритмы функционирования средства ЭП.

>Статья 38. Криптографические протоколы, обеспечивающие операции с ключевой информацией средства ЭП, должны быть реализованы непосредственно в средстве ЭП.

Смысл тут, упрощённо, в том, что в Средстве ЭП можно использовать только криптографические ГОСТ алгоритмы, при этом они должны быть реализованы в нём самом (нельзя использовать, например, какие-то внешние средства) и никакие другие криптографические алгоритмы и протоколы в Средстве ЭП не должны быть реализованы.

Итоговая таблица с основными требованиями к Средствам ЭП в 63-ФЗ и приказе ФСБ №796 выглядит так:

{% include one_image_new2.html picture_name="Основные требования к Средствам ЭП" picture_path="2016/Основные-требования-к-Средствам-ЭП.jpg" %}

Таким образом, для использования простой ЭП можно использовать любые средства, для усиленной неквалифицированной ЭП (или просто неквалифицированной ЭП) - только Средства ЭП, базовые требования к которым определены в 63-ФЗ, и, наконец для усиленной квалифицированной ЭП (или просто квалифицированной ЭП) - только Средства ЭП, имеющие подтверждение соответствия требованиям, установленным в соответствии с Федеральным законом 63-ФЗ и Приказом ФСБ №796. Подтверждением такого соответствия является сертификат соответствия, выданный ФСБ России, в котором такое соответствие упоминается в явном виде.

В [перечне средств защиты информации, сертифицированных ФСБ России](http://clsz.fsb.ru/certification.htm) (по состоянию на 1 октября 2016 года) значится немногим меньше 100 таких сертификатов - есть из чего выбрать =)
