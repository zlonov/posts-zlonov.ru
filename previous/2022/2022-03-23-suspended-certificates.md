---
layout: single
title: 'Приостановленные сертификаты ФСТЭК России'
date: 2022-03-23

tags: ['Microsoft', 'Cisco', 'Kerio Control', 'LabWare', 'Huawei', 'Red Hat', 'SUSE Linux', 'ARMlock', 'VMware', 'IBM', 'ViPNet xFirewall', 'FortiGate', 'eToken', 'OpenText Documentum', 'SAP', 'PlanningSpace', 'Skybox', 'CyberArk', 'DeviceLock', 'Veeam', 'ESET', 'Oracle']

categories: ["Законодательство", "Средства защиты"]

classes: wide

excerpt: 'Десятки приостановленных сертификатов соответствия у зарубежных и российских производителей.'

canonical_url: "https://zlonov.com/suspended-certificates/"

header:
    teaser: /assets/images/2022/stop.png
    overlay_image: /assets/images/2022/stop.png
    show_overlay_excerpt: true
    overlay_filter: 0.25 # same as adding an opacity of 0.5 to a black background
last_modified_at: 2022-04-11    
---
**Добавлено 07.04.2022** - Снова [изменения](https://t.me/zlonov/1403) в реестре сертифицированных средств защиты информации ФСТЭК России: приостановлено действие суммарно у 31 сертификата и прекращено действие у 40 сертификатов.
{: .notice}

**Добавлено 11.04.2022** - Полный [перечень](/catalog/suspended-and-terminated-certificates/) сертификатов соответствия ФСТЭК России, действие которых было приостановлено или прекращено.
{: .notice}

**Добавлено 19.09.2023** - Более детально расписал, что на самом деле означает статус 'приостановлено действие' у сертификата ФСТЭК России в соответствующем посте: [Приостановлен, но не сломлен](/suspended-but-not-broken/).
{: .notice}

Обновление Государственного [реестра](http://bit.ly/reestr-fstec) сертифицированных средств защиты информации ФСТЭК России от 3 марта 2022 года для 18 сертификатов соответствия оказалось не самым радостным - их действие [было приостановлено](https://t.me/zlonov/1383).

{% include one_image_new2.html picture_name="Действие сертификата соответствия приостановлено 03 марта 2022" picture_path="2022/18.png" %}

Коллеги в обсуждении в телеграмм-чате [ruCyberSecurity](https://t.me/ruCyberSecurity) предположили, что основная причина - в отсутствии [сертификации по уровням доверия](https://zlonov.com/laws/приказ-фстэк-76-от-02-06-2020). Косвенно это подтверждается [пресс-релизом](https://www.securitycode.ru/company/news/o-priostanovke-sertifikatov-sootvetstviya-secret-net-studio-c-i-secret-net-lsp-c-/) компании "Код Безопасности":
 > Компания «Код Безопасности» информирует о приостановке сертификатов соответствия ФСТЭК России №3675 и 4200 на продукты Secret Net Studio – C и Secret Net LSP – C.\
 > В связи с архитектурными особенностями ОС Windows и многочисленными ОС семейства Linux взаимодействующими с нашими продуктами, а также особенностями используемых фреймворков при разработке, **объём проверок для сертификации по 2-му уровню доверия значительно превысил запланированные сроки**.

Пару раз после этой даты проверял реестр, но изменений не видел, а вот сегодня во время [эфира AM Live по анализу защищенности промышленных предприятий](https://live.anti-malware.ru/ot-pentest) узнал от коллег, что, оказывается, приостановленных сертификатов уже гораздо больше:

 - №3987 - cистема управления базами данных **Microsoft SQL Server 2016** SP2 в редакциях Enterprise Edition (EE), Standard (Std)\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №4098 - cистема управления базами данных **Microsoft SQL Server 2017** в редакциях Enterprise Edition (EE), Standard (Std), Developer, Web, Express, Express with Advanced Services»\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №4290 - коммутатор серии **Cisco IE-3000** (модели IE-3000-8ТС и IE-3000-8TC-E) с установленным программным обеспечением Cisco IOS версии 15.2.4-ЕА9\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к МЭ, Профиль защиты МЭ(А шестого класса защиты. ИТ.МЭ.А6.ПЗ), Профиль защиты МЭ(Б шестого класса защиты. ИТ.МЭ.Б6.ПЗ)_

 - №4128 - лабораторная информационная менеджмент система «**LabWare 7**» (ЛИМС «LabWare 7»)\
_Было: Соответствует требованиям документов: ТУ_

 - №4323 - межсетевой экран «**Kerio Control**»\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к МЭ, Профиль защиты МЭ(Б шестого класса защиты. ИТ.МЭ.Б6.ПЗ), Требования к САВЗ, Профиль защиты САВЗ(Б шестого класса защиты. ИТ.САВЗ.Б6.ПЗ), Требования к СОВ, Профили защиты СОВ(cети шестого класса защиты. ИТ.СОВ.С6.ПЗ)_

 - №4407 - межсетевой экран серии **Cisco ASA 55xx** (модели: Cisco ASA 5512, Cisco ASA 5515, Cisco ASA 5525, Cisco ASA 5545, Cisco ASA 5555, Cisco ASA 5585) с установленным программным обеспечением Cisco ASA версии 9.X\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к МЭ, Профиль защиты МЭ(А шестого класса защиты. ИТ.МЭ.А6.ПЗ), Профиль защиты МЭ(Б шестого класса защиты. ИТ.МЭ.Б6.ПЗ)_

 - №4373 - межсетевой экран серии **Cisco Firepower 2100** (модели: Firepower 2110, Firepower 2120, Firepower 2130, Firepower 2140)\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к МЭ, Профиль защиты МЭ(А шестого класса защиты. ИТ.МЭ.А6.ПЗ), Профиль защиты МЭ(Б шестого класса защиты. ИТ.МЭ.Б6.ПЗ)_

 - №4083 - межсетевой экран серии **Huawei** (модели: USG6320 (Eudemon200E-N1D), USG6330 (Eudemon200E-N1), USG6350 (Eudemon200E-N2), USG6360, USG6370 (Eudemon200E-N3), USG6380, USG6390 (Eudemon200E-N5), USG6620 (Eudemon1000E-N3), USG6630 (Eudemon1000E-N5), USG6650, USG6660 (Eudemon1000E-N6), USG6670 Eudemon1000E-N7), USG6680 (Eudemon1000E-N7E), USG9560 (Eudemon8000E-X8), USG9580 (Eudemon8000E-X16)) версии V500\
_Было: Соответствует требованиям документов: Требования к МЭ, Профиль защиты МЭ(А четвертого класса защиты. ИТ.МЭ.А4.ПЗ), Профиль защиты МЭ(Б четвертого класса защиты. ИТ.МЭ.Б4.ПЗ)_

 - №4369 - операционная система **Microsoft Windows 10** в редакции Корпоративная\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к ОС, Профиль защиты ОС(А шестого класса защиты. ИТ.ОС.А6.ПЗ)_

 - №4006 - операционная система **Microsoft Windows Server 2016**\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к ОС, Профиль защиты ОС(А шестого класса защиты. ИТ.ОС.А6.ПЗ), ЗБ_

 - №4412 - операционная система **Red Hat Enterprise Linux 7**\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к ОС, Профиль защиты ОС(А шестого класса защиты. ИТ.ОС.А6.ПЗ)_

 - №4403 - операционная система **Red Hat Enterprise Linux 8**\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к ОС, Профиль защиты ОС(А шестого класса защиты. ИТ.ОС.А6.ПЗ)_

 - №4035 - операционная система **SUSE Linux Enterprise Server 12 SP3**\
_Было: Соответствует требованиям документов: Требования к ОС, Профиль защиты ОС(А четвертого класса защиты. ИТ.ОС.А4.ПЗ)_

 - №4497 - операционная система «**SUSE Linux Enterprise Server for SAP Applications 15 SP3**»\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к ОС, Профиль защиты ОС(А шестого класса защиты. ИТ.ОС.А6.ПЗ)_

 - №3474 - Программа защиты информации от несанкционированного доступа **ARMlock**\
_Было: Соответствует требованиям документов: РД НДВ(4), РД СВТ(5)_

 - №4398 - программная платформа **VMware NSX-T Data Center**\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к МЭ, Профиль защиты МЭ(Б шестого класса защиты. ИТ.МЭ.Б6.ПЗ)_

 - №3941 - программно-аппаратные комплексы «Маршрутизаторы **Huawei серии AR3200, серии AR2200, серии AR1200**»\
_Было: Соответствует требованиям документов: Требования к МЭ, Профиль защиты МЭ(А пятого класса защиты. ИТ.МЭ.А5.ПЗ)_

 - №4093 - программно-аппаратный комплекс **ViPNet xFirewall 4**\
_Было: Соответствует требованиям документов: Требования к МЭ, Профиль защиты МЭ(А четвертого класса защиты. ИТ.МЭ.А4.ПЗ), Профиль защиты МЭ(Б четвертого класса защиты. ИТ.МЭ.Б4.ПЗ)_

 - №4462 - программно-аппаратный комплекс **«FortiGate» для защиты промышленной сети**\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к МЭ, Профиль защиты МЭ(Д шестого класса защиты. ИТ.МЭ.Д6.ПЗ), Требования к САВЗ, Профиль защиты САВЗ(Б шестого класса защиты. ИТ.САВЗ.Б6.ПЗ), Требования к СОВ, Профили защиты СОВ(cети шестого класса защиты. ИТ.СОВ.С6.ПЗ)_

 - №4222 - программно-аппаратный комплекс **«FortiGate», функционирующий под управлением операционной системы FortiOS версии 6.X**\
_Было: Соответствует требованиям документов: Требования к МЭ, Профиль защиты МЭ(А четвертого класса защиты. ИТ.МЭ.А4.ПЗ), Профиль защиты МЭ(Б четвертого класса защиты. ИТ.МЭ.Б4.ПЗ), Требования к СОВ, Профили защиты СОВ(cети четвертого класса защиты. ИТ.СОВ.С4.ПЗ)_

 - №4362 - программно-аппаратный комплекс **«FortiGate», функционирующий под управлением операционной системы FortiOS версии 6.X**\
_Было: Соответствует требованиям документов: Требования доверия(6), Требования к МЭ, Профиль защиты МЭ(А шестого класса защиты. ИТ.МЭ.А6.ПЗ), Профиль защиты МЭ(Б шестого класса защиты. ИТ.МЭ.Б6.ПЗ), Требования к САВЗ, Профиль защиты САВЗ(Б шестого класса защиты. ИТ.САВЗ.Б6.ПЗ), Требования к СОВ, Профили защиты СОВ(cети шестого класса защиты. ИТ.СОВ.С6.ПЗ)_

 - №3910 - программно-аппаратный комплекс «Коммутатор **Huawei серии S12700**»\
_Было: Соответствует требованиям документов: Требования к МЭ, Профиль защиты МЭ(А пятого класса защиты. ИТ.МЭ.А5.ПЗ)_

 - №3865 - программно-аппаратный комплекс «Маршрутизатор **Huawei серии NE20E**»\
_Было: Соответствует требованиям документов: Требования к МЭ, Профиль защиты МЭ(А пятого класса защиты. ИТ.МЭ.А5.ПЗ)_

 - №4285 - программно-аппаратный комплекс аутентификации и хранения ключевой информации - «Электронный ключ **SafeNet eToken 10**»\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №2730 - программно-аппаратный комплекс аутентификации и хранения ключевой информации - «Электронный ключ **SafeNet eToken 8**»\
_Было: Соответствует требованиям документов: РД НДВ(4), ТУ_

 - №3863 - программно-аппаратный комплекс Коммутатор **Huawei серии S5720**»\
_Было: Соответствует требованиям документов: Требования к МЭ, Профиль защиты МЭ(А пятого класса защиты. ИТ.МЭ.А5.ПЗ)_

 - №4201 - программное обеспечение **IBM «Maximo 7»**\
_Было: Соответствует требованиям документов: ТУ_

 - №4326 - программное обеспечение **Microsoft SharePoint Server 2019**\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №4198 - программное обеспечение **OpenText Documentum 16.4**\
_Было: Соответствует требованиям документов: ЗБ_

 - №4514 - программное обеспечение **SAP Marketing, версия 1909**\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №4216 - программное обеспечение «**ESET NOD32 Secure Enterprise Pack**» (версия 6)\
_Было: Соответствует требованиям документов: Требования к САВЗ, Профиль защиты САВЗ(А четвертого класса защиты. ИТ.САВЗ.А4.ПЗ), Профиль защиты САВЗ(Б четвертого класса защиты. ИТ.САВЗ.Б4.ПЗ), Профиль защиты САВЗ(В четвертого класса защиты. ИТ.САВЗ.В4.ПЗ), Профиль защиты САВЗ(Г четвертого класса защиты. ИТ.САВЗ.Г4.ПЗ)_

 - №4296 - программное обеспечение «**PlanningSpace**»\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №4414 - программное обеспечение «**SAP Application Platform 7**»\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №3959 - программное обеспечение «**Symantec Endpoint Protection**» (версия 14)\
_Было: Соответствует требованиям документов: Требования к МЭ, Профиль защиты МЭ(В шестого класса защиты. ИТ.МЭ.В6.ПЗ), Требования к САВЗ, Профиль защиты САВЗ(А шестого класса защиты. ИТ.САВЗ.А6.ПЗ), Профиль защиты САВЗ(Б шестого класса защиты. ИТ.САВЗ.Б6.ПЗ), Профиль защиты САВЗ(В шестого класса защиты. ИТ.САВЗ.В6.ПЗ), Профиль защиты САВЗ(Г шестого класса защиты. ИТ.САВЗ.Г6.ПЗ), Требования к СОВ, Профили защиты СОВ(узла шестого класса защиты. ИТ.СОВ.У6.ПЗ)_

 - №4248 - программное обеспечение «**Trend Micro Deep Security 10**»\
_Было: Соответствует требованиям документов: Требования к МЭ, Профиль защиты МЭ(В шестого класса защиты. ИТ.МЭ.В6.ПЗ), Требования к САВЗ, Профиль защиты САВЗ(А шестого класса защиты. ИТ.САВЗ.А6.ПЗ), Профиль защиты САВЗ(В шестого класса защиты. ИТ.САВЗ.В6.ПЗ), Профиль защиты САВЗ(Г шестого класса защиты. ИТ.САВЗ.Г6.ПЗ), Требования к СОВ, Профили защиты СОВ(узла шестого класса защиты. ИТ.СОВ.У6.ПЗ)_

 - №3960 - программное обеспечение «**Veeam Availability Suite**» (версия 9)\
_Было: Соответствует требованиям документов: ТУ_

 - №4435 - программное обеспечение «Вычислительная платформа со встроенными средствами защиты информации от несанкционированного доступа **SAP HANA Enterprise Edition 2**»\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №3966 - программное обеспечение «Программный комплекс «**Huawei Fusion Access**» версии 6.Х»\
_Было: Соответствует требованиям документов: ТУ_

 - №4041 - программное обеспечение мультиплексора **FOX 512/515 и FOX 612/615** с системой управления **FOXMAN**\
_Было: Соответствует требованиям документов: ЗБ, ТУ_

 - №4070 - программное обеспечение мультиплексоров **PCM30U/PCM30U-OCH** с системой управления **TopoNet**\
_Было: Соответствует требованиям документов: ЗБ_

 - №3465 - программный комплекс **DeviceLock 8 DLP Suite**\
_Было: Соответствует требованиям документов: Требования к СКН, Профиль защиты СКН(контроля подключения съемных машинных носителей информации четвертого класса защиты. ИТ.СКН.П4.ПЗ), ЗБ_

 - №4074 - программный комплекс **Microsoft Project Server 2016** в составе SharePoint Server 2016\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №4325 - программный комплекс **Microsoft Project Server 2019** в составе SharePoint Server 2019\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №3978 - программный комплекс **Microsoft System Center 2016**\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №4356 - программный комплекс **Skybox Security Suite**\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №4396 - программный комплекс **VMware Horizon** с системой идентификации и аутентификации **VMware Workspace ONE Access**\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №3659 - программный комплекс **VMware vSphere with Operations Management 6**\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №4378 - программный комплекс для автоматизации и управления ресурсами виртуальной инфраструктуры **VMware vRealize Automation**\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №4319 - программный комплекс для создания и управления виртуальной инфраструктурой **VMware vSphere**\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №3739 - Программный комплекс управления привилегированными учетными записями, сессиями и привилегиями **CyberArk Privileged Access Security Solution**\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №1900 - система комплексного управления безопасностью «**КУБ**»\
_Было: Соответствует требованиям документов: РД НДВ(3), ТУ_

 - №4224 - система корпоративного мобильного рабочего места **WorksPad**\
_Было: Соответствует требованиям документов: РД НДВ(4)_

 - №4388 - система управления базами данных **Oracle Database 19** с опциями Oracle Advanced Security и Oracle Database Vault\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №4370 - система управления базами данных «**Microsoft SQL Server 2019**»\
_Было: Соответствует требованиям документов: Требования доверия(6), ТУ_

 - №3675 - средство защиты информации **Secret Net Studio — C**\
_Было: Соответствует требованиям документов: Требования к МЭ, Профиль защиты МЭ(В второго класса защиты. ИТ.МЭ.В2.ПЗ), РД СВТ(3)_

 - №4200 - средство защиты информации «**Secret Net LSP - C**»\
_Было: Соответствует требованиям документов: РД НДВ(2), ТУ_

---

У многих средств сертификация по требованиям доверия (правда, только по 6 уровню) была выполнена, так что причина не просто в этом. В своём информационном сообщении ФСТЭК России [деталей не раскрывает](https://fstec.ru/127-lenta-novostej/1656-informatsionnoe-soobshchenie-18).

Так что при выборе сертифицированных средств защиты сейчас надо внимательно проверять в том числе и неприостановку действия их сертификатов соответствия.