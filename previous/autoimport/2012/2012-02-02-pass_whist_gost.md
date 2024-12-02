---
layout: zlonov/old_post
title: Пас, вист, ГОСТ!
date: 2012-02-02 15:55
author: admin
category: autoimport
tags: [Aladdin, iBank 2 Key, Rutoken, USB, информационная безопасность, криптография, токен, ШИПКА, ЭЦП]
---
Вот этот уже прошлогодний <a href="http://shaurojen.blogspot.com/2011/07/blog-post.html">пост</a> Евгения Шауро со сравнением различных токенов напомнил мне, что давно хотел более пристально приглядеться к современным ГОСТовым токенам. Хорошо помню, что в своё время эта тема была очень модной и неизменно вызывала интерес у самой разной аудитории.

Небольшое отступление для тех, кто не очень знаком с предметом. USB-токен (он же просто токен, он же электронный ключ, он же брелок, он же USB-ключ) - это устройство, объединяющее в себе USB-контроллер и чип смарт-карты (микроконтроллер). Вся прелесть токена на основе смарт-карты заключается в том, что он целый ряд криптографических вычислений производит, что называется, "на борту". Данный функционал используется для надёжной аутентификации пользователей в самых различных системах (подробнее можно почитать, например, <a href="https://zlonov.ru/%D1%81%D1%82%D0%B0%D1%82%D1%8C%D0%B8/%D1%81%D0%BE%D0%B2%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D1%8B%D0%B5-%D0%BC%D0%B5%D1%82%D0%BE%D0%B4%D1%8B-%D0%B0%D1%83%D1%82%D0%B5%D0%BD%D1%82%D0%B8%D1%84%D0%B8%D0%BA%D0%B0%D1%86%D0%B8%D0%B8-%D1%82/">здесь</a>) и особенно важен при использовании ЭЦП (электронной цифровой подписи), так как позволяет генерировать и использовать закрытые ключи, которые никогда не покидают защищённую память устройства. Данные, которые необходимо подписать, просто передаются внутрь токена, а тот сообщает лишь конечный результат, т.е. значение ЭЦП. Таким образом, закрытый ключ, используемый, например, для того же дистанционного банковского обслуживания, гарантировано не попадёт к злоумышленникам.

До недавнего времени все предлагаемые на российском рынке токены могли работать только с западными стандартами ЭЦП, а поддержка российской ГОСТовой криптографии сводилась к хранению контейнера с закрытым ключом в памяти устройства, защищённой PIN-кодом. При этом для выполнения операций с закрытым ключом контейнер копировался в память компьютера со всеми вытекающими из этого опасностями его утечки.

Первые токены с поддержкой ГОСТ работали только с ГОСТ 28147-89, т.е. могли шифровать данные симметричным алгоритмом, но ЭЦП (ГОСТ Р 34.10-2001 или ГОСТ Р 34.10-94) не поддерживали.

Именно такой токен в далёком 2001 году разработали <a href="https://zlonov.ru/2010/11/tolko-faktyi-i-odin-sluh/">ЗАО "Аладдин Р.Д."</a> и НТЦ "Атлас". Называлось изделие <a href="http://npo123.ru/shop/575927/575928/867921/868709.html">eToken RIC</a> (Russian Intellectual Card), но, насколько мне известно, продажи его как-то не заладились и после 2003 года об устройстве <a href="http://www.aladdin-rd.ru/search/?q=etoken+ric">ничего и слышно даже не было</a>.

<a href="/assets/uploads/eToken-RIC.jpg"><img class="aligncenter size-full wp-image-4247" src="https://i0.wp.com/zlonov.ru/wp-content/uploads/2010/11/ie_savesitenotification.png?fit=800%2C600&#038;ssl=1" alt="eToken-RIC" width="800" height="600" /></a>

<div>У извечного конкурента ЗАО "Аладдин Р.Д." - компании ЗАО "Актив-софт" (при партнёрстве с ООО "Анкад") - устройство, представленное <a href="http://business.compulenta.ru/23633/">примерно в то же время</a>, получилось более удачным: <a href="http://www.rutoken.ru/products/rutoken/">Rutoken</a> продаётся и по сей день.</div>

<div><a href="/assets/uploads/rutoken.jpg"><img class="aligncenter size-full wp-image-4249" src="https://i2.wp.com/zlonov.ru/wp-content/uploads/2010/11/ie_savesitenotification.png?fit=800%2C600&#038;ssl=1" alt="rutoken" width="800" height="600" /></a></div>

<div></div>

<div>Первым токеном с поддержкой российского алгоритма ЭЦП стала <a href="http://www.shipka.ru/common.txt">ШИПКА-1.5</a> от ЗАО "ОКБ САПР". Самое раннее упоминание ШИПКИ <a href="http://okbsapr.ru/news.html?year=&amp;month=&amp;p=9">датируется сентябрём 2005 года</a>. Этот год, наверное, и можно считать датой рождения нового устройства.</div>

<div><a href="/assets/uploads/listovka-shipka.gif"><img class="aligncenter size-full wp-image-4250" src="/assets/uploads/listovka-shipka.gif" alt="listovka-shipka" width="150" height="113" /></a></div>

<div></div>

В последующие несколько лет ШИПКА оставалась единственным предложением на этом рынке, но никакого взрывного роста продаж, насколько можно судить об этом по отсутствию публикаций историй внедрения, не произошло: то ли отсутствие сертификации в ФСБ помешало, то ли что-то иное. Домысливать не буду, а то некоторые обижаются и вместо конструктива на личности переходят =)

Ситуация изменилась в 2008 году (<a href="http://www.banki.ru/news/lenta/?id=646428">более ранних упоминаний</a> не обнаружил) с выпуском ООО "БИФИТ" ключа <a href="http://www.bifit.com/ru/company/press/usb-token.html">iBank 2 Key</a>. По сообщениям в пресс-релизах данное устройство имело сертификат ФСБ, что положительно отличало его от остальных конкурентов. На самом деле, ситуация с сертификацией тут не однозначна, т.к. текущий сертификат (подробнее о сертификатах ниже) датируется только 08 июля 2010 года.

<a href="/assets/uploads/iBank2Key.jpg"><img class="aligncenter size-full wp-image-4251" src="/assets/uploads/iBank2Key.jpg" alt="iBank2Key" width="250" height="100" /></a>

<div></div>

<div>Появление нового игрока явно подстегнуло других участников и конкуренты БИФИТа начали/усилили активную рекламную компанию своих аналогичных разработок: eToken ГОСТ у ЗАО "Аладдин Р.Д." и Rutoken ЭЦП у ЗАО "Актив-софт". Примечательно, что оба продукта получили сертификаты ФСБ хоть и несколько лет спустя, но в один и тот же день - 11 мая 2011 г.</div>

<div><a href="/assets/uploads/rutoken-dsa.png"><img class="aligncenter wp-image-4248" src="/assets/uploads/rutoken-dsa.png" alt="rutoken-dsa" width="183" height="132" /></a><a href="/assets/uploads/eToken_GOST_USB_Smart_Card.jpg"><img class="aligncenter size-full wp-image-4252" src="/assets/uploads/eToken_GOST_USB_Smart_Card.jpg" alt="eToken_GOST_USB_Smart_Card" width="150" height="120" /></a></div>

<div>Таким образом, сегодня на рынке доступны четыре различных сертифицированных ФСБ токена с поддержкой российских криптографических алгоритмов, используемых для ЭЦП.</div>

<div>
<table>
<tbody>
<tr>
<td>
<p style="text-align: center;"><b>eToken ГОСТ</b>
<p style="text-align: center;"><a href="/assets/uploads/eToken_.png"><img class="aligncenter size-medium wp-image-4253" src="/assets/uploads/eToken_-214x300.png" alt="_eToken_" width="214" height="300" /></a>
</td>
<td style="text-align: center;"><b>iBank 2 Key </b>

<a href="/assets/uploads/iBank2Key1.jpg"><img class="aligncenter size-medium wp-image-4254" src="/assets/uploads/iBank2Key1-210x300.jpg" alt="_iBank2Key" width="210" height="300" /></a></td>
</tr>
<tr>
<td style="text-align: center;"><b>Rutoken ЭЦП </b>

<a href="/assets/uploads/Rutoken.png"><img class="aligncenter size-medium wp-image-4255" src="/assets/uploads/Rutoken-249x300.png" alt="_Rutoken" width="249" height="300" /></a></td>
<td>
<p style="text-align: center;"><b>ШИПКА-1.6</b>
<a href="/assets/uploads/1.6.jpg"><img class="aligncenter size-medium wp-image-4256" src="/assets/uploads/1.6-213x300.jpg" alt="_1.6" width="213" height="300" /></a></td>
</tr>
</tbody>
</table>
</div>

Беглый взгляд показывает, что сертификат сертификату рознь. Так, например, изделия ШИПКА и Rutoken сертифицированы целиком как СКЗИ и имеют самые широкие (по сравнению с остальными) разрешённые области применения, а вот в случае с eToken сертификат выдан на некий "Криптотокен", входящий в состав изделия. Если я правильно помню архитектуру, то этот "Криптотокен" - суть java-апплет, выполняемый на встроенной в eToken виртуальной Java-машине. При этом, в отличие от ШИПКи и Rutoken, для eToken в сертификате не прописан следующий функционал: управление ключевой информацией, шифрование данных, вычисление имитовставки для данных, содержащихся в областях оперативной памяти СКЗИ.

Ситуация с iBank 2 Key самая запутанная, т.к. сертифицировано<i> программное средство криптографической защиты "Криптомодуль С23", предназначенное для встраивания в операционные системы интеллектуальных карт, построенных на базе микроконтроллеров семейств ST23</i>. Область же применения вообще прописана так:<i> может использоваться в качестве криптографического ядра для реализации функций формирования и проверки электронной цифровой подписи, шифрования информации, не содержащей сведений, составляющих государственную тайну, при создании функционально законченных СКЗИ класса КС2</i>. Кстати, у всех остальных тоже класс КС2, кроме ШИПКи - у неё КС3.

В общем, не всё так просто и очевидно, как это пишут в маркетинговых материалах. Для более детального анализа, понятно, нужно изучать технические условия, формуляры и прочую сопроводительную документацию, да вот только редко производители это всё просто так выдают, хотя я бы, например, с удовольствием потратил немного личного времени на их изучение.

Выкладываю сводную таблицу с данными о токенах (пока только в части, касающейся сертификатов). Если тема окажется интересной, таблицу можно будет дополнить.

<a style="-x-system-font: none; display: block; font-family: Helvetica,Arial,Sans-serif; font-size-adjust: none; font-size: 14px; font-stretch: normal; font-style: normal; font-variant: normal; font-weight: normal; line-height: normal; margin: 12px auto 6px auto; text-decoration: underline;" title="View Токены с поддержкой ЭЦП по ГОСТ on Scribd" href="http://www.scribd.com/doc/109163358/%D0%A2%D0%BE%D0%BA%D0%B5%D0%BD%D1%8B-%D1%81-%D0%BF%D0%BE%D0%B4%D0%B4%D0%B5%D1%80%D0%B6%D0%BA%D0%BE%D0%B9-%D0%AD%D0%A6%D0%9F-%D0%BF%D0%BE-%D0%93%D0%9E%D0%A1%D0%A2">Токены с поддержкой ЭЦП по ГОСТ</a>

<iframe id="doc_12329" src="https://www.scribd.com/embeds/109163358/content?start_page=1&amp;view_mode=slideshow&amp;access_key=key-19fo474jhf68qm4xqxye" width="650" height="450" frameborder="0" scrolling="no" data-aspect-ratio="1.41666666666667" data-auto-height="false"></iframe>

<div style="text-align: right;"><i><span style="font-size: x-small;">Изображение: http://sladsloboda.ru/production/sweet/classical</span></i></div>
