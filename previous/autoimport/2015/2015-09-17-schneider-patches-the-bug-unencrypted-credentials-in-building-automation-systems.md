---
layout: zlonov/old_post
title: (уязвимость) Schneider патчит баг незашифрованных учетных данных в системах автоматизации зданий
date: 2015-09-17 08:46
author: admin
category: autoimport
tags: [ICS-CERT, StruxureWare Building Expert, Sсhneider Electric, автоматизация зданий, Артем Курбатов, уязвимости, уязвимость]
---
<div id="Y/SOKe0yMAmbfA7fBxY0g9YwK/QqaU7ukANkbYFpMyA=_14fdc154098:b373bc8:fccac72e_entryBody" class="entryBody" title="">
<div id="Y/SOKe0yMAmbfA7fBxY0g9YwK/QqaU7ukANkbYFpMyA=_14fdc154098:b373bc8:fccac72e_entryContent" class="content">

Известный производитель автоматизированных систем управления — компания Sсhneider Electric опубликовала новую прошивку для своей системы автоматизации зданий StruxureWare Building Expert, в которой закрыта уязвимость, эксплуатируемая удаленно.

Исследователь Артем Курбатов обнаружил, что система передает учетные данные пользователя между сервером и клиентом в открытом (незашифрованном) виде. В <a href="https://ics-cert.us-cert.gov/advisories/ICSA-15-258-01" target="_blank">оповещении</a> от ICS-CERT говорится, что данная уязвимость не была эксплуатирована гласно.

«Успешный эксплойт позволит злоумышленнику получить учетные данные пользователя», — пишет Schneider в своем <a href="http://download.schneider-electric.com/files?p_Reference=SEVD-2015-254-01&amp;p_EnDocType=Brochure&amp;p_File_Id=1079944536&amp;p_File_Name=SEVD-2015-254-01.pdf" target="_blank">оповещении.</a>

По данным Schneider Electric, эта система автоматизации зданий используется во всем мире, по большей части в коммерческих зданиях. StruxureWare Building Expert описывается как <a href="http://www2.schneider-electric.com/sites/corporate/en/solutions/struxureware/applications/building-expert.page" target="_blank">многоцелевое устройство управления</a>, которое отслеживает работу систем вентиляции, отопления и кондиционирования, систем освещения и измерительных систем, прежде всего для контроля за расходом энергии. Уязвимость содержат версии до 2.15, по данным ICS-CERT, причем уязвимость получила CVSS-балл 10.0.

Менеджерам следует обновить MPM до версии <a href="https://buildingsdownloads.schneider-electric.com/documents/10807/250220/MPM+Series+-+Installation+Sheet/6b83cb2c-6d93-4e41-9902-2d8e13936727" target="_blank">2.15 или выше.</a>

Schneider Electric вплотную занялась закрытием дыр в безопасности с начала осени. 3 сентября компания выпустила <a href="https://ics-cert.us-cert.gov/advisories/ICSA-15-246-02" target="_blank">оповещение</a>, в котором говорится о закрытии ряда уязвимостей в Modicon M340 PLC Station P34. Об этих уязвимостях сообщил исследователь Хуан Франсиско Боливар (Juan Francisco Bolivar), также в июле о них сообщил и рассказал на конференции DEF CON независимый исследователь Адитья К. Соод (Aditya K. Sood).

Продукты Modicon BMXNOC0401, BMXNOE0100, BMXNOE0110, BMXNOE0110H, BMXNOR0200H, BMXP342020, BMXP342020H, BMXP342030, BMXP3420302, BMXP3420302H и BMXP342030H содержали уязвимости, с помощью которых можно было заставить браузер <a href="https://threatpost.ru/risky-schneider-electric-scada-vulnerabilities-remain-unpatched/10945/" target="_blank">перенаправлять пользователя на удаленный файл или исполняемый JavaScript</a>, хранящийся удаленно.
<p style="text-align: right;"><sub><em><a href="https://threatpost.ru/schneider-patches-plaintext-credentials-bug-in-building-automation-system/11845/" target="_blank">Источник</a></em></sub>

</div>
</div>
<div></div>
<div id="Y/SOKe0yMAmbfA7fBxY0g9YwK/QqaU7ukANkbYFpMyA=_14fdc154098:b373bc8:fccac72e_wallHolder"></div>
