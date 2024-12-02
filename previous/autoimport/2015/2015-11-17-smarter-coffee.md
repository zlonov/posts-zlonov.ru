---
layout: zlonov/old_post
title: (уязвимость) Исследователи признали небезопасной кофемашину Smarter Coffee
date: 2015-11-17 19:09
author: admin
category: autoimport
tags: [IoT, Pen Test Partners, Smarter, Wi-Fi, кофемашина, уязвимости]
---
Исследователи компании Pen Test Partners в конце октября <a href="https://xakep.ru/2015/10/20/ikettle/" data-jsbanchorprepared="sjVoGUEtKnpKg6f">рассказывали</a> о способе взлома Wi-Fi сетей через «умный» чайник iKettle, созданный компанией <a href="http://smarter.am/" data-jsbanchorprepared="1xI8raxcSnhJ9CZ">Smarter</a>. Теперь они обнаружили, что кофемашина Smarter Coffee, созданная тем же производителем, тоже представляет угрозу безопасности пользователей.

В данный момент исследователи Pen Test Partners <a href="https://www.pentestpartners.com/blog/hacking-a-wi-fi-coffee-machine-part-1/" data-jsbanchorprepared="7klRHAs1ZoVeBig">изучают</a> вторую модель чайников iKettle и кофеварки Smarter Coffee. Wi-Fi кофемашина компании Smarter, а также официальное мобильное приложение, оказались защищены не многим лучше многострадального чайника. Хотя изучение «умной» бытовой техники еще не закончено, по словам исследователей, кофемашина более чем уязвима.

Ненастроенная Smarter Coffee «из коробки» работает в режиме Wi-Fi access point. Для сравнения:  чайник iKettle функционировал как ad-hoc Wi-Fi девайс. Чайник также работал с портами TCP 23 и 2000, но кофеварка по этим портам не отвечает, вероятно, это объясняется тем, что кофемашина использует другой Wi-Fi модуль, отличный от VSD03 в чайниках. Тем не менее, исследователи обнаружили, что Smarter Coffee работает с портами TCP и UDP 2081, используя при этом простейший бинарный протокол. Устройство передает системное сообщение каждые пять секунд, оно содержит информацию о статусе кофеварки, включая уровень воды в резервуаре, число чашек и крепость кофе.

Равно как и чайник, кофемашина экономит драгоценные секунды пользователя, позволяя ему управлять устройством удаленно, через мобильное приложение. Изучив трафик, которым обмениваются кофеварка и приложение, исследователи выяснили, что Smarter Coffee оснащается модулем ESP8266. Данный модуль является одним из наиболее распространенных среди IoT-устройств (вероятно, потому что он очень дешев).

<a class="cboxElement" href="https://xakep.ru/wp-content/uploads/2015/11/coffee1-7.png" data-jsbanchorprepared="RAQpI8aMsVOrIRl"><img class="aligncenter size-full wp-image-83906" src="https://xakep.ru/wp-content/uploads/2015/11/coffee1-7.png" alt="coffee1-7" width="562" height="202" /></a>

Обладая этой информацией, исследователи сумели не только узнать многое о Wi-Fi сети, к которой подключена кофеварка (это всё же нельзя назвать проблемой с безопасностью), но и смогли перехватить контроль над устройством, отправив сигнал о том, что пора варить кофе.

<a class="cboxElement" href="https://xakep.ru/wp-content/uploads/2015/11/coffee1-8.png" data-jsbanchorprepared="xNyFQYcM1TvmXcM"><img class="aligncenter size-full wp-image-83907" src="https://xakep.ru/wp-content/uploads/2015/11/coffee1-8.png" alt="coffee1-8" width="258" height="385" /></a>

Также эксперты Pen Test Partners смогли удаленно спровоцировать устройство на обновление прошивки, что сделало кофемашину временно недоступной и привело к сбросу всех настроек до заводских. Более того, после этой процедуры кофеварка не вернется к нормальной работе без хард резета. Пользователю понадобится зажать кнопку «Start» и держать ее в таком положении 10 секунд. Учитывая, что пользователь вообще не понимает, что происходит, догадаться перезагрузить устройство, сумеет явно не каждый.

Pen Test Partners сейчас продолжают изучать процесс обновления ПО на Smarter Coffee. По словам исследователей, в прошивку ковефарки, скорее всего, возможно внедрить вредоносный код.

Директор Pen Test Partners Кэн Манро (Ken Munro) отмечает, что нормально настроенная кофеварка защищена куда лучше. Изданию The Register он <a href="http://www.theregister.co.uk/2015/11/16/icoffee_kit_hackable_smarter_ikettle/" data-jsbanchorprepared="4enSPRapFuygPfE">рассказал</a>: «Дело в том, что пока мы нашли уязвимость только в ненастроенных кофеварках. Да, мы осуществили вполне успешную атаку, но это не такая убийственная штука, как кража Wi-Fi PSK, которую мы провернули с iKettle… пока что. Здесь требуется изучить еще множество векторов атак, просто для этого нам понадобится больше времени».

<p style="text-align: right;"><em><a href="https://xakep.ru/2015/11/17/smarter-coffee/" target="_blank">Источник</a></em>
