---
layout: zlonov/old_post
title: WiFi, модемы, TeamViewer и прочие ужасы ИБ АСУ ТП
date: 2016-04-27 13:57
author: admin
category: autoimport
tags: [ICS-CERT, ICS-CERT Monitor, TeamViewer, WiFi, аудит, ИБ АСУ ТП, информационная безопасность, инцидент, модем, пароль, УЦСБ]
---
В начале года Команда экстренного реагирования на киберугрозы промышленных систем управления ICS-CERT (Industrial Control Systems Cybersecurity Emergency Response Team) в своём <a href="https://ics-cert.us-cert.gov/sites/default/files/Monitors/ICS-CERT_Monitor_Jan-Feb2016.pdf">отчёте за Январь-Февраль 2016</a> опубликовала интересную короткую заметку о показательном инциденте в некоторой неназванной организации, управляющей несколькими промышленными объектами. Соответствующей новости на русском языке не встречал, поэтому кратко передам суть произошедшего.

В ICS-CERT обратились представители организации, владеющей несколькими объектами из сферы энергетики и водоснабжения с подозрениями на проникновение в их сеть. Специалисты ICS-CERT, приехав на место и выполнив мониторинг сетевого трафика, обнаружили вредоносное программное обеспечение в сети объекта водоснабжения. Дальнейшее обследование выявило беспроводной маршрутизатор с прямым подключением к сети управления, хотя предполагалось, что такого доступа у него быть не должно.

Ещё одной находкой стал сотовый модем, подключенный к центральному переключателю (выключателю?) воды. Не сразу, но выяснилось, что данный модем использовался вендором для организации удалённого подключения. При этом аутентификация проводилась с использованием крайне простых логина и пароля.

Наконец, в трафике были обнаружены сессии ПО для удалённого управления рабочими станциями TeamViewer, при чём для достаточно критических рабочих мест.

Более подробных деталей ICS-CERT не раскрывает, но с точки зрения сути выявленных в ходе этого экспресс-аудита ИБ АСУ ТП нарушений случай получился достаточно типовым и показательным: неконтролируемые беспроводные сети и несанкционированный удалённый доступ - действительно часто встречающиеся<i> </i>проблемы с точки зрения обеспечения информационной безопасности АСУ ТП.

Например, в ходе недавнего <a href="https://www.youtube.com/watch?v=Au8p3ICtWgc&amp;list=PLr6gcpE7CNuFxLEmVpzRwRExmlHjnlMoT&amp;index=5">вебинара</a> по решениям Cisco для кибербезопасности промышленных систем автоматизации и управления Алексей Лукацкий рассказал, как в ходе семинара во Владивостоке (сам рассказ <a href="https://www.youtube.com/watch?v=Au8p3ICtWgc&amp;feature=youtu.be&amp;t=1h13m04s">на 1:13:04</a>) на одном из гидротехнических сооружений случайно была обнаружена беспроводная сеть, несмотря на полный запрет WiFi внутри контролируемой зоны. Выяснилось, что инженер АСУ ТП, чтобы не ходить по несколько раз в день по дамбе и не отслеживать работоспособность всех устройств (особенно в плохую погоду), поставил в центре дамбы точку доступа, завёл на неё исполнительные устройства и снимал с них информацию, не выходя из диспетчерской. При этом радиус действия точки доступа выходил за пределы контролируемой зоны.

<a name="audit"></a> Ещё о некоторых выявляемых при аудите ИБ АСУ ТП типичных проблемах говорилось на прошедшем CISO FORUM 2016 в ходе совместного мастер-класса Романа Попова, начальника отдела по информационной безопасности Э.ОН Россия и Антона Ёркина, руководителя аналитического направления УЦСБ (полностью презентация доступна <a href="http://www.slideshare.net/USSCru/ics-security-audit-eon-and-ussc">здесь</a>):

<ul>
    <li>Уязвимости в ПО, например:
<ul>
    <li>Зависание ПЛК вследствие некорректной обработки запросов на TCP-соединения;</li>
    <li>Уязвимость в реализации сетевого протокола FLEET (QNX) приводит к аварийной перезагрузке;</li>
</ul>
</li>
    <li>Неиспользуемое ПО;</li>
    <li>Простые пароли, пароли по умолчанию и пароли, хранящиеся в легко доступных местах;</li>
    <li>Отсутствие базовых настроек безопасности;</li>
    <li>«Дырки» в периметре АСУ ТП, например:
<ul>
    <li>Удаленный доступ в АСУ ТП с АРМ наладчика;</li>
</ul>
</li>
    <li>«Слабые» механизмы безопасности в АСУ ТП.</li>
</ul>

В ближайшее время должна выйти моя статья в журнале «Connect. Мир информационных технологий» под названием "<a href="https://zlonov.ru/2016/05/why-to-audit/"><em>Пять причин провести аудит информационной безопасности АСУ ТП в этом году</em></a>", вернусь к этой теме ещё раз.

В заключение же приведу оригинал статьи ICS-CERT на английском языке.

<blockquote><em>ICS-CERT recently worked with an industrial control system asset owner following a report of possible intrusion activity targeting the entity’s network. The asset owner operates in the power and water sectors, providing both power and water to their local community.</em>

<em>The company was receptive to working with ICS-CERT and ultimately requested that ICS-CERT come onsite to gather data and attempt to discover compromises on their network. ICS-CERT held a conference call with the entity to plan onsite incident response actions, request technical information, and establish expectations. On the call, ICS-CERT learned that the asset owner was in the process of merging its power and water networks, which had previously operated independently.</em>

<em>When the ICS-CERT incident response team arrived onsite, they first met with network engineers and top executives. At the request of the company, the team temporarily installed network security monitoring equipment, gathered host and network data, and examined ICS equipment to assess network integrity. Initial analysis spotted low-level malware throughout the water network, but found no indication of the same on the power network.</em>

<em>Next the team visited several sites essential to the entity’s operations. One of these sites was the distribution/transmission control center, where the team met with personnel who oversee operations on the power side and manually collected information from the site’s servers/HMI.While reviewing the network architecture of the distribution/transmission control center and the data capture, the team discovered a wireless router that the asset owner believed to be disconnected from the network. The wireless router was active and allowed for direct access into the control system environment.</em>

<em>The team also visited the water control center and a power substation to examine equipment. At the water control center, the team discovered a cellular modem connected to the main water switch. The local staff was unsure of its direct function, but it was later identified as a cellular modem that allowed for remote vendor access via a simple username and password. While analyzing the collected data,TeamViewer connections were discovered on high value hosts (IT operations computers, billing, nance, and badging) to foreign hosts. The team confirmed with local staff that these were not legitimate and the activity was blocked by the asset owner.</em>

<em>At the end of the visit, the team provided the asset owner with its initial findings, as well as an assortment of best practices/recommendations specific to their environment.The customer was receptive to ICS-CERT’s recommendations and requested additional support in the coming months to review the architecture/cyber security posture of its proposed new network.</em>
