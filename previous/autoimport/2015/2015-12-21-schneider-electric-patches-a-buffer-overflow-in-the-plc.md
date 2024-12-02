---
layout: zlonov/old_post
title: (уязвимость) Schneider Electric патчит переполнение буфера в PLC
date: 2015-12-21 20:09
author: admin
category: autoimport
tags: [CyberX, ICS-CERT, Modicon, Modicon M340 PLC, Schneider Electric, водоснабжение, Нир Гиллер, промышленное производство, транспорт, уязвимости, уязвимость, электроэнергетика, энергетика]
---
На прошлой неделе компания Schneider Electric, разработчик систем автоматизации управления энергетическими объектами, устранила уязвимость, чреватую взломом ряда программируемых контроллеров.

Данная уязвимость связана с переполнением буфера и актуальна для тринадцати продуктов линейки Modicon M340 PLC. Ее эксплойт позволяет вывести устройство из строя или удаленно выполнить код.

Согласно <a href="https://ics-cert.us-cert.gov/advisories/ICSA-15-351-01" target="_blank">бюллетеню ICS-CERT</a>, уязвимости подвержены контроллеры Schneider следующих сборок:

<ul>
    <li>BMXNOC0401,</li>
    <li>BMXNOE0100,</li>
    <li>BMXNOE0100H,</li>
    <li>BMXNOE0110,</li>
    <li>BMXNOE0110H,</li>
    <li>BMXNOR0200,</li>
    <li>BMXNOR0200H,</li>
    <li>BMXP342020,</li>
    <li>BMXP342020H,</li>
    <li>BMXP342030,</li>
    <li>BMXP3420302,</li>
    <li>BMXP3420302H,</li>
    <li>BMXPRA0100.</li>
</ul>

В минувший четверг были пропатчены первые пять продуктов; новая прошивка для BMXNOR0200 (H), BMXP342020, BMXP3420302 и BMXPRA0100 будет выпущена 16 января.

Schneider позиционирует Modicon M340 как программируемые контроллеры среднего класса; эти продукты широко используются в таких отраслях, как промышленное производство, транспортные перевозки, электроэнергетика и водоснабжение.

Уязвимость в продуктах Schneider обнаружил Нир Гиллер (Nir Giller), технический директор израильской компании CyberX, специализирующейся на поиске багов в платформах АСУ ТП. Ранее Гиллер нашел ряд багов в программируемых контроллерах производства Rockwell Automation, в том числе <a href="https://threatpost.com/rockwell-patches-serious-frostyurl-plc-vulnerability/115196/" target="_blank">уязвимость FrostyURL</a>. Все эти бреши были пропатчены в конце октября.

<p style="text-align: right;"><em><a href="https://threatpost.ru/schneider-electric-patches-buffer-overflow-in-plc-line/13918/" target="_blank">Источник</a></em>
