---
layout: zlonov/old_post
title: (Российские криптошлюзы)++
date: 2013-11-04 21:39
author: admin
category: autoimport
tags: [Stonesoft, информационная безопасность, криптография, криптошлюз, межсетевой экран, сертификация, ФСБ]
---
Про сертифицированные ФСТЭК межсетевые экраны (МЭ) <a href="https://zlonov.ru/tag/межсетевой-экран/" target="_blank">писал уже много раз</a> (полный список обзоров <a href="https://zlonov.ru/certified_firewalls/" target="_blank">доступен на отдельной странице</a>). Теперь же <a href="http://stonesoft-rus.blogspot.ru/2013/11/stonegate-firewallvpn.html" target="_blank">появился повод</a> взглянуть на этот класс решений под немного иным углом - с точки зрения применения в них криптографии.

Традиция добавлять к межсетевому экрану (FW) функциональность VPN-сервера зародилась довольно давно и является настолько удачной и логичной (некоторые так и пишут - FW/VPN), что найти периметровый (шлюзовой) межсетевой экран (особенно в аппаратном исполнении) без поддержки VPN не так и просто. Возможно, что они есть, но мне такие что-то сходу не припоминаются. Поправьте в комментариях, если ошибаюсь.

Естественно, что при построении VPN (виртуальных частных сетей) хочется получить канал действительно надёжно защищённый, что предполагает использование сильной криптографии (high encryption). А в России, как известно, область сильной криптографии не менее сильно регулируется, ведь VPN-сервер по сути своей является ни чем иным, как криптошлюзом.

Можно утверждать, что сертифицированный в соответствии с российским законодательством VPN-сервер обязательно должен иметь поддержку алгоритма ГОСТ и сертификат ФСБ, коль скоро именно данное ведомство курирует у нас вопросы шифрования.

Даже при сертификации во ФСТЭК в качестве межсетевого экрана в продуктах класса FW/VPN рекомендуется отключать сильную криптографию, оставляя только алгоритм DES с длиной ключа 56 бит. Другое дело, что не все это делают, а если и делают, то, как вариант, могут продать (подарить) ключ активации сильной криптографии, отправив его просто по электронной почте. Впрочем, сейчас не об этом.

Сертификация в ФСБ имеет, конечно, что-то схожее с аналогичной процедурой во ФСТЭК, но она точно гораздо сложнее - косвенно это можно оценить, например, по тому факту, что в <a href="http://fstec.ru/sistema-sertifikatsii-tzi/153-deyatelnost/tekushchaya/tekhnicheskaya-zashchita-informatsii/sistema-sertifikatsii/591-gosudarstvennyj-reestr-sertifitsirovannykh-sredstv-zashchity-informatsii-n-ross-ru-0001-01bi00" target="_blank">реестре сертифицированных средств ФСТЭК</a> значится более 2000 позиций, а в аналогичном <a href="http://clsz.fsb.ru/certification.htm" target="_blank">Перечне от ФСБ</a> - в пять раз меньше.

Сам перечень средств, сертифицированных ФСБ, конечно, не радует в плане своего оформления, представляя собой таблицу, вставленную в doc-документ. Попытка скопировать эту таблицу в Excel не сильно помогает - некоторые ячейки получаются произвольно-хаотично объединены странными группами, а некоторые (например, изготовитель, название продукта и его описание) наоборот разбиты на произвольное число строк от 2 до 6, даты начала и окончания действия сертификата расположены в соседних по вертикали(!) ячейках и т.д. Наверное, работать можно привыкнуть и с таким представлением информации, но для своего удобства я сделал Перечень в более приятном глазу и автоматическому фильтру Excel виде (доступен по этой ссылке: <a href="http://bit.ly/HuKeIS" target="_blank">Перечень средств защиты информации, сертифицированных ФСБ России</a>).

Однако, если с формой ещё можно что-то сделать, то разобраться в содержании под силу только глубоко разбирающемуся в теме специалисту. Какой-либо классификации продуктов особо не предусмотрено, да ещё и каждый разработчик называет изделие по своему усмотрению. Немного спасают более-менее сходные описания выполняемых функций, но разобраться в них удалось не сразу.

После вдумчивого изучения представленных в Перечне продуктов пришёл к (надеюсь, оправдавшему себя) предположению, что интересующие нас сегодня криптошлюзы - это те изделия, в описании функций которых упоминается протокол IP и криптографическая защита. Таких сертификатов оказалось целых 80, но реально продуктов гораздо меньше, так как присутствуют отдельные сертификаты на разные версии продуктов или даже их модули, а в некоторых случаях на каждое исполнение выписан отдельный сертификат с отдельным номером.

Итак, отфильтровав строки в Excel, давайте посмотрим, чем же нам можно пользоваться для шифрования IP-трафика.

Из уже встречавшихся в обзорах сертифицированных ФСТЭК межсетевых экранов имеют сертификаты ФСБ такие продукты:
<ul>
	<li><strong>ViPNet</strong> (разработчик ИнфоТеКС)</li>
	<li><strong>Континент</strong> (разработчик Информзащита, Код Безопасности)</li>
	<li><strong>CSP VPN</strong> (разработчик С-Терра СиЭсПи)</li>
	<li><strong>ЗАСТАВА</strong> (разработчик ЭЛВИС-ПЛЮС)</li>
	<li><strong>StoneGate SSL VPN</strong> (разработчик Новые технологии безопасности)</li>
	<li><strong>DioNIS</strong> (разработчик Фактор-ТС)</li>
	<li><strong>АТЛИКС-VPN</strong> (разработчик НТЦ Атлас)</li>
	<li><strong>Туннель</strong> (разработчик АМИКОН, ИнфоКрипт -  ПАК на основе <strong>ФПСУ-IP</strong>)</li>
</ul>
Дополнительно присутствуют два узкоспециальных изделия и два (если я правильно понял) криптографических провайдера:
<ul>
	<li><strong>Модуль HSM</strong> (разработчик НТЦ Атлас, <a href="http://web.stcnet.ru/products_pid_31.htm" target="_blank">описание</a>)</li>
	<li><strong>М-448-1.4</strong> (разработчик ГУ спецпрограмм Президента РФ, РЦЗИ ФОРТ, <a href="http://www.rczifort.ru/products.html" target="_blank">описание</a>)</li>
	<li><strong>Барьер IPSec</strong> (разработчик Валидата)</li>
	<li><strong>КриптоПро CSP/IPSec</strong> (разработчик  КРИПТО-ПРО)</li>
</ul>
Как видно, число межсетевых экранов, сертифицированных не только во ФСТЭК, но и в ФСБ крайне мало - фактически можно говорить лишь о семи игроках. Такое малое количество вендоров позволяет сильным - чувствовать себя в относительной безопасности, а остальным - достаточно комфортно находится в своей узкой нише. Любое изменение устоявшегося равновесия не на руку никому из них, ну, лидерам рынка так уж точно.

Второе наблюдение, которое можно сделать - почти все продукты изначально российского производства. Да, компания-разработчик сертифицированного ФСБ СКЗИ может быть только российским юридическим лицом, но и сами продукты в большинстве своём представляют собой отечественные продукты, положа руку на сердце, разрабатываемые исключительно для выполнения требований регуляторов. Каких-либо серьёзных успехов за пределами России (кроме, понятно, сопредельных дружеских государств) никто из представленных отечественных вендоров со своими разработками пока не добился.

Ситуация серьёзно изменилась в прошлом году, когда произошло знаковое (но, быть может, тогда ещё не такое значительное) событие: доработанный до требований российских реалий <a href="https://zlonov.ru/2012/04/fsb_certificate_for_stonegate_ssl/ " target="_blank">продукт StoneGate SSL был сертифицирован ФСБ</a>. Изначально разрабатываемый для открытого коммерческого мирового рынка продукт получил сертификат ФСБ - есть ли в Перечне ещё такие примеры?

Но, всё же, это был не классический IPSec криптошлюз, а SSL-решение со всеми вытекающими нюансами, к которым рынку ещё нужно было привыкнуть. Примерно в то же время, что и для StoneGate SSL, была анонсирована сертификация StoneGate FW/VPN.

Мы можем догадываться и предполагать, с какими трудностями пришлось столкнуться команде, занимавшейся этой сертификацией, но все они были успешно преодолены и в октябре StoneGate FW/VPN получил сертификат ФСБ № СФ/124-2027 от 04.10.2013 (пока в Перечне от 07.10.2013 почему-то отсутствует). Вот теперь уже можно говорить, что на рынке криптошлюзов появилась прямая угроза для действующих игроков. При этом, если вспомнить, что StoneGate - это коммерчески успешный в мире продукт, настолько успешный, что <a href="https://zlonov.ru/2013/05/mcafee-stonesoft/" target="_blank">компания Stonesoft даже стала лакомым кусочком для McAfee</a> и своим продуктовым портфелем расширила линейку решений данного вендора, то становится ясно - угроза эта более, чем просто немного опасная.

Понятно, что этот рынок достаточно инертен и не стоит ждать резких изменений уже завтра. В конце концов, есть выстроенные каналы сбыта, определённая инсталляционная база, которую вот так единоразово не обновишь, да и какие-то личные человеческие отношения и договорённости, как это водится, наверняка, имеют место быть. Вместе с тем, событие это, без сомнения, важное для всего рынка и теперь у российских заказчиков и интераторов, реализующих проекты, есть отличная альтернатива привычному прежнему набору сертифицированных решений для построения шифрованных каналов передачи данных с использованием российской криптографии.
