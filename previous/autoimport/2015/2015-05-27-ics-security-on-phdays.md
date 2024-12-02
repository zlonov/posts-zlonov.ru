---
layout: zlonov/old_post
title: ИБ АСУ ТП на PHDays
date: 2015-05-27 18:15
author: admin
category: autoimport
tags: [DATAPK, Positive Technologies, SCADA, ИБ АСУ ТП, информационная безопасность, Лаборатория Касперского, мероприятие, УЦСБ]
---
Тема информационной безопасности промышленных систем автоматизации не была центральной на Positive Hack Days, но в ряду других была представлена достаточно широко, хотя и концентрировалась преимущественно в первом дне мероприятия.

Начну с того, что всем желающим предлагалось взломать электрическую подстанцию в рамках конкурса <a href="http://www.phdays.ru/program/contests/#40924" target="_blank">Digital Substation Takeover</a>. На стенде были представлены реальные коммутаторы, сервера, контроллеры и устройства релейной защиты, поэтому выглядел он внушительно. По комментариям представителей отрасли электроэнергетики <em>хакеры</em>, сидящие на пуфиках и <em>ломающие</em> реальное оборудование, впечатление производят. При этом, к слову, по замыслу организаторов, одной из задач было продемонстрировать то, что для взлома промышленных систем вовсе не обязательно хорошо представлять себе, как они на самом деле работают.

[caption id="attachment_6624" align="aligncenter" width="500"]<a href="/assets/uploads/Digital-Substation-Takeover-на-PHDays.jpg"><img class="wp-image-6624" src="/assets/uploads/Digital-Substation-Takeover-на-PHDays-1024x587.jpg" alt="Digital Substation Takeover на PHDays" width="500" height="287" /></a> Digital Substation Takeover на PHDays[/caption]

Из докладов, затрагивающих тематику безопасности АСУ ТП, центральным я бы назвал выступление Андрея Духвалова "<em><a href="http://www.phdays.ru/program/business/40976/" target="_blank">Технологии защиты непрерывности процесса управления АСУ ТП</a></em>". Речь шла об основных отличиях промышленных и ИТ сетей, была приведена статистика и примеры задокументированных инцидентов. В заключение Андрей предложил основные подходы к защите узлов сети АСУ ТП и сетевых взаимодействий между ними. Некоторые слайды из презентации ниже на фотографиях экрана (пока, к сожалению, в таком качестве, презентации ещё не выложены).

<table>
<tbody>
<tr>
<td>

[caption id="attachment_6627" align="aligncenter" width="300"]<a href="/assets/uploads/Отличия-АСУ-ТП-от-корпоративных-IT-сетей.jpg"><img class="size-medium wp-image-6627" src="/assets/uploads/Отличия-АСУ-ТП-от-корпоративных-IT-сетей-300x196.jpg" alt="Отличия АСУ ТП от корпоративных IT сетей" width="300" height="196" /></a> Отличия АСУ ТП от корпоративных IT сетей[/caption]</td>
<td>

[caption id="attachment_6628" align="aligncenter" width="300"]<a href="/assets/uploads/Конфиденциальность-или-непрерывность-в-промышленных-и-корпоративных-сетях.jpg"><img class="size-medium wp-image-6628" src="/assets/uploads/Конфиденциальность-или-непрерывность-в-промышленных-и-корпоративных-сетях-300x192.jpg" alt="Конфиденциальность или непрерывность в промышленных и корпоративных сетях" width="300" height="192" /></a> Конфиденциальность или непрерывность в промышленных и корпоративных сетях[/caption]</td>
</tr>
<tr>
<td>

[caption id="attachment_6629" align="aligncenter" width="300"]<a href="/assets/uploads/Состояние-ИБ-АСУ-ТП-по-статистике-Лаборатории-Касперского.jpg"><img class="size-medium wp-image-6629" src="/assets/uploads/Состояние-ИБ-АСУ-ТП-по-статистике-Лаборатории-Касперского-300x228.jpg" alt="Состояние ИБ АСУ ТП по статистике Лаборатории Касперского" width="300" height="228" /></a> Состояние ИБ АСУ ТП по статистике Лаборатории Касперского[/caption]</td>
<td>

[caption id="attachment_6630" align="aligncenter" width="300"]<a href="/assets/uploads/Краткая-статистика-по-ИБ-АСУ-ТП-от-ICS-CERT.jpg"><img class="size-medium wp-image-6630" src="/assets/uploads/Краткая-статистика-по-ИБ-АСУ-ТП-от-ICS-CERT-300x229.jpg" alt="Краткая статистика по ИБ АСУ ТП от ICS-CERT" width="300" height="229" /></a> Краткая статистика по ИБ АСУ ТП от ICS-CERT[/caption]</td>
</tr>
<tr>
<td>

[caption id="attachment_6631" align="aligncenter" width="300"]<a href="/assets/uploads/Инциденты-в-ИБ-АСУ-ТП.jpg"><img class="size-medium wp-image-6631" src="/assets/uploads/Инциденты-в-ИБ-АСУ-ТП-300x227.jpg" alt="Инциденты в ИБ АСУ ТП" width="300" height="227" /></a> Инциденты в ИБ АСУ ТП[/caption]</td>
<td>

[caption id="attachment_6632" align="aligncenter" width="300"]<a href="/assets/uploads/Мифы-об-IT-безопасности-в-АСУ-ТП.jpg"><img class="size-medium wp-image-6632" src="/assets/uploads/Мифы-об-IT-безопасности-в-АСУ-ТП-300x228.jpg" alt="Мифы об IT-безопасности в АСУ ТП" width="300" height="228" /></a> Мифы об IT-безопасности в АСУ ТП[/caption]</td>
</tr>
<tr>
<td>

[caption id="attachment_6633" align="aligncenter" width="300"]<a href="/assets/uploads/Скрытность-атак-в-АСУ-ТП.jpg"><img class="size-medium wp-image-6633" src="/assets/uploads/Скрытность-атак-в-АСУ-ТП-300x192.jpg" alt="Скрытность атак в АСУ ТП" width="300" height="192" /></a> Скрытность атак в АСУ ТП[/caption]</td>
<td>

[caption id="attachment_6634" align="aligncenter" width="300"]<a href="/assets/uploads/Способы-защиты-для-узлов-сети-АСУ-ТП.jpg"><img class="size-medium wp-image-6634" src="/assets/uploads/Способы-защиты-для-узлов-сети-АСУ-ТП-300x201.jpg" alt="Способы защиты для узлов сети АСУ ТП" width="300" height="201" /></a> Способы защиты для узлов сети АСУ ТП[/caption]</td>
</tr>
<tr>
<td>

[caption id="attachment_6635" align="aligncenter" width="300"]<a href="/assets/uploads/Способы-защиты-для-сетевого-взаимодействия-в-АСУ-ТП.jpg"><img class="size-medium wp-image-6635" src="/assets/uploads/Способы-защиты-для-сетевого-взаимодействия-в-АСУ-ТП-300x226.jpg" alt="Способы защиты для сетевого взаимодействия в АСУ ТП" width="300" height="226" /></a> Способы защиты для сетевого взаимодействия в АСУ ТП[/caption]</td>
<td>

[caption id="attachment_6640" align="aligncenter" width="300"]<a href="/assets/uploads/Сервисы-для-обеспечения-непрерывности-процесса-управления.jpg"><img class="size-medium wp-image-6640" src="/assets/uploads/Сервисы-для-обеспечения-непрерывности-процесса-управления-300x224.jpg" alt="Сервисы для обеспечения непрерывности процесса управления" width="300" height="224" /></a> Сервисы для обеспечения непрерывности процесса управления[/caption]</td>
</tr>
</tbody>
</table>

Мне понравился тезис о том, что атаки в промышленных сетях не бывают мгновенными, а развиваются даже медленнее, чем в классических офисных сетях. При этом за счёт постоянного мониторинга такие атаки можно обнаружить и предотвратить на самых ранних этапах. Чем ещё хорош мониторинг, так это тем, что в отличие от решений по предотвращению никакого воздействия на технологические процессы при этом не оказывается. Ровно такой подход, кстати, используется УЦСБ в концепции комплекса оперативного мониторинга и контроля защищенности АСУ ТП - <a href="http://www.slideshare.net/zlonov/datapk" target="_blank">DATAPK</a> и возник он (подход) исключительно из практики и на основе наработанного опыта.

Доклад Константина Каманина "<a href="http://www.phdays.ru/program/business/40975/" target="_blank"><em>Портфель решений «Лаборатории Касперского» для защиты АСУ ТП</em></a>" был не столько про продукты, сколько именно что про решения - связку продуктов и услуг. Такой подход понятен, ведь в силу общей недостаточной проработанности тематики и большого числа вариативности технологических процессов предложить <em>решение-из-коробки</em> для ИБ АСУ ТП пока без предварительного аудита/обследования сложно.

<table>
<tbody>
<tr>
<td>

[caption id="attachment_6642" align="aligncenter" width="300"]<a href="/assets/uploads/Секторы-критически-важной-инфраструктуры.jpg"><img class="size-medium wp-image-6642" src="/assets/uploads/Секторы-критически-важной-инфраструктуры-300x171.jpg" alt="Секторы критически важной инфраструктуры" width="300" height="171" /></a> Секторы критически важной инфраструктуры[/caption]</td>
<td>

[caption id="attachment_6643" align="aligncenter" width="300"]<a href="/assets/uploads/Атакующие-и-защищающиеся-в-ИБ-АСУ-ТП.jpg"><img class="size-medium wp-image-6643" src="/assets/uploads/Атакующие-и-защищающиеся-в-ИБ-АСУ-ТП-300x167.jpg" alt="Атакующие и защищающиеся в ИБ АСУ ТП" width="300" height="167" /></a> Атакующие и защищающиеся в ИБ АСУ ТП[/caption]</td>
</tr>
<tr>
<td>

[caption id="attachment_6644" align="aligncenter" width="300"]<a href="/assets/uploads/Причины-уязвимости-промышленных-систем.jpg"><img class="size-medium wp-image-6644" src="/assets/uploads/Причины-уязвимости-промышленных-систем-300x168.jpg" alt="Причины уязвимости промышленных систем" width="300" height="168" /></a> Причины уязвимости промышленных систем[/caption]</td>
<td>

[caption id="attachment_6645" align="aligncenter" width="300"]<a href="/assets/uploads/Трудности-в-защите-КВО.jpg"><img class="size-medium wp-image-6645" src="/assets/uploads/Трудности-в-защите-КВО-300x189.jpg" alt="Трудности в защите КВО" width="300" height="189" /></a> Трудности в защите КВО[/caption]</td>
</tr>
<tr>
<td>

[caption id="attachment_6646" align="aligncenter" width="300"]<a href="/assets/uploads/Угрозы-верхнего-уровня-SCADA-систем.jpg"><img class="size-medium wp-image-6646" src="/assets/uploads/Угрозы-верхнего-уровня-SCADA-систем-300x164.jpg" alt="Угрозы верхнего уровня SCADA систем" width="300" height="164" /></a> Угрозы верхнего уровня SCADA систем[/caption]</td>
<td>

[caption id="attachment_6647" align="aligncenter" width="300"]<a href="/assets/uploads/Угрозы-нижнего-уровня-SCADA-систем.jpg"><img class="size-medium wp-image-6647" src="/assets/uploads/Угрозы-нижнего-уровня-SCADA-систем-300x144.jpg" alt="Угрозы нижнего уровня SCADA систем" width="300" height="144" /></a> Угрозы нижнего уровня SCADA систем[/caption]</td>
</tr>
</tbody>
</table>

Посмотреть продукт Kaspersky TMS можно было на их стенде с макетом деревообрабатывающего завода. Про <a href="http://www.kaspersky.ru/news?id=207734159" target="_blank">ЩИТ и совместные разработки</a>, кстати, уже не упоминают, но никто особо и не спрашивает.

[caption id="attachment_6650" align="aligncenter" width="500"]<a href="/assets/uploads/Макет-деревообрабатывающего-завода-для-демонстрации-подхода-к-ИБ-АСУ-ТП.jpg"><img class="wp-image-6650" src="/assets/uploads/Макет-деревообрабатывающего-завода-для-демонстрации-подхода-к-ИБ-АСУ-ТП-1024x932.jpg" alt="Макет деревообрабатывающего завода для демонстрации подхода к ИБ АСУ ТП" width="500" height="455" /></a> Макет деревообрабатывающего завода для демонстрации подхода к ИБ АСУ ТП[/caption]

Интересный доклад был от Марины Кротофил: "<a href="http://www.phdays.ru/program/tech/40605/"><em>Этот чертов уязвимый химический процесс</em></a>". На примере химического завода она наглядно показала, что чем лучше хакер понимает суть технологического процесса, тем больший экономический ущерб он может нанести. Выведенное из строя оборудование быстро обнаружат и заменят, а вот изменённый режим функционирования, ухудшающий качество или количество продукции на выходе, может оставаться незамеченным достаточно долго, нанося ущерб ежедневно.

[caption id="attachment_6658" align="aligncenter" width="500"]<a href="/assets/uploads/Потенциальные-последствия-от-реализации-атак-на-АСУ-ТП.png"><img class="wp-image-6658" src="/assets/uploads/Потенциальные-последствия-от-реализации-атак-на-АСУ-ТП-1024x770.png" alt="Потенциальные последствия от реализации атак на АСУ ТП" width="500" height="376" /></a> Потенциальные последствия от реализации атак на АСУ ТП[/caption]

Тематика безопасности АСУ ТП затрагивалась и в рамках других докладов. Вот например, статистика от представителей Positive Technologies.

<table>
<tbody>
<tr>
<td>

[caption id="attachment_6651" align="aligncenter" width="300"]<a href="/assets/uploads/Доступные-из-Интернет-слева-и-уязвимые-среди-них-справа-компоненты-АСУ-ТП.png"><img class="size-medium wp-image-6651" src="/assets/uploads/Доступные-из-Интернет-слева-и-уязвимые-среди-них-справа-компоненты-АСУ-ТП-300x144.png" alt="Доступные из Интернет (слева) и уязвимые среди них (справа) компоненты АСУ ТП" width="300" height="144" /></a> Доступные из Интернет (слева) и уязвимые среди них (справа) компоненты АСУ ТП[/caption]</td>
<td>

[caption id="attachment_6652" align="aligncenter" width="300"]<a href="/assets/uploads/Рост-числа-выявляемых-уязвимостей-в-АСУ-ТП-и-скорость-их-закрытия.png"><img class="size-medium wp-image-6652" src="/assets/uploads/Рост-числа-выявляемых-уязвимостей-в-АСУ-ТП-и-скорость-их-закрытия-300x158.png" alt="Рост числа выявляемых уязвимостей в АСУ ТП и скорость их закрытия" width="300" height="158" /></a> Рост числа выявляемых уязвимостей в АСУ ТП и скорость их закрытия[/caption]</td>
</tr>
</tbody>
</table>

Можно ещё почитать впечатления от PHDays (<a href="http://www.rosint.net/content/2/502/" target="_blank">первый день</a>) Сергея Борисова.

Про другие ближайшие мероприятия по теме ИБ АСУ ТП писал <a href="https://zlonov.ru/2015/05/ics-security-upcoming-events/" target="_blank">здесь</a>.
