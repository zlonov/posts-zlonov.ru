---
layout: zlonov/old_post

title: '[таблицы] Системы обнаружения вторжений, сертифицированные по новым требованиям'
date: 2018-08-22
featured-image: /2018/IPS.jpg
tags: ['Check Point', 'Dallas Lock', 'Dionis-NX', 'FortiGate', 'Secret Net Studio', 'Trend Micro', 'UserGate UTM', 'ViPNET IDS', 'ИВК Сенсор', 'Континент', 'Ребус-СОВ', 'Рубикон', 'СОВ', 'СОВ Кречет', 'СрЗИ', 'Форпост', 'ФСТЭК']
category: security
AllowComments: true
LinkedLinks: ""
---
> **Добавлено 18.02.2022**\
> Свежий обзор сертифицированных СОВ: [Сертифицированные системы обнаружения вторжений в 2022 году](/newest-fstec-ips)

> **См. также:**
> * [Межсетевые экраны, сертифицированные по новым требованиям](/new-fstec-fw)
> * [Антивирусы, сертифицированные по новым требованиям](/new-fstec-av)
> * [Средства доверенной загрузки, сертифицированные по новым требованиям](/trusted-boot)

> **Важно!**\
> Информация в приведённых таблицах актуальна на дату публикации. Текущие действующие сертификаты ФСТЭК можно посмотреть в соответствующем <a href="http://bit.ly/reestr-fstec">Реестре ФСТЭК</a>. Также по возможности актуализируется информация в <a href="https://zlonov.com/catalog/">Каталоге средств защиты информации.

Требования (профили защиты) к системам обнаружения вторжений (СОВ) были утверждены Приказом ФСТЭК России №638 от 6 декабря 2011 года &nbsp;и &nbsp;<a href="https://fstec.ru/tekhnicheskaya-zashchita-informatsii/dokumenty-po-sertifikatsii/118-prikazy/394-informatsionnoe-pismo-fstek-rossii?highlight=WyJcdTA0M2VcdTA0MzEiLCJcdTA0NDNcdTA0NDJcdTA0MzJcdTA0MzVcdTA0NDBcdTA0MzZcdTA0MzRcdTA0MzVcdTA0M2RcdTA0MzhcdTA0MzgiLCJcdTA0NDJcdTA0NDBcdTA0MzVcdTA0MzFcdTA0M2VcdTA0MzJcdTA0MzBcdTA0M2RcdTA0MzhcdTA0MzkiLCJcdTA0M2EiLCJcdTA0NDFcdTA0MzhcdTA0NDFcdTA0NDJcdTA0MzVcdTA0M2NcdTA0MzBcdTA0M2MiLCJcdTA0M2VcdTA0MzFcdTA0M2RcdTA0MzBcdTA0NDBcdTA0NDNcdTA0MzZcdTA0MzVcdTA0M2RcdTA0MzhcdTA0NGYiLCJcdTA0MzJcdTA0NDJcdTA0M2VcdTA0NDBcdTA0MzZcdTA0MzVcdTA0M2RcdTA0MzhcdTA0MzkiLCJcdTA0M2VcdTA0MzEgXHUwNDQzXHUwNDQyXHUwNDMyXHUwNDM1XHUwNDQwXHUwNDM2XHUwNDM0XHUwNDM1XHUwNDNkXHUwNDM4XHUwNDM4IiwiXHUwNDNlXHUwNDMxIFx1MDQ0M1x1MDQ0Mlx1MDQzMlx1MDQzNVx1MDQ0MFx1MDQzNlx1MDQzNFx1MDQzNVx1MDQzZFx1MDQzOFx1MDQzOCBcdTA0NDJcdTA0NDBcdTA0MzVcdTA0MzFcdTA0M2VcdTA0MzJcdTA0MzBcdTA0M2RcdTA0MzhcdTA0MzkiLCJcdTA0NDNcdTA0NDJcdTA0MzJcdTA0MzVcdTA0NDBcdTA0MzZcdTA0MzRcdTA0MzVcdTA0M2RcdTA0MzhcdTA0MzggXHUwNDQyXHUwNDQwXHUwNDM1XHUwNDMxXHUwNDNlXHUwNDMyXHUwNDMwXHUwNDNkXHUwNDM4XHUwNDM5IiwiXHUwNDQzXHUwNDQyXHUwNDMyXHUwNDM1XHUwNDQwXHUwNDM2XHUwNDM0XHUwNDM1XHUwNDNkXHUwNDM4XHUwNDM4IFx1MDQ0Mlx1MDQ0MFx1MDQzNVx1MDQzMVx1MDQzZVx1MDQzMlx1MDQzMFx1MDQzZFx1MDQzOFx1MDQzOSBcdTA0M2EiLCJcdTA0NDJcdTA0NDBcdTA0MzVcdTA0MzFcdTA0M2VcdTA0MzJcdTA0MzBcdTA0M2RcdTA0MzhcdTA0MzkgXHUwNDNhIiwiXHUwNDQyXHUwNDQwXHUwNDM1XHUwNDMxXHUwNDNlXHUwNDMyXHUwNDMwXHUwNDNkXHUwNDM4XHUwNDM5IFx1MDQzYSBcdTA0NDFcdTA0MzhcdTA0NDFcdTA0NDJcdTA0MzVcdTA0M2NcdTA0MzBcdTA0M2MiLCJcdTA0M2EgXHUwNDQxXHUwNDM4XHUwNDQxXHUwNDQyXHUwNDM1XHUwNDNjXHUwNDMwXHUwNDNjIiwiXHUwNDNhIFx1MDQ0MVx1MDQzOFx1MDQ0MVx1MDQ0Mlx1MDQzNVx1MDQzY1x1MDQzMFx1MDQzYyBcdTA0M2VcdTA0MzFcdTA0M2RcdTA0MzBcdTA0NDBcdTA0NDNcdTA0MzZcdTA0MzVcdTA0M2RcdTA0MzhcdTA0NGYiLCJcdTA0NDFcdTA0MzhcdTA0NDFcdTA0NDJcdTA0MzVcdTA0M2NcdTA0MzBcdTA0M2MgXHUwNDNlXHUwNDMxXHUwNDNkXHUwNDMwXHUwNDQwXHUwNDQzXHUwNDM2XHUwNDM1XHUwNDNkXHUwNDM4XHUwNDRmIiwiXHUwNDQxXHUwNDM4XHUwNDQxXHUwNDQyXHUwNDM1XHUwNDNjXHUwNDMwXHUwNDNjIFx1MDQzZVx1MDQzMVx1MDQzZFx1MDQzMFx1MDQ0MFx1MDQ0M1x1MDQzNlx1MDQzNVx1MDQzZFx1MDQzOFx1MDQ0ZiBcdTA0MzJcdTA0NDJcdTA0M2VcdTA0NDBcdTA0MzZcdTA0MzVcdTA0M2RcdTA0MzhcdTA0MzkiLCJcdTA0M2VcdTA0MzFcdTA0M2RcdTA0MzBcdTA0NDBcdTA0NDNcdTA0MzZcdTA0MzVcdTA0M2RcdTA0MzhcdTA0NGYgXHUwNDMyXHUwNDQyXHUwNDNlXHUwNDQwXHUwNDM2XHUwNDM1XHUwNDNkXHUwNDM4XHUwNDM5Il0=">вступили в действие с 15 марта 2012 года</a>. Как и для других средств защиты информации, профили защиты открыто опубликованы только частично - доступны требования<strong>&nbsp;</strong><a href="https://fstec.ru/tekhnicheskaya-zashchita-informatsii/dokumenty-po-sertifikatsii/120-normativnye-dokumenty/406-metodicheskie-dokumenty-utverzhdeny-fstek-rossii-3-fevralya-2012-g">для четвёртого</a>,&nbsp;<a href="https://fstec.ru/tekhnicheskaya-zashchita-informatsii/dokumenty-po-sertifikatsii/120-normativnye-dokumenty/407-metodicheskie-dokumenty-utverzhdeny-fstek-rossii-6-marta-2012-g">пятого и шестого</a>&nbsp;классов защиты.




Всего было введено два типа систем обнаружения вторжений (СОВ):



<ul><li><strong>СОВ&nbsp;уровня сети</strong>: Датчики (сенсоры) собирают информацию о пакетах данных,&nbsp;<strong>передаваемых</strong>&nbsp;<strong>в пределах информационной системы</strong>(ИС) (сегмента ИС), в которой (котором) установлены эти датчики. Датчики СОВ уровня сети могут быть реализованы в виде программного обеспечения (ПО), устанавливаемого на стандартные программно-технические платформы, а также в виде программно-технических устройств, подключаемых к ИС (сегменту ИС);</li><li><strong>СОВ уровня узла</strong>: Датчики СОВ уровня узла представляют собой программные модули,&nbsp;<strong>устанавливаемые на защищаемые узлы информационной системы</strong>&nbsp;(ИС) и предназначенные для сбора информации о событиях, возникающих на этих узлах.</li></ul>



Помимо двух типов СОВ определены 6 классов защиты для них: чем выше класс (1 — самый высокий), тем больше к ним требований и тем в более высокого класса систем (ГИС, АСУ, ИСПДн, системы значимых объектов КИИ) они могут применяться.



<table class="wp-block-table"><thead><tr><th><strong>КЛАСС ЗАЩИТЫ</strong></th><th><strong>СОВ УРОВНЯ СЕТИ</strong></th><th><strong>СОВ УРОВНЯ УЗЛА</strong></th></tr></thead><tbody><tr><td>1</td><td>ИТ.СОВ.С1.ПЗ</td><td>ИТ.СОВ.У1.ПЗ</td></tr><tr><td>2</td><td><a href="https://zlonov.ru/catalog/tags/%D0%B8%D1%82-%D1%81%D0%BE%D0%B2-%D1%812-%D0%BF%D0%B7/">ИТ.СОВ.С2.ПЗ</a></td><td><a href="https://zlonov.ru/catalog/tags/%D0%B8%D1%82-%D1%81%D0%BE%D0%B2-%D1%832-%D0%BF%D0%B7/">ИТ.СОВ.У2.ПЗ</a></td></tr><tr><td>3</td><td><a href="https://zlonov.ru/catalog/tags/%D0%B8%D1%82-%D1%81%D0%BE%D0%B2-%D1%813-%D0%BF%D0%B7/">ИТ.СОВ.С3.ПЗ</a></td><td>ИТ.СОВ.У3.ПЗ</td></tr><tr><td>4</td><td><a href="https://zlonov.ru/catalog/tags/%D0%B8%D1%82-%D1%81%D0%BE%D0%B2-%D1%814-%D0%BF%D0%B7/">ИТ.СОВ.С4.ПЗ</a></td><td><a href="https://zlonov.ru/catalog/tags/%D0%B8%D1%82-%D1%81%D0%BE%D0%B2-%D1%834-%D0%BF%D0%B7/">ИТ.СОВ.У4.ПЗ</a></td></tr><tr><td>5</td><td><a href="https://zlonov.ru/catalog/tags/%D0%B8%D1%82-%D1%81%D0%BE%D0%B2-%D1%815-%D0%BF%D0%B7/">ИТ.СОВ.С5.ПЗ</a></td><td>ИТ.СОВ.У5.ПЗ</td></tr><tr><td>6</td><td>ИТ.СОВ.С6.ПЗ</td><td>ИТ.СОВ.У6.ПЗ</td></tr></tbody></table>



На момент публикации данного поста в&nbsp;<a href="http://bit.ly/reestr-fstec">реестре ФСТЭК</a>&nbsp;присутствует 22 сертификата с упоминанием профилей защиты СОВ и 19 из них выданы на серию (3 - на ограниченную партию изделий).&nbsp;



Ниже приведены все доступные на сегодня сертифицированные серией по текущим требованиям ФСТЭК системы обнаружения вторжений, сгруппированные по типам.



<strong>Важно!</strong>&nbsp;Информация в приведённых таблицах актуальна на дату публикации. Текущие действующие сертификаты ФСТЭК можно посмотреть в соответствующем&nbsp;<a href="http://bit.ly/reestr-fstec">Реестре ФСТЭК</a>. Также по возможности актуализируется информация в&nbsp;<a href="https://zlonov.ru/catalog/">Каталоге средств защиты информации</a>.



<h2 id="-">Системы обнаружения вторжений уровня сети</h2>


<!-- wp:table {"align":"center"} -->
<table class="wp-block-table aligncenter"><tbody><tr><td><strong>Класс защиты</strong></td><td><strong>№&nbsp;сертификата - Система обнаружения вторжений уровня сети</strong></td></tr><tr><td>ИТ.СОВ.С<strong>1</strong>.ПЗ</td><td>отсутствуют</td></tr><tr><td>ИТ.СОВ.С<strong>2</strong>.ПЗ</td><td><strong>2574</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/%D1%80%D1%83%D0%B1%D0%B8%D0%BA%D0%BE%D0%BD/">Межсетевой экран и система обнаружения вторжений Рубикон</a><br /><strong>3530</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/dionis-nx/">программно-аппаратный комплекс Dionis-NX с установленным программным обеспечением версий 1.2-6 Hand, 1.2-7 Hand и 1.2-8 Hand UTM</a><br /><strong>3856</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/%D1%80%D0%B5%D0%B1%D1%83%D1%81-%D1%81%D0%BE%D0%B2/">программный комплекс обнаружения вторжений Ребус-СОВ</a></td></tr><tr><td>ИТ.СОВ.С<strong>3</strong>.ПЗ</td><td><strong>2845</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/%D1%84%D0%BE%D1%80%D0%BF%D0%BE%D1%81%D1%82/">система обнаружения компьютерных атак Форпост, версия 2.0</a><br /><strong>3008</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/%D0%BA%D0%BE%D0%BD%D1%82%D0%B8%D0%BD%D0%B5%D0%BD%D1%82-3-7/">Континент 3.7</a></td></tr><tr><td>ИТ.СОВ.С<strong>4</strong>.ПЗ</td><td><strong>3634</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/check-point-security-gateway/">шлюз безопасности Check Point Security Gateway версии R77.10</a><br /><strong>3720</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/fortigate/">FortiGate</a><br /><strong>3804</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/vipnet-ids/">программно-аппаратный комплекс ViPNet IDS 2 (версия 2.4)</a><br /><strong>3868</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/%D1%81%D0%BE%D0%B2-%D0%B8%D0%B2%D0%BA-%D1%81%D0%B5%D0%BD%D1%81%D0%BE%D1%80/">программное изделие Система обнаружения вторжений ИВК Сенсор (СОВ ИВК СЕНСОР)</a><br /><strong>3905</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/usergate-utm/">изделие Универсальный шлюз безопасности UserGate UTM</a><br /><strong>3911</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/%D1%81%D0%BE%D0%B2-%D0%BA%D1%80%D0%B5%D1%87%D0%B5%D1%82/">программное средство системы обнаружения вторжений (СОВ) Кречет</a><br /><strong>3976</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/%D0%B0%D1%80%D0%BA%D0%B0%D0%BD/">программный комплекс Аркан</a><a href="https://zlonov.ru/catalog/check-point-security-gateway/"></a></td></tr><tr><td>ИТ.СОВ.С<strong>5</strong>.ПЗ</td><td><strong>3481</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/tippingpoint/">программно-аппаратный комплекс HP TippingPoint серий N и NX с операционной системой TOS версия 3 и системой управления SMS версия 3</a><br /><strong>3904</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/cisco-asa-firepower/">система обнаружения вторжений Cisco ASA FirePOWER версии 6.2, реализованная адаптивным устройством безопасности серии Cisco ASA 5500-X (модели: ASA 5506-X, ASA 5508-X, ASA 5512-X, ASA 5515-X, ASA 5516-X, ASA 5525-X, ASA 5545-X, ASA 5555-X, ASA 5585-X SSP10FP10)</a></td></tr><tr><td>ИТ.СОВ.С<strong>6</strong>.ПЗ</td><td>отсутствуют</td></tr></tbody></table>



<h2 id="--1"><strong>Системы обнаружения вторжений уровня узла</strong></h2>



<table class="wp-block-table"><tbody><tr><td><strong>Класс защиты</strong></td><td><strong>№&nbsp;сертификата - Система обнаружения вторжений уровня узла</strong></td></tr><tr><td>ИТ.СОВ.У<strong>1</strong>.ПЗ</td><td>отсутствуют</td></tr><tr><td>ИТ.СОВ.У<strong>2</strong>.ПЗ</td><td><strong>3856</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/%D1%80%D0%B5%D0%B1%D1%83%D1%81-%D1%81%D0%BE%D0%B2/">программный комплекс обнаружения вторжений Ребус-СОВ</a></td></tr><tr><td>ИТ.СОВ.У<strong>3</strong>.ПЗ</td><td>отсутствуют</td></tr><tr><td>ИТ.СОВ.У<strong>4</strong>.ПЗ</td><td><strong>2720</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/dallas-lock-8-0/">Система защиты информации от&nbsp;несанкционированного доступа Dallas Lock 8.0-K</a><br /><strong>2945</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/dallas-lock-8-0/">Система защиты информации от&nbsp;несанкционированного доступа Dallas Lock 8.0-С</a><br /><strong>3232</strong>&nbsp;-&nbsp;HP TrippingPoint (скорее всего речь о&nbsp;<a href="https://zlonov.ru/catalog/tippingpoint/">TippingPoint</a>)<br /><strong>3745</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/secret-net-studio/">cредство защиты информации Secret Net Studio</a><br /><strong>3802</strong>&nbsp;-&nbsp;<a href="https://zlonov.ru/catalog/vipnet-ids-hs/">система обнаружения вторжений ViPNet IDS HS</a></td></tr><tr><td>ИТ.СОВ.У<strong>5</strong>.ПЗ</td><td>отсутствуют</td></tr><tr><td>ИТ.СОВ.У<strong>6</strong>.ПЗ</td><td>отсутствуют</td></tr></tbody></table>



Сетевых СОВ представлено много (14 штук), есть как отчественные решения, так и зарубежные (правда, последние только 4 и 5 классов защиты). А вот СОВ уровня узла лишь 6 вариантов и все, кроме Ребус-СОВ (у него класс 2), имеют только 4 класс защиты.



Пожалуй, стоит обратить внимание ещё вот на какой момент (спасибо&nbsp;<a href="https://www.facebook.com/alexey.lukatsky">Алексею Лукацкому</a>&nbsp;за идею) - версия продукта, на которую выдан сертификат.



В случае с отечественными решениями, которые почти все в ином, отличном от сертифицированного виде не существуют и не продаются, это не так важно, а вот для зарубежных продуктов - дело совсем другое.



Так, если верить,&nbsp;<a href="http://www.trendmicro.com.ru/newsroom/pr/trend-micro-tipping-point-compliance-with-fstec-requirements/index.html">пресс-релизу Trend Micro</a>&nbsp;от июня 2017 года, сертификат 3232 выдан на "<em>программно-аппаратный комплекс Trend Micro TippingPoint серий N и NX с операционной системой TOS&nbsp;<strong>версия 3.9.0</strong>&nbsp;и системой управления Security Management System&nbsp;<strong>версия 4.5.0</strong></em>", что, согласно документу&nbsp;<a href="https://success.trendmicro.com/solution/TP000071914-TippingPoint-End-of-Life-EOL-dates">TippingPoint End of Life (EOL) dates</a>, означает, что данное сертифицированное решение хоть и не последней версии, но, по крайней мере, является поддерживаемым.



Нужно, правда, отметить, что в тексте пресс-релиза в отношении сертификата&nbsp;<strong>3232</strong>&nbsp;говорится о том, что он выдан на СОВ уровня сети, но в реестре ФСТЭК указано, что &nbsp;сертификат&nbsp;<strong>3232</strong>&nbsp;выдан для СОВ уровня узла (ИТ.СОВ.У4.ПЗ), да и вообще - на некий "HP T<strong>r</strong>ippingPoint".



Сертификат уровня сети на TippingPoint в реестре ФСТЭК всё же есть - это сертификат&nbsp;<strong>3481</strong>. Беда только в том, что (если верить реестру) сертификат 3481 выдан на "<em>программно-аппаратный комплекс HP TippingPoint серий N и NX с операционной системой TOS версия 3 и системой управления&nbsp;<strong>SMS версия 3</strong></em>", т.е. на&nbsp;<a href="https://success.trendmicro.com/solution/TP000071914-TippingPoint-End-of-Life-EOL-dates">устаревшую и неподдерживаемую с марта 2016</a>&nbsp;систему управления.



{% include one_image_new2.html picture_name="" picture_path="2018/2018-08-22-new-fstec-ips/Trend-Micro-NX-SMS.png" %}


Пресс-релиз и реестр ФСТЭК противоречат друг другу и можно было бы верить реестру, но в нём тоже есть ошибки: упомянутый T<strong>r</strong>ippingPoint или тот же САВ3.ИТ с цифрой 3 вместо буквы З (<a href="https://zlonov.ru/2018/07/new-fstec-av/">писал про него в июле</a>, пока так и не исправили). Оригиналы сертификатов ФСТЭК просит не публиковать, так что "<em>The Truth Is Out There</em>" (с)



У другого нероссийского вендора Check Point, к сожалению, сертифицирована версия (R77.10),&nbsp;<a href="https://www.checkpoint.com/support-services/support-life-cycle-policy/">официально снятая с поддержки год назад</a>.


{% include one_image_new2.html picture_name="" picture_path="2018/2018-08-22-new-fstec-ips/Check-Point-R77.10.png" %}


У ещё одного зарубежного производителя Fortinet сертифицирован "<em>программно-аппаратный комплекс «FortiGate», функционирующий под управлением операционной системы FortiOS 5.4.1</em>". Данная версия будет снята с инженерной поддержки в декабре 2018 года, а окончательно - только в 2020 году (информация из раздела Службы поддержки:&nbsp;<a href="https://support.fortinet.com/Information/ProductLifeCycle.aspx">Fortinet Life Cycle Information</a>, для доступа нужно иметь зарегистрированный аакаунт).


{% include one_image_new2.html picture_name="" picture_path="2018/2018-08-22-new-fstec-ips/FortiOS-5.4.png" %}


Наконец, у Cisco сертифицирована "<em>система обнаружения вторжений Cisco ASA FirePOWER версии 6.2</em>",&nbsp;<a href="https://www.cisco.com/c/en/us/td/docs/security/asa/compatibility/asamatrx.pdf">являющаяся актуальной</a>, что и понятно - сертификат был получен только в марте этого года.&nbsp;


{% include one_image_new2.html picture_name="" picture_path="2018/2018-08-22-new-fstec-ips/ASA-and-ASA-FirePOWER-Compatibility.png" %}


Кстати, в отчёте&nbsp;<a href="https://www.trendmicro.com/content/dam/trendmicro/global/en/business/campaign/nss-labs-ngips/nss-labs_ngips_comparative-report_svm.pdf">NSS Labs 2017 Security Value Map (SVM) for Next Generation Intrusion Prevention Systems (NGIPS)</a>&nbsp;от ноября прошлого года фигурируют такие модели и версии продуктов упомянутых производителей:



<ul><li>Check Point Software Technologies 15600&nbsp;<strong>R77.30</strong></li><li>Cisco FirePOWER 8350&nbsp;<strong>v6.2.0.1</strong></li><li>Fortinet FortiGate 600D&nbsp;<strong>v5.4.5</strong></li><li>Trend Micro 7500NX&nbsp;<strong>v3.9.2.4784</strong></li></ul>


{% include one_image_new2.html picture_name="" picture_path="2018/2018-08-22-new-fstec-ips/NSS-Labs-2017-Security-Value-Map-SVM-for-Next-Generation-Intrusion-Prevention-Systems-NGIPS.png" %}


Итоговая таблица по версиям неотечественных продуктов выглядит так (для Trend Micro требуется уточнение номера сертифицированной версии):



<table class="wp-block-table"><thead><tr><th><strong>ПРОИЗВОДИТЕЛЬ</strong></th><th><strong>СЕРТИФИЦИРОВАНО</strong></th><th><strong>СТАТУС</strong></th><th><strong>В ОТЧЁТЕ NSS LABS</strong></th><th><strong>ТЕКУЩАЯ ВЕРСИЯ</strong></th></tr></thead><tbody><tr><td>Check Point</td><td>R77.10</td><td>Снята с поддержки</td><td>R77.30</td><td>R80.10</td></tr><tr><td>Cisco</td><td>FirePOWER 6.2</td><td>Актуальна</td><td>FirePOWER 6.2.0.1</td><td>FirePOWER 6.2.3</td></tr><tr><td>Fortinet</td><td>5.4.1</td><td>Поддерживается</td><td>5.4.5</td><td>6.0</td></tr><tr><td>Trend Micro</td><td>NX 3*</td><td>Поддерживается*</td><td>NX 3.9.2.4784</td><td>NX 3.9.3</td></tr><tr><td>Trend Micro</td><td>SMS 3*</td><td>Снята с поддержки*</td><td>-</td><td>SMS 5.1.0</td></tr></tbody></table>



В качестве пожелания авторам и составителям реестра ФСТЭК отмечу, что было бы здорово в реестре видеть в явном виде сертифицированную версию продукта с детализацией хотя бы до одной цифры после точки для всех средств защиты информации.



Ну, и ошибок, которых, понятно, не избежать на 100%, хотелось бы поменьше.
