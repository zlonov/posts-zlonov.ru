---
layout: zlonov/old_post
title: (уязвимость) В продуктах Siemens RUGGEDCOM обнаружены множественные уязвимости
date: 2015-12-23 00:09
author: admin
category: autoimport
tags: [NTP, ntpd, POODLE, ROX I, ROX II, RuggedCom, Siemens, уязвимости, уязвимость]
---
<strong>Уязвимости вызваны использованием устаревшей версии протокола NTP.</strong>

Промышленные устройства Siemens RUGGEDCOM оказались подвержены множественным уязвимостям, существующим из-за использования устаревшей версии ntpd.

Уязвимостям подвержены все устройства под управлением операционных систем ROX I (все версии) и ROX II (до версии 2.9.0). Успешная эксплуатация требует использования NTP с ресурса ntp.org для синхронизации времени.

Одна из уязвимостей (CVE-2015-7871) позволяет удаленному пользователю обойти аутентификацию. Отправив специально сформированные пакеты UDP, злоумышленник вынудит демон NTP принимать обновления времени со сторонних серверов. Другая ошибка (CVE-2015-7855) позволяет вызвать аварийное завершение работы ntpd путем отправки специально сформированных пакетов NTP.

В устройствах RUGGEDCOM также обнаружены две уязвимости, позволяющие модифицировать дату и время (CVE-2015-7704), а также предотвратить получение корректного времени (CVE-2015-5300). Операционная система ROX II также была подвержена уязвимости POODLE.

Для устройств под управлением ОС ROX II было выпущено исправление, устраняющее вышеуказанные ошибки.

<p style="text-align: right;"><em><a href="http://www.securitylab.ru/news/477910.php" target="_blank">Источник</a></em>