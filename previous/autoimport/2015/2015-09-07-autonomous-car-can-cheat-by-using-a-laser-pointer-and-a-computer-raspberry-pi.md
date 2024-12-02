---
layout: zlonov/old_post
title: (уязвимость) Автономный автомобиль можно обмануть, используя лазерную указку и компьютер Raspberry Pi
date: 2015-09-07 12:58
author: admin
category: autoimport
tags: [LIDAR, Raspberry Pi, автомобиль, Джонатан Петит, уязвимости, уязвимость]
---
Исследователь в области безопасности Джонатан Петит (Jonathan Petit) обнаружил, что оптические дальномеры (LIDAR), используемые в автономных автомобилях, легко могут быть введены в заблуждение с помощью простой установки, включающей маломощный лазер и контроллер, в качестве которого можно использовать, например, одноплатный компьютер Raspberry Pi. Установка формирует импульсы, которые LIDAR принимает за отражения от объектов. В результате у электроники, управляющей автономным автомобилем, создается ложное представление о наличии препятствий, таких как другие транспортные средства, стены и люди.

Необходимые импульсы хакер записал, используя серийный LIDAR IBEO Lux. Сложная часть, по его словам, заключается в том, чтобы синхронизировать сигналы от автономного автомобиля с «отражениями», воспроизводимыми установкой.

Лазерные дальномеры используются для обнаружения объектов на больших дистанциях. Как утверждает Петит, ему удавалось создать иллюзию присутствия машины, стены или пешехода на расстоянии от 20 до 350 метров до автономного автомобиля, причем технически нет сложности в формировании большого количества объектов и имитации их движения. Атака удавалась с расстояния до 100 метров, с разных направлений. Взломщик отмечает, что ему даже не приходилось точно нацеливаться на автономный автомобиль.

«Загрузив» систему автономного автомобиля большим количеством ложных объектов, можно лишить ее возможности следить за настоящими объектами. Исследование Петита, которое будет представлено на ноябрьской конференции по компьютерной безопасности Black Hat Europe, показывает, что создателям автономных автомобилей еще есть над чем поработать, прежде чем выпускать свои детища на дороги.
<p style="text-align: right;"><em><a href="http://www.ixbt.com/news/2015/09/07/avtonomnyj-avtomobil-mozhno-obmanut-ispolzuja-lazernuju-ukazku-i-kompjuter-raspberry-pi.html" target="_blank">Источник</a>
</em>
