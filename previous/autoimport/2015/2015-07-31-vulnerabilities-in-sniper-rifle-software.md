---
layout: zlonov/old_post
title: (уязвимость) Уязвимости в ПО снайперских винтовок позволяет изменить цель поражения
date: 2015-07-31 10:42
author: admin
category: autoimport
tags: [Michael Auger, Runa Sandvik, TrackingPoint, вооружение, Майкл Огер, оружие, Руна Сэндвик, снайперская винтовка, уязвимости]
---
Исследователи безопасности Руна Сэндвик (Runa Sandvik) и Майкл Огер (Michael Auger) заявили о том, что им удалось успешно проэксплуатировать уязвимости в самонаводящихся снайперских винтовках TrackingPoint.

Эксперты опубликовали видео, в котором продемонстрировали, как с помощью брешей в программном обеспечении оружия им удалось скомпрометировать его через Wi-Fi.

Как показано в видеоролике, оснащенная компьютером самонаводящаяся снайперская винтовка дальнего действия, стоимость которой составляет $13 тыс. за штуку, позволяет выстрелить только в случае, если ее ствол находится на одной линии с целью, гарантируя высокую точность попадания даже малоопытным стрелкам.

Сэндвик и Огер провели реверс-инжиниринг прицела, аппаратного обеспечения и трех сопутствующих мобильных приложений. Им удалось найти способ подключиться к компьютеру винтовки и изменить значения таким образом, чтобы их вмешательство не отображалось на ее экране. Далее исследователи загрузили неверные данные о весе пули, поэтому при определении, когда нужно произвести выстрел, прицел сбивается.

Наихудший сценарий, считают эксперты, заключается в том, что злоумышленники могут изменить настройки винтовки таким образом, что она начнет действовать нетипичным для себя образом.

<div style="margin-bottom: 5px; text-align: center;"><iframe src="https://www.youtube.com/embed/BJPCYdjrNWs?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe></div>
<p style="text-align: right;"><sub><em><a href="http://www.securitylab.ru/news/473939.php" target="_blank">Источник</a></em></sub>