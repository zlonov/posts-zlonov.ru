---
layout: zlonov/old_post
title: (уязвимость) Благодаря Positive Technologies устранены опасные уязвимости в SCADA-системах Siemens и Schneider Electric
date: 2015-08-19 19:12
author: admin
category: autoimport
tags: [InduSoft Web Studio, InTouch Machine Edition 2014, Positive Technologies, Schneider Electric, Siemens, Siemens SIMATIC, Илья Карпов, нефтехимия, уязвимости]
---
<p class="preview">Специалисты Schneider Electric советуют пользователям как можно скорее установить существующие обновления безопасности.

<div class="news-full-content">

Эксперт Positive Technologies Илья Карпов обнаружил и помог устранить уязвимости в продуктах, предназначенных для построения систем автоматизации в различных отраслях, от нефтехимических заводов до электростанций.

Илья выявил проблему хранения паролей в открытом виде в системах компании Schneider Electric — InTouch Machine Edition 2014 (версия 7.1, Service Pack 3, Patch 4) и InduSoft Web Studio (7.1.3.4), а также в их предыдущих версиях. Уязвимость, которая получила идентификатор CVE-2015-1009 и базовую оценку 6,4, нельзя использовать удаленно, однако внутреннему злоумышленнику достаточно низкой квалификации для ее эксплуатации.

Специалисты Schneider Electric советуют пользователям как можно скорее установить существующие обновления безопасности (патч для InTouch Machine Edition 2014, патч для InduSoft Web Studio) и ограничить физический доступ персонала к этим системам в целях снижения потенциальной угрозы разглашения конфиденциальной информации со стороны внутренних злоумышленников.

Кроме того, в июле компания Siemens выпустила специальный апдейт к апрельскому бюллетеню, в котором поблагодарила Илью Карпова за обнаружение опасной и очень простой в использовании уязвимости, угрожающей безопасности целого ряда решений на базе Siemens SIMATIC:
<ul>
	<li>SIMATIC HMI Basic Panels 2nd Generation — все версии до WinCC (TIA Portal) V13 SP1 Upd2;</li>
	<li>SIMATIC HMI Comfort Panels — все версии до WinCC (TIA Portal) V13 SP1 Upd2;</li>
	<li>SIMATIC WinCC Runtime Advanced — все версии до WinCC (TIA Portal) V13 SP1 Upd2;</li>
	<li>SIMATIC WinCC Runtime Professional — все версии до WinCC (TIA Portal) V13 SP1 Upd2;</li>
	<li>SIMATIC HMI Basic Panels 1st Generation (WinCC TIA Portal) — все версии до WinCC (TIA Portal) V13 SP1 Upd4;</li>
	<li>SIMATIC HMI Mobile Panel 277 (WinCC TIA Portal) — все версии до WinCC (TIA Portal) V13 SP1 Upd4;</li>
	<li>SIMATIC HMI Multi Panels (WinCC TIA Portal) — все версии до WinCC (TIA Portal) V13 SP1 Upd4;</li>
	<li>SIMATIC WinCC V7.X — все версии до V7.3 Upd4;</li>
	<li>SIMATIC PCS 7 — все версии до V8.1 SP1.</li>
</ul>
Ошибка CVE-2015-2823 с оценкой 6,8 дает возможность локально и удаленно пройти аутентификацию на сервере с помощью хеш-функции пароля пользователя. Пароль при этом знать не обязательно.

Компания Positive Technologies одной из первых стала исследовать вопросы безопасности систем промышленной автоматизации, сотрудничая с ведущими производителями АСУ ТП (SCADA). В 2012 году было представлено масштабное исследование «Безопасность промышленных систем в цифрах». Год спустя в лаборатории Positive Technologies создали стенд Choo Choo Pwn — модель игровой железной дороги, все элементы которой — поезда, шлагбаумы, светофоры — контролируются с помощью АСУ ТП, собранной на основе трех SCADA-систем. Эксперты компании регулярно проводят тематические вебинары и выступают на ведущих международных конференциях по информационной безопасности.

В 2015 году одним из самых зрелищных элементов соревновательной программы форума PHDays V стал конкурс, участники которого должны были захватить контроль над промышленной системой управления, связанной с ракетной установкой, и произвести выстрел по «секретному объекту». А конкурс Choo Choo Pwn в этом году стал еще более реалистичным: как и в реальном мире, участникам нельзя было отправить команду, которая приведет к аварии: логика, обеспечивающая безопасность движения, не позволяла этому произойти, — и целью соревнования стал взлом целого комплекса средств, обеспечивающих безопасность транспорта.

Все необходимые проверки на наличие недостатков безопасности, выявленных в программном обеспечении Siemens SIMATIC, добавлены в базу знаний системы контроля защищенности и соответствия стандартам MaxPatrol. Часть этих проблем безопасности обнаруживается эвристическими механизмами MaxPatrol и без обновления базы знаний.
<p style="text-align: right;"><sub><em><a href="http://Специалисты Schneider Electric советуют пользователям как можно скорее установить существующие обновления безопасности. Эксперт Positive Technologies Илья Карпов обнаружил и помог устранить уязвимости в продуктах, предназначенных для построения систем автоматизации в различных отраслях, от нефтехимических заводов до электростанций. Илья выявил проблему хранения паролей в открытом виде в системах компании Schneider Electric — InTouch Machine Edition 2014 (версия 7.1, Service Pack 3, Patch 4) и InduSoft Web Studio (7.1.3.4), а также в их предыдущих версиях. Уязвимость, которая получила идентификатор CVE-2015-1009 и базовую оценку 6,4, нельзя использовать удаленно, однако внутреннему злоумышленнику достаточно низкой квалификации для ее эксплуатации. Специалисты Schneider Electric советуют пользователям как можно скорее установить существующие обновления безопасности (патч для InTouch Machine Edition 2014, патч для InduSoft Web Studio) и ограничить физический доступ персонала к этим системам в целях снижения потенциальной угрозы разглашения конфиденциальной информации со стороны внутренних злоумышленников. Кроме того, в июле компания Siemens выпустила специальный апдейт к апрельскому бюллетеню, в котором поблагодарила Илью Карпова за обнаружение опасной и очень простой в использовании уязвимости, угрожающей безопасности целого ряда решений на базе Siemens SIMATIC: SIMATIC HMI Basic Panels 2nd Generation — все версии до WinCC (TIA Portal) V13 SP1 Upd2; SIMATIC HMI Comfort Panels — все версии до WinCC (TIA Portal) V13 SP1 Upd2; SIMATIC WinCC Runtime Advanced — все версии до WinCC (TIA Portal) V13 SP1 Upd2; SIMATIC WinCC Runtime Professional — все версии до WinCC (TIA Portal) V13 SP1 Upd2; SIMATIC HMI Basic Panels 1st Generation (WinCC TIA Portal) — все версии до WinCC (TIA Portal) V13 SP1 Upd4; SIMATIC HMI Mobile Panel 277 (WinCC TIA Portal) — все версии до WinCC (TIA Portal) V13 SP1 Upd4; SIMATIC HMI Multi Panels (WinCC TIA Portal) — все версии до WinCC (TIA Portal) V13 SP1 Upd4; SIMATIC WinCC V7.X — все версии до V7.3 Upd4; SIMATIC PCS 7 — все версии до V8.1 SP1. Ошибка CVE-2015-2823 с оценкой 6,8 дает возможность локально и удаленно пройти аутентификацию на сервере с помощью хеш-функции пароля пользователя. Пароль при этом знать не обязательно. Компания Positive Technologies одной из первых стала исследовать вопросы безопасности систем промышленной автоматизации, сотрудничая с ведущими производителями АСУ ТП (SCADA). В 2012 году было представлено масштабное исследование «Безопасность промышленных систем в цифрах». Год спустя в лаборатории Positive Technologies создали стенд Choo Choo Pwn — модель игровой железной дороги, все элементы которой — поезда, шлагбаумы, светофоры — контролируются с помощью АСУ ТП, собранной на основе трех SCADA-систем. Эксперты компании регулярно проводят тематические вебинары и выступают на ведущих международных конференциях по информационной безопасности. В 2015 году одним из самых зрелищных элементов соревновательной программы форума PHDays V стал конкурс, участники которого должны были захватить контроль над промышленной системой управления, связанной с ракетной установкой, и произвести выстрел по «секретному объекту». А конкурс Choo Choo Pwn в этом году стал еще более реалистичным: как и в реальном мире, участникам нельзя было отправить команду, которая приведет к аварии: логика, обеспечивающая безопасность движения, не позволяла этому произойти, — и целью соревнования стал взлом целого комплекса средств, обеспечивающих безопасность транспорта. Все необходимые проверки на наличие недостатков безопасности, выявленных в программном обеспечении Siemens SIMATIC, добавлены в базу знаний системы контроля защищенности и соответствия стандартам MaxPatrol. Часть этих проблем безопасности обнаруживается эвристическими механизмами MaxPatrol и без обновления базы знаний." target="_blank">Источник</a></em></sub>

</div>