---
layout: zlonov/old_post
title: (уязвимость) В линейке SCADA-систем Schneider Electric обнаружены опасные бреши
date: 2014-09-19 22:53
author: admin
category: autoimport
tags: [ClearSCADA, ICS-CERT, SCADA, Schneider Electric, аутентификация, водоснабжение, Европа, ИБ АСУ ТП, США, уязвимости, хеширование, энергетика]
---
В общей сложности сторонние исследователи безопасности обнаружили три уязвимости.

Как сообщают разработчики SCADA Expert ClearSCADA (линейка популярных SCADA-систем) из Schneider Electric, сторонние исследователи безопасности обнаружили в продуктах компании три опасные бреши. При этом уязвимые программно-аппартаные комплексы используются в таких отраслях как энергетика, водоснабжение, контроль крупных коммерческих объектов и наиболее распространены в США и Европе.

Обнаружить уязвимости удалось специалистам из ICS-CERT, по словам которых эти бреши позволяют потенциальному удаленному злоумышленнику обойти механизм аутентификации и осуществить CSRF-нападение. Третья брешь заключается в наличии слабого алгоритма хеширования.

В сумме эти изъяны в системе безопасности позволяют полностью скомпрометировать атакуемую систему. Тем не менее, для этого атакующим необходимо вынудить пользователя с правами администратора перейти по специально сформированной ссылке.

Представители Schneider Electric заверяют, что соответствующие исправления безопасности будут выпущены в конце текущего месяца. При этом слабый алгоритм можно будет заменить специальной отдельной утилитой.
