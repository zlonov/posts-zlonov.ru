---
layout: zlonov/old_post
title: '(инцидент) Обнаружен троян, инфицирующий «умные» телевизоры'
date: 2016-01-13 17:41
author: admin
category: autoimport
tags: [Android, Trend Micro, вредоносное ПО, инциденты, умные телевизоры, уязвимость]
---
<em>Вредоносное ПО эксплуатирует уязвимость в устаревших версиях ОС Android.</em>

Исследователи Trend Micro обнаружили троян, поражающий «умные» телевизоры под управлением ОС Android. Вредонос эксплуатирует уязвимость в устаревших версиях операционной системы и позволяет скомпрометировать устройство.

Троян эксплуатирует уязвимость <a href="http://www.securitylab.ru/vulnerability/478415.php" target="_blank">CVE-2014-7911</a>, присутствующую в версиях ОС Android 1.6 – 4.4.2. Ошибка позволяет удаленному злоумышленнику повысить привилегии на целевой системе. Уязвимость была исправлена еще в 2014 году, но до сих пор присутствует в большинстве «умных» телевизоров под управлением Android, поскольку производители редко выпускают обновленные версии прошивок.

Троян распространяется через сайты, содержащие вредоносные приложения, якобы предназначенные для просмотра зарубежных телеканалов. Ресурсы преимущественно размещены на американских или канадских серверах. Загружаемые с подобных сайтов приложения инфицированы трояном AndroidOS_RootsTV.A позволяющим злоумышленнику получить полный контроль над устройством путем эксплуатации уязвимости.

Повысив привилегии, злоумышленник может без ведома пользователя устанавливать произвольные приложения или вредоносное ПО на устройство жертвы. При этом программы будут загружаться по HTTP, создавая условия для новой атаки. Осуществив атаку «человек посередине», другой хакер сможет перехватить и подменить трафик.

<a href="http://www.securitylab.ru/news/478412.php" target="_blank">Источник</a>