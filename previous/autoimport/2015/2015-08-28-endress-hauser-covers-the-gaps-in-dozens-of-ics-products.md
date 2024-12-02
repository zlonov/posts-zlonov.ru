---
layout: zlonov/old_post
title: (уязвимость) Endress+Hauser закрывает бреши в десятках ICS-продуктов
date: 2015-08-28 16:38
author: admin
category: autoimport
tags: [CodeWrights, Digital Security, Endress+Hauser, HART, ICS-CERT, Александр Большев, Светлана Черкасова, уязвимости, уязвимость, эксплойт]
---
Критическая уязвимость, доступная удаленно и приводящая к полному зависанию системы, присутствует в библиотеке Device Type Manager, используемой многими АСУ ТП немецкой компании Endress+Hauser. Продукция компании используется многими компаниями, относящимися к секторам критической инфраструктуры. Библиотека DTM разработана другой компанией, CodeWrights, выпустившей новую версию, в которой брешь была устранена.

«Александр Большев и Светлана Черкасова из Digital Security обнаружили уязвимость, вызванную некорректной обработкой входящих данных и присутствующую в библиотеке HART Device Type Manager (DTM), разрабатываемой компанией CodeWrights GmbH и используемой в HART-оборудовании Endress+Hauser, — говорится в <a href="https://ics-cert.us-cert.gov/advisories/ICSA-15-237-01" target="_blank">бюллетене</a> ICS-CERT. — Уязвимость способна приводить к переполнению буфера с последующим сбоем в работе базового FDT-приложения (Field Device Tool). Для восстановления штатной работы системы требуется перезагрузка базового приложения. Базовое приложение используется в основном для проведения удаленной настройки. Эксплойт этой уязвимости не приводит к утере информации или контроля над системой, использующей HART-устройства на базе петель уровня 4—20 мА».

Для эксплойта уязвимости атакующему понадобится послать специально созданный пакет на уязвимое устройство, однако в бюллетене ICS-CERT говорится, что разработка рабочего эксплойта будет весьма затруднительна.

«Это достаточно сложная уязвимость. Разработать для нее рабочий эксплойт будет нелегкой задачей. Для эксплойта понадобится получить доступ к каналу, по которому пакеты передаются приложению. К тому же для того, чтобы привести к сбою в работе приложения, потребуются четко согласованные по времени действия. Все эти факторы делают эксплойт уязвимости крайне сложным», — говорится в бюллетене.

Endress+Hauser выпустила программное обновление для своей продукции, которое ее клиенты могут скачать с <a href="https://portal.endress.com/webdownload/FieldCareDownloadGui/" target="_blank">веб-сайта</a> компании.
<p style="text-align: right;"><sub><em><a href="https://threatpost.ru/endresshauser-patches-buffer-overflow-in-dozens-of-ics-products/11231/" target="_blank">Источник</a></em></sub>
