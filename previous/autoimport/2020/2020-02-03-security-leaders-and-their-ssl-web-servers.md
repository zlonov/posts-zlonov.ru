---
layout: zlonov/old_post
title: ИБ лидеры и поддержка SSL их веб-серверами
date: 2020-02-03 17:29
author: admin
category: autoimport
tags: [CNews, Qualys Security, SSL, информационная безопасность, рейтинг, сертификат]
---

У компании Qualys есть хороший бесплатный онлайн-сервис по анализу конфигурации SSL любых веб-серверов в Интернете: <a href="https://www.ssllabs.com/ssltest/index.html">SSL Server Test</a>.



В одной из недавних статей на Хабре автор тестировал сайт РЖД, а мне захотелось проверить сайты компаний из текущего рейтинга CNews Security: <a href="https://www.cnews.ru/reviews/security2019/review_table/9f40780235d21a3c5c6e116bcf364c193569ff98">Крупнейшие компании России в сфере защиты информации 2019</a>.



Дабы не приводить в посте детальные скриншоты по каждому из 30 номинантов, свёл их в таблицу. Ссылки открывают окна сканирования. Сортировка в ячейках - согласно позициям в рейтинге CNews (наименования тоже взяты из рейтинга).


<!-- wp:table {"align":"center"} -->
<figure class="wp-block-table aligncenter"><table class=""><tbody><tr><td><img src="/assets/uploads/Рейтинг-A.png" alt="" class="wp-image-73662"/></td><td><a href="https://www.ssllabs.com/ssltest/analyze.html?d=ptsecurity.com">Positive Technologies</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=aq.ru">Аквариус</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=ussc.ru">УЦСБ</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=angaratech.ru">Angara</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=crosstech.su">Кросс Технолоджис</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=saveit.pro">SaveIT</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=npo-echelon.ru">Эшелон</a></td></tr><tr><td><img src="/assets/uploads/Рейтинг-B.png" alt="" class="wp-image-73664"/></td><td><a href="https://www.ssllabs.com/ssltest/analyze.html?d=www.kaspersky.ru">Лаборатория Касперского</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=softline.ru">Softline</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=infosec.ru">Информзащита</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=infotecs.ru">ИнфоТеКС</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=jet.su">Инфосистемы Джет</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=croc.ru">Крок</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=lanit.ru">Ланит</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=dialognauka.ru">ДиалогНаука</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=mascom.ru">Маском</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=swemel.ru">Свемел</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=aktiv-company.ru">Актив-софт</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=syssoft.ru">Системный Софт</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=gardatech.ru">Гарда Технологии</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=xcom.ru">X-Com</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=s-terra.ru">С-Терра СиЭсПи</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=astral.ru">Астрал</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=ntc-vulkan.ru">НТЦ Вулкан</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=confident.ru">Конфидент</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=secret-net.ru">ЦИБ (Центр Информационной Безопасности)</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=ancud.ru">Анкад</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=nvg.ru">Энвижн Груп</a></td></tr><tr><td><img src="/assets/uploads/Нет-сертификата.png" alt="" class="wp-image-73665"/></td><td><a href="https://www.ssllabs.com/ssltest/analyze.html?d=itgrp.ru">ITG (Inline Technologies Group)</a><br /><a href="https://www.ssllabs.com/ssltest/analyze.html?d=amt.ru">АМТ-Груп</a></td></tr></tbody></table></figure>
<!-- /wp:table -->


Как видно, только у 7 из 30 компаний рейтинг <strong>A</strong>, у большинства - лишь <strong>B</strong>. Две компании, вообще не использующие в 2020 году  SSL-сертификат на корпоративном сайте, стоят несколько особняком.



В целом - это очень неплохие результаты, учитывая, что <a href="https://github.com/ssllabs/research/wiki/SSL-Server-Rating-Guide">рейтинг может быть</a> и <strong>С</strong>, и <strong>D</strong>, и <strong>E</strong>, <a href="https://www.ssllabs.com/ssltest/analyze.html?d=www.rzd.ru">и даже <strong>F</strong></a>.



В любом случае, не хочу сказать, что по оценке, выдаваемой SSL Server Test, можно релевантно оценивать наличие компетенций у компании, хотя забавно было бы увидеть в Техническом Задании, например, на <a href="https://pentest.ussc.ru">тестирование на проникновение</a> в требованиях к исполнителю ограничение по минимальному рейтингу Qualys SSL Labs собственного сайта исполнителя =)



Шучу, конечно. В конце концов, задача упомянутых выше сайтов - лишь представлять компанию-владельца, и вряд ли какие-то существенные данные, кроме разве что электронной почты в формах обратной связи, с их помощью собираются и обрабатываются.



С другой стороны, корректная настройка сайта для получения <strong>A+</strong> и тем более <strong>А</strong> настолько несложная, что даже <a href="https://www.ssllabs.com/ssltest/analyze.html?d=zlonov.ru">у меня это получилось сделать</a> для собственного сайта ZLONOV.ru.


<!-- wp:image {"align":"center","id":73903,"sizeSlug":"large"} -->
<div class="wp-block-image"><figure class="aligncenter size-large"><img src="/assets/uploads/Рейтинг-сайта-ZLONOV.ru_-1024x674.png" alt="" class="wp-image-73903"/><figcaption>Рейтинг сайта ZLONOV.ru при сканировании Qualys SSL Labs</figcaption></figure></div>
<!-- /wp:image -->


Кстати, на сайте Qualys можно проверить не только сервер, но и собственный клиент: <a href="https://clienttest.ssllabs.com:8443/ssltest/viewMyClient.html">SSL Client Test</a>.

