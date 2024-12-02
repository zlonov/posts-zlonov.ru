---
layout: zlonov/old_post

title: '[таблицы] МЭ, сертифицированные по новым требованиям'
date: 2018-06-21

header:
    teaser: /assets/images/2018/FW.png
    overlay_image: /assets/images/2018/FW.png
    show_overlay_excerpt: true
    overlay_filter: 0.25

tags: ['межсетевые экраны', 'обзор', 'подборка', 'сертификация ФСТЭК']
category: security
AllowComments: true
LinkedLinks: ""
---
> **См. также:**
> * [Антивирусы, сертифицированные по новым требованиям](/new-fstec-av)
> * [Сертифицированные системы обнаружения вторжений в 2022 году](/newest-fstec-ips)
> * [Средства доверенной загрузки, сертифицированные по новым требованиям](/trusted-boot)

> **Важно!**\
> Информация в приведённых таблицах актуальна на дату публикации. Текущие действующие сертификаты ФСТЭК можно посмотреть в соответствующем <a href="http://bit.ly/reestr-fstec">Реестре ФСТЭК</a>. Также по возможности актуализируется информация в <a href="https://zlonov.com/catalog/">Каталоге средств защиты информации.

Свежие (текущие) требования к межсетевым экранам <a href="https://fstec.ru/normotvorcheskaya/informatsionnye-i-analiticheskie-materialy/1184-informatsionnoe-soobshchenie-fstek-rossii-ot-12-sentyabrya-2016-g-n-240-24-4278">были утверждены ФСТЭК России</a> 12 сентября 2016 г. Именно тогда официально появились методические документы, содержащие <a href="https://fstec.ru/tekhnicheskaya-zashchita-informatsii/dokumenty-po-sertifikatsii/120-normativnye-dokumenty/1185-metodicheskie-dokumenty-utverzhdeny-fstek-rossii-12-sentyabrya-2016-g">профили защиты межсетевых экранов для 5 типов и 6 классов межсетевых экранов</a>.

Кратко напомню (и сам для себя ещё раз зафиксирую, чтобы потом знать, где искать), какие типы межсетевых экранов c точки зрения ФСТЭК бывают:
<ul>
 	<li><strong>МЭ типа «А»</strong> – это МЭ, применяемый на физической границе (периметре) информационной системы или между физическими границами сегментов информационной системы.</li>
 	<li><strong>МЭ типа «Б»</strong> – это МЭ, применяемый на логической границе (периметре) информационной системы или между логическими границами сегментов информационной системы.</li>
 	<li><strong>МЭ типа «В»</strong> – это МЭ, применяемый на узле (хосте) информационной системы.</li>
 	<li><strong>МЭ типа «Г»</strong> – это МЭ, применяемый на сервере, обслуживающем сайты, веб-службы и веб-приложения, или на физической границе сегмента таких серверов (сервера). Межсетевые экраны типа «Г» могут иметь программное или программно-техническое исполнение и должны обеспечивать контроль и фильтрацию информационных потоков по протоколу передачи гипертекста, проходящих к веб-серверу и от веб-сервера.</li>
 	<li><strong>МЭ уровня промышленной сети (тип «Д»)</strong> – это МЭ, применяемый в автоматизированной системе управления технологическими или производственными процессами. МЭ типа «Д» может иметь программное или программно-техническое исполнение и должен обеспечивать контроль и фильтрацию промышленных протоколов передачи данных (Modbus, Profibus, CAN, HART, Industrial Ethernet и (или) иные протоколы).</li>
</ul>
C классами защиты ещё проще - чем выше класс (1 - самый высокий), (тем больше к ним требований и) тем в более высокого класса систем (ГИС, АСУ, ИСПДн, системы значимых объектов КИИ) они могут применяться.

Для удобства были введены идентификаторы профилей защиты в формате <strong>ИТ.МЭ.«тип»«класс».ПЗ </strong>Вот полная их таблица:

<table>
<tbody>
<tr>
<td><strong>Класс защиты / Тип межсетевого экрана</strong></td>
<td><strong>6</strong></td>
<td><strong>5</strong></td>
<td><strong>4</strong></td>
<td><strong>3</strong></td>
<td><strong>2</strong></td>
<td><strong>1</strong></td>
</tr>
<tr>
<td>Межсетевой экран типа «А»</td>
<td><a href="https://zlonov.ru/catalog/tags/ит-мэ-а6-пз/">ИТ.МЭ.
А6.ПЗ</a></td>
<td><a href="https://zlonov.ru/catalog/tags/ит-мэ-а5-пз/">ИТ.МЭ.
А5.ПЗ</a></td>
<td><a href="https://zlonov.ru/catalog/tags/ит-мэ-а4-пз/">ИТ.МЭ.
А4.ПЗ</a></td>
<td><a href="https://zlonov.ru/catalog/tags/ит-мэ-а3-пз/">ИТ.МЭ.
А3.ПЗ</a></td>
<td><a href="https://zlonov.ru/catalog/tags/ит-мэ-а2-пз/">ИТ.МЭ.
А2.ПЗ</a></td>
<td>ИТ.МЭ.
А1.ПЗ</td>
</tr>
<tr>
<td>Межсетевой экран типа «Б»</td>
<td><a href="https://zlonov.ru/catalog/tags/ит-мэ-б6-пз/">ИТ.МЭ.
Б6.ПЗ</a></td>
<td><a href="https://zlonov.ru/catalog/tags/ит-мэ-б5-пз/">ИТ.МЭ.
Б5.ПЗ</a></td>
<td><a href="https://zlonov.ru/catalog/tags/ит-мэ-б4-пз/">ИТ.МЭ.
Б4.ПЗ</a></td>
<td>ИТ.МЭ.
Б3.ПЗ</td>
<td>ИТ.МЭ.
Б2.ПЗ</td>
<td>ИТ.МЭ.
Б1.ПЗ</td>
</tr>
<tr>
<td>Межсетевой экран типа «В»</td>
<td>ИТ.МЭ.
В6.ПЗ</td>
<td>ИТ.МЭ.
В5.ПЗ</td>
<td><a href="https://zlonov.ru/catalog/tags/ит-мэ-в4-пз/">ИТ.МЭ.
В4.ПЗ</a></td>
<td>ИТ.МЭ.
В3.ПЗ</td>
<td><a href="https://zlonov.ru/catalog/tags/ит-мэ-в2-пз/">ИТ.МЭ.
В2.ПЗ</a></td>
<td>ИТ.МЭ.
В1.ПЗ</td>
</tr>
<tr>
<td>Межсетевой экран типа «Г»</td>
<td>ИТ.МЭ.
Г6.ПЗ</td>
<td>ИТ.МЭ.
Г5.ПЗ</td>
<td><a href="https://zlonov.ru/catalog/tags/ит-мэ-г4-пз/">ИТ.МЭ.
Г4.ПЗ</a></td>
<td>-</td>
<td>-</td>
<td>-</td>
</tr>
<tr>
<td>Межсетевой экран типа «Д»</td>
<td>ИТ.МЭ.
Д6.ПЗ</td>
<td>ИТ.МЭ.
Д5.ПЗ</td>
<td>ИТ.МЭ.
Д4.ПЗ</td>
<td>-</td>
<td>-</td>
<td>-</td>
</tr>
</tbody>
</table>

С момента утверждения новых требований прошло более полутора лет, но в <a href="http://bit.ly/reestr-fstec">реестре ФСТЭК</a> присутствуют (на момент публикации) только 43 сертификата с упоминанием профилей защиты ИТ.МЭ и только 22 из них выданы на серию, а не на ограниченную партию изделий.

Ниже приведены все доступные на сегодня сертифицированные по новым требованиям (и при этом серией) межсетевые экраны, сгруппированные по типам.
<h2>Межсетевые экраны типа «А»</h2>

<table>
<tbody>
<tr>
<td width="15%"><strong>Класс защиты</strong></td>
<td><strong>№ сертификата - Межсетевые экраны</strong></td>
</tr>
<tr>
<td>ИТ.МЭ.А<strong>1</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
<tr>
<td>ИТ.МЭ.А<strong>2</strong>.ПЗ</td>
<td>
<ul>
 	<li><strong>2574</strong> - <a href="https://zlonov.ru/catalog/рубикон/">Межсетевой экран и система обнаружения вторжений Рубикон</a></li>
 	<li><strong>3530</strong> - <a href="https://zlonov.ru/catalog/dionis-nx/">программно-аппаратный комплекс Dionis-NX с установленным программным обеспечением версий 1.2-6 Hand, 1.2-7 Hand и 1.2-8 Hand UTM</a></li>
 	<li><strong>3886</strong> - <a href="https://zlonov.ru/catalog/маршрутизатор-доступа/">аппаратно-программный комплекс Маршрутизатор доступа</a></li>
</ul>
</td>
</tr>
<tr>
<td>ИТ.МЭ.А<strong>3</strong>.ПЗ</td>
<td>
<ul>
 	<li><strong>3008</strong> - <a href="https://zlonov.ru/catalog/континент-3-7/">Континент 3.7</a></li>
</ul>
</td>
</tr>
<tr>
<td>ИТ.МЭ.А<strong>4</strong>.ПЗ</td>
<td>
<ul>
 	<li><strong>3634</strong> - <a href="https://zlonov.ru/catalog/check-point-security-gateway/">шлюз безопасности Check Point Security Gateway версии R77.10</a></li>
 	<li><strong>3692</strong> - <a href="https://zlonov.ru/catalog/vipnet-coordinator/">программно-аппаратный комплекс защиты информации ViPNet Coordinator HW 4</a></li>
 	<li><strong>3720</strong> - <a href="https://zlonov.ru/catalog/fortigate/">FortiGate (функционирующий под управлением операционной системы FortiOS 5.4.1) </a></li>
 	<li><strong>3834</strong> - <a href="https://zlonov.ru/catalog/traffic-inspector-next-generation/">программно-аппаратный комплекс Traffic Inspector Next Generation</a></li>
 	<li><strong>3905</strong> - <a href="https://zlonov.ru/catalog/usergate-utm/">изделие Универсальный шлюз безопасности UserGate UTM</a></li>
</ul>
</td>
</tr>
<tr>
<td>ИТ.МЭ.А<strong>5</strong>.ПЗ</td>
<td>
<ul>
 	<li><strong>3778</strong> - <a href="https://zlonov.ru/catalog/маршрутизатор-esr/">маршрутизатор ESR-1000 с программным обеспечением esr-1000-1.0.7-ST</a></li>
 	<li><strong>3788</strong> - <a href="https://zlonov.ru/catalog/маршрутизатор-esr/">маршрутизатор ESR-100 с программным обеспечением esr-100-1.0.7-ST</a></li>
 	<li><strong>3789</strong> - <a href="https://zlonov.ru/catalog/маршрутизатор-esr/">маршрутизатор ESR-200 с программным обеспечением esr-200-1.0.7-ST</a></li>
</ul>
</td>
</tr>
<tr>
<td>ИТ.МЭ.А<strong>6</strong>.ПЗ</td>
<td>
<ul>
 	<li><strong>3892</strong> - <a href="https://zlonov.ru/catalog/cisco-asa-services-module/">межсетевой экран Cisco ASA-SM1 с установленным программным обеспечением Cisco ASA версии 9.x</a></li>
 	<li><strong>3909</strong> - <a href="https://zlonov.ru/catalog/eudemon8000e-x-terabit-firewall/">межсетевой экран Huawei Eudemon (модель Eudemon 8000E-X3) версии V500</a></li>
 	<li><strong>3935</strong> - <a href="https://zlonov.ru/catalog/huawei-ar/">маршрутизаторы серии Huawei AR (модели: AR2220E, AR2240, AR161FG-L) версии V200</a></li>
</ul>
</td>
</tr>
</tbody>
</table>

<h2>Межсетевые экраны типа «Б»</h2>

<table>
<tbody>
<tr>
<td width="15%"><strong>Класс защиты</strong></td>
<td><strong>№ сертификата - Межсетевые экраны</strong></td>
</tr>
<tr>
<td>ИТ.МЭ.Б<strong>1</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
<tr>
<td>ИТ.МЭ.Б<strong>2</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
<tr>
<td>ИТ.МЭ.Б<strong>3</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
<tr>
<td>ИТ.МЭ.Б<strong>4</strong>.ПЗ</td>
<td>
<ul>
 	<li><strong>3462</strong> - <a href="https://zlonov.ru/catalog/kaspersky-hybrid-cloud-security/">Kaspersky Security для виртуальных сред 3.0 Защита без агента</a></li>
 	<li><strong>3634</strong> - <a href="https://zlonov.ru/catalog/check-point-security-gateway/">шлюз безопасности Check Point Security Gateway версии R77.10</a></li>
 	<li><strong>3720</strong> - <a href="https://zlonov.ru/catalog/fortigate/">FortiGate (функционирующий под управлением операционной системы FortiOS 5.4.1)</a></li>
 	<li><strong>3834</strong> - <a href="https://zlonov.ru/catalog/traffic-inspector-next-generation/">программно-аппаратный комплекс Traffic Inspector Next Generation</a></li>
 	<li><strong>3871</strong> - <a href="https://zlonov.ru/catalog/рустэк/">программный комплекс РУСТЭК версия 1.0</a></li>
 	<li><strong>3905</strong> - <a href="https://zlonov.ru/catalog/usergate-utm/">изделие Универсальный шлюз безопасности UserGate UTM</a></li>
</ul>
</td>
</tr>
<tr>
<td>ИТ.МЭ.Б<strong>5</strong>.ПЗ</td>
<td>
<ul>
 	<li><strong>2407</strong> - <a href="https://zlonov.ru/catalog/трафик-инспектор/">Traffic Inspector 3.0</a></li>
</ul>
</td>
</tr>
<tr>
<td>ИТ.МЭ.Б<strong>6</strong>.ПЗ</td>
<td>
<ul>
 	<li><strong>3844</strong> - <a href="https://zlonov.ru/catalog/vmware-nsx-for-vsphere/">программный комплекс VMware NSX for vSphere 6</a></li>
 	<li><strong>3892</strong> - <a href="https://zlonov.ru/catalog/cisco-asa-services-module/">межсетевой экран Cisco ASA-SM1 с установленным программным обеспечением Cisco ASA версии 9.x</a></li>
 	<li><strong>3909</strong> - <a href="https://zlonov.ru/catalog/eudemon8000e-x-terabit-firewall/">межсетевой экран Huawei Eudemon (модель Eudemon 8000E-X3) версии V500</a></li>
 	<li><strong>3935</strong> - <a href="https://zlonov.ru/catalog/huawei-ar/">маршрутизаторы серии Huawei AR (модели: AR2220E, AR2240, AR161FG-L) версии V200</a></li>
</ul>
</td>
</tr>
</tbody>
</table>

<h2>Межсетевые экраны типа «В»</h2>

<table>
<tbody>
<tr>
<td width="15%"><strong>Класс защиты</strong></td>
<td><strong>№ сертификата - Межсетевые экраны</strong></td>
</tr>
<tr>
<td>ИТ.МЭ.В<strong>1</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
<tr>
<td>ИТ.МЭ.В<strong>2</strong>.ПЗ</td>
<td>
<ul>
 	<li><strong>3675</strong> - <a href="https://zlonov.ru/catalog/secret-net-studio/">средство защиты информации Secret Net Studio — C</a></li>
</ul>
</td>
</tr>
<tr>
<td>ИТ.МЭ.В<strong>3</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
<tr>
<td>ИТ.МЭ.В<strong>4</strong>.ПЗ</td>
<td>
<ul>
 	<li><strong>3745</strong> - <a href="https://zlonov.ru/catalog/secret-net-studio/">cредство защиты информации Secret Net Studio</a></li>
</ul>
</td>
</tr>
<tr>
<td>ИТ.МЭ.В<strong>5</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
<tr>
<td>ИТ.МЭ.В<strong>6</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
</tbody>
</table>

<h2>Межсетевые экраны типа «Г»</h2>

<table>
<tbody>
<tr>
<td width="15%"><strong>Класс защиты</strong></td>
<td><strong>№ сертификата - Межсетевые экраны</strong></td>
</tr>
<tr>
<td>ИТ.МЭ.Г<strong>1</strong>.ПЗ</td>
<td>не предусмотрен</td>
</tr>
<tr>
<td>ИТ.МЭ.Г<strong>2</strong>.ПЗ</td>
<td>не предусмотрен</td>
</tr>
<tr>
<td>ИТ.МЭ.Г<strong>3</strong>.ПЗ</td>
<td>не предусмотрен</td>
</tr>
<tr>
<td>ИТ.МЭ.Г<strong>4</strong>.ПЗ</td>
<td>
<ul>
 	<li><strong>3455</strong> - <a href="https://zlonov.ru/catalog/pt-application-firewall/">cистема защиты приложений от несанкционированного доступа Positive Technologies Application Firewall</a></li>
</ul>
</td>
</tr>
<tr>
<td>ИТ.МЭ.Г<strong>5</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
<tr>
<td>ИТ.МЭ.Г<strong>6</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
</tbody>
</table>

<h2>Межсетевые экраны типа «Д»</h2>

<table>
<tbody>
<tr>
<td width="15%"><strong>Класс защиты</strong></td>
<td><strong>№ сертификата - Межсетевые экраны</strong></td>
</tr>
<tr>
<td>ИТ.МЭ.Д<strong>1</strong>.ПЗ</td>
<td>не предусмотрен</td>
</tr>
<tr>
<td>ИТ.МЭ.Д<strong>2</strong>.ПЗ</td>
<td>не предусмотрен</td>
</tr>
<tr>
<td>ИТ.МЭ.Д<strong>3</strong>.ПЗ</td>
<td>не предусмотрен</td>
</tr>
<tr>
<td>ИТ.МЭ.Д<strong>4</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
<tr>
<td>ИТ.МЭ.Д<strong>5</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
<tr>
<td>ИТ.МЭ.Д<strong>6</strong>.ПЗ</td>
<td>пока нет</td>
</tr>
</tbody>
</table>


<hr />

Как видно, некоторые типы сертифицированных межсетевых экранов представлены в крайне ограниченном количестве, а например, МЭ типа Д и вовсе пока отсутствуют.

Для полноты картины стоит отметить, что, судя по уже выданным сертификатам, есть возможность сертифицировать как МЭ типа А шестого класса защиты (ИТ.МЭ.А6.ПЗ) партии устройств Cisco:
<ul>
 	<li>коммутатор Cisco 6504 VS-S720-10G с установленным программным обеспечением Cisco IOS версии 15.1(2)SY10</li>
 	<li>коммутатор Cisco Catalyst WS-C3560V2-24TS с установленным программным обеспечением Cisco IOS версии 12.2(55)SE12</li>
 	<li>коммутатор Cisco Catalyst WS-C3560X-24T с установленным программным обеспечением Cisco IOS версии 15.0(2)SE11</li>
 	<li>коммутатор Cisco Catalyst WS-C3650-24TD-E с установленным программным обеспечением Cisco IOS-XE версии 03.06.07.E</li>
 	<li>коммутатор Cisco Nexus 5596 с установленным программным обеспечением Cisco NX-OS версии 7.1(2)N1(1)</li>
 	<li>коммутатор Cisco Nexus 7000 с установленным программным обеспечением Cisco NX-OS версии 7.2(1)D1(1)</li>
 	<li>коммутатор Cisco WS-C6506-E с установленным программным обеспечением Cisco IOS версии 15.1(2)SY10</li>
 	<li>маршрутизатор Cisco 2901/K9 с установленным программным обеспечением Cisco IOS версии 15.4(3)М9</li>
 	<li>маршрутизатор Cisco 2911/K9 с установленным программным обеспечением Cisco IOS версии 15.4(3)М9</li>
 	<li>маршрутизатор Cisco C3900-SPE200/K9 с установленным программным обеспечением Cisco IOS версии 15.4(3)М9</li>
 	<li>межсетевой экран Cisco ASA 5512-X с установленным программным обеспечением Cisco Adaptive Security Appliance Software v. 9.6.3</li>
 	<li>межсетевой экран Cisco ASA 5525-X с установленным программным обеспечением Cisco Adaptive Security Appliance Software v. 9.6.3</li>
 	<li>межсетевой экран Cisco ASA5508-K8 с установленным программным обеспечением Cisco ASA версии 9.6(4)3</li>
 	<li>межсетевой экран Cisco ASA5510-K8 с установленным программным обеспечением Cisco ASA версии 9.1(7)19</li>
 	<li>межсетевой экран Cisco ASA5512-X-K8 с установленным программным обеспечением Cisco ASA версии 9.2(4)27</li>
 	<li>межсетевой экран Cisco ASA5515-K8 с установленным программным обеспечением Cisco ASA версии 9.2(4)27</li>
 	<li>межсетевой экран Cisco ASA5520-K8 с установленным программным обеспечением Cisco ASA версии 9.1(7)23</li>
 	<li>межсетевой экран Cisco ASA5525-K8 с установленным программным обеспечением Cisco ASA версии 9.2(4)27</li>
 	<li>межсетевой экран Cisco ASA5550-K8 c установленным программным обеспечением Cisco ASA версии 9.1(7)23</li>
 	<li>межсетевой экран Cisco ASA5555-K8 с установленным программным обеспечением Cisco ASA версии 9.2(4)27</li>
 	<li>межсетевой экран Cisco ASA5585-K8 с установленным программным обеспечением Cisco ASA версии 9.2(4)27</li>
</ul>
