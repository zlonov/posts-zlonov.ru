---
layout: zlonov/old_post
title: Как распильщики с логикой воюют или Подводный токен
date: 2012-08-10 12:38
author: admin
category: autoimport
tags: [Aladdin, Rutoken, информационная безопасность, мошенничество, сертификация, токен, ШИПКА]
---
Тему откатов и распилов в области информационной безопасности я уже как-то в своём блоге<a href="https://zlonov.ru/2011/12/raspilit-izvolite/"> поднимал</a>, но тема это такая, что сколько её ни поднимай, а новый повод всё равно находится чуть ли ни каждый день.

Вот и сейчас привлёк моё внимание один <a href="http://zakupki.gov.ru/pgz/public/action/orders/info/common_info/show?notificationId=3937254">Открытый аукцион в электронной форме</a> на «<i>Право заключения государственного контракта на поставку USB – ключей для нужд ФМС России</i>». Контракт вполне себе не маленький 3 107 321,20 руб. (к примеру, если <a href="http://base.garant.ru/3921257/">верить данным Росстата о прожиточном минимуме в России</a>, на эти деньги 52 пенсионера могут прожить целый год).

<a name="pdf"></a>Документация к этому аукциону была размещена очень забавно. Если вы скачаете её по <a href="http://zakupki.gov.ru/pgz/documentdownload?documentId=74442405">этой ссылке</a>, то увидите, что выложена была не текстовая версия документа, а его копия в виде графического tif-файла(!). Хитро придумал представитель заказчика г-н П.Б.Жданов и его коллеги – сайт Госзакупки графические файлы ведь не индексирует, а значит "посторонние", не знающие об этом конкурсе от "доверенных лиц", даже расширенным поиском по ключевым словам его не найдут. Для индексации доступен был лишь вот <a href="http://zakupki.gov.ru/pgz/printForm?type=NOTIFICATION&amp;id=3848022">этот малоинформативный документ</a> с самой общей информацией. Так что аукцион разве что по "<i>USB ключ</i>" можно было отыскать. В самой конкурсной документации ключевых слов, естественно, гораздо больше, вот кто-то и придумал "подстраховаться".

Как обычно, самое интересное в документации – это Технические требования к поставляемым ключам. Вот они:

<img class="aligncenter size-full wp-image-2761" src="/assets/uploads/2012/08/23-24.png" alt="23-24" width="1024" height="798" />

Для удобства - <a href="http://ru.scribd.com/doc/136193354/" target="_blank">ссылка на распознанные страницы 23-24 документа</a>.

USB-ключей, а тем более сертифицированных, вообще-то у нас <a href="https://zlonov.ru/2012/02/pass_whist_gost/">и так немного</a>, но в данном случае заказчик пошёл ещё дальше и в явном виде указал вполне себе конкретную модель. Убедиться в этом можно, например, поискав «<i>Микросхема смарт-карты Atmel AT90SC25672RCT-USB (Atmel AT90SC25672R)</i>» в <a href="https://www.google.ru/search?ie=UTF-8&amp;hl=ru&amp;q=%D0%9C%D0%B8%D0%BA%D1%80%D0%BE%D1%81%D1%85%D0%B5%D0%BC%D0%B0%20%D1%81%D0%BC%D0%B0%D1%80%D1%82-%D0%BA%D0%B0%D1%80%D1%82%D1%8B%20Atmel%20AT90SC25672RCT-USB%20(Atmel%20AT90SC25672R)">Google</a> или <a href="http://yandex.ru/yandsearch?text=%D0%9C%D0%B8%D0%BA%D1%80%D0%BE%D1%81%D1%85%D0%B5%D0%BC%D0%B0+%D1%81%D0%BC%D0%B0%D1%80%D1%82-%D0%BA%D0%B0%D1%80%D1%82%D1%8B+Atmel+AT90SC25672RCT-USB+(Atmel+AT90SC25672R)&amp;lr=213">Яндексе</a>.

Вообще, конечно, надо отдать должное тому, кто готовил аукцион – всё же текст в технических требованиях не на 100% соответствует описанию на сайте поставщика, но факт ограничения конкуренции тем не менее очевиден. Очевиден настолько, что кто-то (предполагаю, что один из конкурентов) обратился в ФМС России с просьбой дать разъяснения. Полный список вопросов и те ответы, которые дал на них представитель заказчика С.И. Голиков приведены <a href="http://zakupki.gov.ru/pgz/documentdownload?documentId=76429197">здесь</a>. Вот краткая суть с моими комментариями:
<ul>
	<li>Вопрос 1.Для чего будут использоваться ключи и какая ОС используется?
<ul>
	<li>Ответ. Для использования ЭЦП в информационной системе ФМС, ОС Win 7 x32.</li>
	<li><i>Но на всякий случай впишем и </i><i>MacOs и </i><i>Linux</i></li>
</ul>
</li>
	<li>Вопрос 2. Возможна ли поставка ключей, не построенных на базе Atmel AT905C25672RCT-USB (Atmel AT90SC25672R) и если нет, то почему?
<ul>
	<li>Без конкретного ответа, но внесены изменения в Технические требования.</li>
	<li><i>Да, слишком уж нагло прописали, не думали, видимо, что отсканированную документацию кто-то отыщет…</i></li>
</ul>
</li>
	<li>Вопрос 3. Почему прописаны требования к наличию западных стандартов шифрования RSA 1024 / 2048, DES, 3DES, SHA-1?
<ul>
	<li>Ответ. Планируется использовать USB-ключи в том числе и для аутентификации в домене Windows с использованием технологии Smart Card Logon.</li>
	<li><i>В домен вообще-то можно и по ГОСТовым сертификатам входить – у КриптоПро даже <a href="http://www.cryptopro.ru/products/other/winlogon">решение отдельное для этого есть</a>.</i></li>
</ul>
</li>
	<li>Вопрос 4. Для чего в требования к сертификации указано дополнительное условие о наличии ОУД2?
<ul>
	<li>Без конкретного ответа, но внесены изменения в Технические требования.</li>
	<li><i>"Ладно-ладно, уберём – у нас и другие ограничения конкурентов прописаны".</i></li>
</ul>
</li>
	<li>Вопрос 5. Совместимость с какими конкретно средствами криптографической защиты информации требуется?
<ul>
	<li>Ответ. Требуются сертификаты совместимости USB-ключа с СКЗИ "КриптоПро CSP"</li>
	<li><i>Какую юридическую силу имеют эти «сертификаты совместимости» - не очень понятно, но штука вроде модная, все их получают.</i></li>
</ul>
</li>
	<li>Вопрос 6. Для чего требуется водонепроницаемость корпуса (стандарту IP Х8 - IEC 529 - Защита от воды при неограниченном времени погружения на определённую глубину). «<i><b>ФМС России планирует использование USB-ключей в подводной среде?</b></i>» =) (смайлик мой, цитата дословная)
<ul>
	<li>Без конкретного ответа, но внесены изменения в Технические требования.</li>
	<li><i>Может известному аквалангисту Макаревичу один ключ хотели подарить? =)</i></li>
</ul>
</li>
	<li>Вопросы 7-8. Технические требования сокращают список возможных производителей до одного производителя. Вы сознательно нарушаете ст. 41.6, п. 1, Главы 3.1 и ст. 34, п. 3 и 3.1, Главы 3 Федерального закона №94-ФЗ? Допустима ли поставка других ключей с аналогичными по своей функциональности характеристиками?
<ul>
	<li>Ответ. По имеющейся у ФМС России информации, закупаемый товар, соответствующий характеристикам, установленным в документации об открытом аукционе в электронной форме производят целый ряд производителей.</li>
	<li><i>Весь рынок не в курсе, а ФМС знает целый ряд таких производителей, надо же…</i></li>
</ul>
</li>
</ul>
<a href="http://zakupki.gov.ru/pgz/documentdownload?documentId=76430356">Обновлённая версия</a> технических требований стала выглядеть вот так:
<div><img class="aligncenter size-full wp-image-2762" src="/assets/uploads/2012/08/Обновлённые-требования.png" alt="Обновлённые требования" width="597" height="633" /></div>
Справедливость восторжествовала? Нет, конечно! Ведь будущий откат, наверняка, оговорён и попилен, или наоборот "серьёзным" людям "правильные" конверты ещё раньше занесли – не знаю, как там точно у них всё делается.

Посмотрите, как ловко играют мошенники. Вроде бы убрали и микросхему Atmel AT905C25672RCT-USB (Atmel AT90SC25672R), и "подводный" стандарт IP Х8 - IEC 529 и объективно не нужный уровень доверия ОУД 2, но вписали "<i>реализацию виртуальной машина Java (полностью совместимая со стандартом Sun Java Card)</i>". В общем, конкуренция всё также осталась ограниченной, какой бы там мифический ряд производителей ни был ФМС известен.

Наш неизвестный борец за справедливость повторно обратился к ФМС за разъяснениями. Вопросы с ответами второго разъяснения <a href="http://zakupki.gov.ru/pgz/documentdownload?documentId=76703799">полностью тут</a>, а кратко с комментариями так:
<ul>
	<li>Вопрос 1. На российском рынке средств электронной подписи операционная система смарт-карты, включающая реализацию виртуальной машина Java (полностью совместимой со стандартом Sun Java Card), есть только в USB-ключах одного производителя. Просим разъяснить реальную и обоснованную необходимость в наличии указанного требования.
<ul>
	<li>Ответ. Государственная информационная система миграционного учёта (далее ГИСМУ), оператором которой является ФМС России, в качестве своей основной технологии реализации прикладной функциональности отдельных информационных систем входящих в состав ГИСМУ применяет технологию Java. В связи с этим, для целей реализации расширенной прикладной функциональности по обеспечению информационной безопасности информации, собираемой и обрабатываемой в ГИСМУ, нами было принято решение задействовать расширенные возможности современных электронных ключей для достижения указанных целей на основе применения в качестве программного компонента ряда информационных систем, входящих в состав ГИСМУ, апплетов, загружаемых и исполняющихся на электронных ключах.</li>
	<li><i>Ответ ФМС я привёл полностью из "любви к искусству": так и представляю себе чиновника, пишущего этот ответ про технологию </i><i>Java, - долго, наверное, формулировки подбирал =) А по сути-то написан бред: </i><i>Java в прикладной информационной системе и </i><i>Java-апплеты в памяти ключа - это персонажи совсем из разных опер. А уж как там и что они в сертифицированный ключ собрались загружать – это я бы с удовольствием посмотрел. Крутые спецы в ФМС работают, ничего не скажешь .</i></li>
</ul>
</li>
</ul>
<ul>
	<li>Вопрос 2. Какой объем СВОБОДНОЙ (т.е. доступной для пользователя) памяти USB-ключа необходим?
<ul>
	<li>Ответ. Не менее 64 КБ и не более 72 КБ.</li>
	<li><i>Ага, и ни килобайтом больше!</i></li>
</ul>
</li>
</ul>
<ul>
	<li>Вопрос 3. Допускается ли использование носителей, поддерживающих технологию Smart Card Logon и алгоритмы RSA, DES (3DES), RC2, RC4, MD4, MD5, SHA-1?
<ul>
	<li>Ответ. Допускается при выполнении всех требований документации.</li>
	<li><i>Отличный ответ: ненужные на самом деле требования можно не выполнять, если они выполнены.</i></li>
</ul>
</li>
</ul>
<ul>
	<li>Вопрос 4. USB-ключи закупаются для ЭЦП, для чего необходимо использование интерфейсов SSL v3 и IPSec/IKE?
<ul>
	<li>Ответ. Доступ уполномоченных лиц в ФГИС ФМС России осуществляется, в том числе, посредством защищенного удаленного доступа с использованием протоколов SSL и IPSec/IKE, при этом аутентификация пользователей осуществляется посредством сертификатов ЭП.</li>
	<li><i>Не видел, конечно, я их систему, но как-то сомнительно.</i></li>
</ul>
</li>
</ul>
<ul>
	<li>Вопрос 5. Требование наличия Microsoft CCID подразумевает использование USB-ключей без какого-либо дополнительного ПО, однако, по условиям сертификации ФСТЭК программно-аппаратного комплекса (ПАК) установка дополнительного ПО необходима. Возможна ли поставка решения, в соответствии с сертификацией которого, все необходимые для работы драйвера входят в состав сертифицированного программно-аппаратного комплекса?
<ul>
	<li>Комплектность поставляемого оборудования должна соответствовать требованиям, изложенным в формуляре на сертифицированное изделие. Требования по сертификации установлены в документации об открытом аукционе в электронной форме.</li>
	<li><i>Отписка, а не ответ по сути.</i></li>
</ul>
</li>
</ul>
Второе разъяснение было дано 01 августа и по его итогам изменения в Технические требования уже не вносились. С этой даты новых обновлений на сайте пока больше нет. Сам аукцион состоится 23.08.2012 в 11:30 – посмотрим, чем закончится эта история…

[box type="info" style="rounded"]UPD. 23.08.2012 Чуда не произошло: <a href="/2012/08/logic_kickback_0-1/">Логика - Пила, счёт 0:1</a>.[/box]
<p style="text-align: right;"><i>Изображение: http://byaki.net/kartinki/7520-podvodnyjj_mir.html</i>