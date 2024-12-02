---
layout: zlonov/old_post
title: (уязвимость) Терминалы Siemens SIPROTEC подвержены уязвимости отказа в обслуживании
date: 2016-01-12 15:06
author: admin
category: autoimport
tags: [Siemens, SIPROTEC, отказ в обслуживании, уязвимости]
---
<em>Устройство возможно вывести из строя путем отправки специально сформированных пакетов на UDP-порт 50000.</em>

Терминалы Siemens серии SIPROTEC 4 и SIPROTEC Compact с коммуникационным модулем EN100 версии 4.24 и ниже подвержены <a href="http://www.securitylab.ru/vulnerability/478357.php" target="_blank">уязвимости</a> отказа в обслуживании. Об этом сообщается на сайте компании.

Эксплуатация уязвимости осуществляется за счет передачи на терминалы с установленными уязвимыми прошивками модуля специально сформированных пакетов на UDP-порт 50000. В случае успешной атаки устройство будет выведено из строя, а для восстановления работоспособности терминала потребуется перезагрузка.

Ошибка была устранена в обновлении прошивки EN100 версии 4.25. Исправление также повышает стабильность работы устройства в условиях приема большого количества запросов ARP.

Проверить версию ПО модуля EN100 можно с помощью браузера, перейдя по адресу http://IP_устройства/home. Для установки обновления понадобится посетить официальный сайт Siemens.

<a href="http://www.securitylab.ru/news/478354.php" target="_blank">Источник</a>
