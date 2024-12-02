---
layout: zlonov/old_post
title: Презентация нового MaxPatrol SIEM
date: 2015-05-21 20:32
author: admin
category: autoimport
tags: [Positive Technologies, SIEM, информационная безопасность, мероприятие]
---
Компания Positive Technologies сегодня провела пресс-конференцию для СМИ, блогеров и экспертов под общим названием "Как увидеть невидимые кибератаки?". Ответ на данный вопрос предполагался достаточно очевидный - с помощью <a href="https://zlonov.ru/catalog/maxpatrol-siem/">MaxPatrol SIEM</a>.

До презентации самого SIEM коллеги рассказали кратко о истории своей компании, как здорово у них получается делать пентесты (взлом сети компании занимает 3-5 дней), какие методы используют для проникновения и почему их почти никогда не обнаруживают администраторы проверяемых компаний. Несколько слайдов про это ниже.

[caption id="attachment_6554" align="aligncenter" width="700"]<a href="/assets/uploads/Positive-Technologies.-Безопасность-в-цифрах.jpg"><img class="wp-image-6554" title="Positive Technologies. Безопасность в цифрах" src="/assets/uploads/Positive-Technologies.-Безопасность-в-цифрах-1024x666.jpg" alt="Positive Technologies. Безопасность в цифрах" width="700" height="455" /></a> Positive Technologies. Безопасность в цифрах[/caption]

[caption id="attachment_6555" align="aligncenter" width="700"]<a href="/assets/uploads/Positive-Technologies.-Используемые-недостатки.jpg"><img class="wp-image-6555" title="Positive Technologies. Используемые недостатки" src="/assets/uploads/Positive-Technologies.-Используемые-недостатки-1024x633.jpg" alt="Positive Technologies. Используемые недостатки" width="700" height="433" /></a> Positive Technologies. Используемые недостатки[/caption]

[caption id="attachment_6556" align="aligncenter" width="700"]<img class="wp-image-6556" title="Positive Technologies. Проблема обнаружения" src="/assets/uploads/Positive-Technologies.-Проблема-обнаружения-1024x665.jpg" alt="Positive Technologies. Проблема обнаружения" width="700" height="454" /> Positive Technologies. Проблема обнаружения[/caption]

Непосредственно презентация MaxPatrol SIEM представляла собой два видео-ролика. Сделаны качественно, хотя, конечно, требуют аудитории, которая понимает суть хакерских атак, но не слишком глубоко (иначе <a href="https://twitter.com/sb0risov/status/601327791947255808" target="_blank">банально и не впечатляет</a>). В любом случае, очень здорово, что интерфейс системы показывали именно на видео - действительно, это же не пилотное тестирование, какая разница: живая перед нами система или запись с вырезанными лишними движениями курсора мыши, кликами и ожиданиями отклика системы?

Технической стороне вопроса (всё же формат мероприятия - пресс-конференция) было уделено ровно столько, сколько надо: оставшиеся у каждого вопросы можно было задать после: и про используемые базы данных и про возможности дашбоардов.

Что касается непосредственно самого MaxPatrol SIEM (ранее рабочее название было MaxPatrol X), то по словам представителей Positive Technologies они создали новую платформу, которая, например, в терминологии Gartner попадает сразу в несколько его <a href="https://zlonov.ru/gartner-magic-quadrants/" target="_blank">Магических Квадратов</a>, но для определённости в глазах заказчиков остановились всё же на варианте названия именно SIEM. Отчасти поэтому среди конкурентов оказались "<em>псевдо-российские разработки с переклеенными шильдиками</em>". Вот такой вот камень в некоторый огород был отправлен в ходе презентации =)

Про преимущества нового продукта говорили много, они подробно расписаны в <a href="http://bit.ly/1dn4H2a" target="_blank">листовке</a>, но всё же самым <em>вкусным</em> на мой взгляд является то, что вся годами нарабатываемая Positive Technologies экспертиза в понимании того, как именно работают хакеры (как они проникают в системы, какие методы и инструменты используют) легла в основу правил для корреляционного движка. Поэтому MaxPatrol SIEM по череде характерных событий способен выявить планируемую атаку даже таргетированную (целенаправленную) на достаточно раннем этапе и отреагировать на неё с упреждением. Ну, по крайне мере в теории может =) Хотя, коллеги были достаточно убедительны - так что не удивлюсь, если первые практические результаты будут близки к маркетинговым обещаниям.

В заключение небольшая, но говорящая деталь - код листовки, которую выдавали участникам: MP_SIEM_PB_A4.RUS.001.03.MAY.18.2015 Чувствуете всю системность и серьёзность подхода даже к разработке маркетинговых материалов? =)

[caption id="attachment_6562" align="aligncenter" width="500"]<a href="/assets/uploads/Positive-Technologies.-MaxPatrol-SIEM.-Код-листовки.jpg"><img class="wp-image-6562" src="/assets/uploads/Positive-Technologies.-MaxPatrol-SIEM.-Код-листовки-1024x357.jpg" alt="Positive Technologies. MaxPatrol SIEM. Код листовки" width="500" height="174" /></a> Positive Technologies. MaxPatrol SIEM. Код листовки[/caption]

Ещё некоторые слайды и тезисы с пресс-конференции можно отыскать в твитах Сергея Борисова (<a href="https://twitter.com/sb0risov" target="_blank">@sb0risov</a>) и Андрея Прозорова (<a href="https://twitter.com/3dwave" target="_blank">@3dwave</a>).

[box type="info" style="rounded"]<strong>UPD. 22.05.2015</strong> Ещё впечатления коллег можно почитать здесь: Артём Агеев "<a href="http://www.itsec.pro/2015/05/positive-siem.html" target="_blank">Positive SIEM</a>", Александр Бодрик "<a href="http://inf-sec.blogspot.ru/2015/05/maxpatrol-siem.html" target="_blank">MaxPatrol SIEM - отчаянная ставка Позитивов</a>"[/box]

Из мелочей - меня почему-то до сих пор в базах Positive Technologies считают сотрудником SafeLine. Да, тут системность чуть пострадала, видимо =)

<a href="/assets/uploads/ZlonovRu.jpg"><img class="aligncenter wp-image-6558" src="/assets/uploads/ZlonovRu-1024x1024.jpg" alt="ZlonovRu" width="500" height="500" /></a>
