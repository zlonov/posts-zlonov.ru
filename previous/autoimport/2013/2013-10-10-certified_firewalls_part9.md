---
layout: zlonov/old_post
title: Сертифицированные межсетевые экраны (часть 9)
date: 2013-10-10 18:38
author: admin
category: autoimport
tags: [информационная безопасность, межсетевой экран, регулирование, сертификация, СЗИ]
---
<div title="Page 1">

Почти год прошёл с момента последней актуализации <a href="https://zlonov.ru/certified_firewalls/">таблицы сертифицированных межсетевых экранов</a>, пришла пора обновить информацию в ней, пока она окончательно не устарела.

Для оптимизации внешнего вида в самой таблице убрал ссылки - поддерживать их в актуальном состоянии не просто, а найти сайт вендора или описание продукта самостоятельно не так и сложно, а также исключил малоинформативные столбцы про ОС и актуальность - условно будем считать, что продукт актуален, пока на него действует сертификат.

Посмотрим, какие изменения произошли с ноября прошлого года. Прежде всего приведу краткий список продлённых сертификатов:
<ul>
	<li><strong>DioNIS Security Server v.6.0</strong> - №359/5 до 03 мая 2015 года</li>
	<li><strong>ИВК Кольчуга</strong> - №1094/1 до 29.06.2015</li>
	<li><strong>Cisco ASA-5505</strong> - №1976 до 11.12.2015</li>
	<li><strong>ViPNet CUSTOM 3.2</strong> - №1549/1 до 26.05.2016</li>
	<li><strong>ФПСУ-IP/Клиент</strong> - №1281 до 03.11.2015</li>
	<li><strong>WatchGuard Firebox</strong> - №2038 до 16.02.2016</li>
	<li><strong>ССПТ-2</strong> - №2141 до 23.07.2016 (согласно разработчику)</li>
	<li><strong>Security Studio Endpoint Protection Personal Firewall</strong> - №2170 до 20.09.2016</li>
	<li><strong>CSP VPN Server v. 3.1</strong> - №2197 до 10.11.2016</li>
	<li><strong>CSP VPN Gate v. 3.1</strong> - №2198 до 10.11.2016</li>
	<li><strong>CSP VPN Client v. 3.1</strong> - №2199 до 10.11.2016</li>
	<li><strong>TrustAccess</strong> - №2146 до 30.07.2016 (согласно разработчику)</li>
	<li><strong>TrustAccess S</strong> - №2147 до 30.07.2016 (согласно разработчику)</li>
	<li><strong>Z-2</strong> - №1353 до 09.03.2016</li>
	<li><strong>Z-2, версия 2.6</strong> - №1353/1 до 05.08.2015</li>
</ul>
Последние два, как оказалось, рано были списаны мной со счетов, раз сертификаты на них были обновлены. Информация о некоторых продлениях пока отсутствует в реестре, но имеется на сайте разработчиков. В таблице дата окончания таких сертификатов отмечена оранжевым цветом.

Теперь о "потерях". Закончили своё действие и не были продлены целый ряд сертификатов на продукты <strong>Cisco</strong>: ASA-5510, ASA-5520, Cisco ASA-5540, FWSM, 1800, 2800, 3800, 7200, 7600, 3750, 1841, 2811, 6509, 3825. Есть непродлившиеся сертфикаты у <strong>Кода Безопасности</strong>, <strong>ЛИССИ-Крипто</strong>, <strong>Check Point</strong>. Все их убрал из таблицы.

«Отмучались» <strong>Proventia Server</strong> и <strong>Proventia Desktop</strong>, сильно сдавшие позиции после покупкой их производителя ISS компанией IBM.

Видимо, ничего не получилось и с <a href="https://zlonov.ru/2012/06/certified_firewalls_part5/#RSOS6850">«псевдо-российским» <strong>RSOS6850</strong></a> - сертификат на него не был продлён.

Есть также несколько сертификатов <strong>Cisco</strong>, <strong>ИнфоТеКС</strong> и <strong>Stonesoft</strong>, истекших в августе, которые пока оставил в таблице, так как есть в её обновлении определённая инертность. Про Stonesoft, кстати, достоверно знаю, что сертификаты будут продлены.

</div>
<div title="Page 2">

С сертификатом №2540 на <strong>Cisco 881</strong> история получилась странная - ранее он присутствовал в реестре с указанием «серия», сейчас же только «20 экз.». Убираем.

Забавная накладка с сертификатом №1091 на <strong>ФПСУ-IP</strong> - он всё ещё числится в реестре ФСТЭК как просроченный, хотя <a href="http://amicon.ru/img/about/sert/ sert1091-2011-2014.jpg" target="_blank">актуальная (не фейковая ли только?) копия</a> присутствует на сайте вендора.

Наконец, в реестре появилось значительное число новых сертифицированных межсетевых экранов как от уже присутствующих на этом рынке игроков, так и от совсем новых:
<ul>
	<li><strong>D-Link DFL-260E</strong></li>
	<li><strong>D-Link DFL-860E</strong></li>
	<li><strong>D-Link DFL-1660</strong></li>
	<li><strong>Kerio Control</strong></li>
	<li><strong>Altell NEO ПО</strong></li>
	<li><strong>Check Point Security Gateway R71</strong></li>
	<li><strong>Filter</strong></li>
	<li><strong>D-Link DFL-256</strong></li>
	<li><strong>Cisco 2911R</strong></li>
	<li><strong>Dionis NX</strong></li>
	<li><strong>Deep Security 8.0</strong></li>
	<li><strong>Cisco ASA 5510</strong></li>
	<li><strong>Cisco IE-3000-8TC</strong></li>
	<li><strong>ViPNet Terminal 3.0</strong></li>
</ul>
Подробнее о новинках поговорим в следующий раз, пока же выкладываю <a href="https://zlonov.ru/certified_firewalls/#table" target="_blank">обновлённую таблицу</a>. Если у вас предложения/замечания - буду за них признателен. <a href="https://zlonov.ru/contactme/">Мои контакты</a>.

</div>
