---
layout: zlonov/old_post
title: Как узнать номер недели в году по дате?
date: 2012-04-18 12:13
author: admin
category: autoimport
tags: [excel, полезное]
---
<p style="text-align: center;"><a href="https://zlonov.ru/2012/04/how_to_calculate_number_of_the_week/excel/" rel="attachment wp-att-1819"><img class="aligncenter  wp-image-1819" title="excel" alt="" src="/assets/uploads/2012/04/excel.gif" width="280" height="280" /></a>
Удобнее всего использовать Excel, введя в ячейку A1 дату, а в любую другую - формулу:

<em>=ЦЕЛОЕ((A1-ДАТА(ГОД(A1-ДЕНЬНЕД(A1-1)+4);1;3)+ДЕНЬНЕД(ДАТА(ГОД(A1-ДЕНЬНЕД(A1-1)+4);1;3))+5)/7)</em>
