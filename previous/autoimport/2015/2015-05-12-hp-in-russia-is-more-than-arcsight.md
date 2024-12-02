---
layout: zlonov/old_post
title: HP в России больше, чем ArcSight
date: 2015-05-12 17:24
author: admin
category: autoimport
tags: [ArcSight, HP, SIEM, TippingPoint, Voltage Security, информационная безопасность, мероприятие]
---
Лет 6-7 назад компания Hewlett-Packard (HP) с информационной  безопасностью не ассоциировалась почти никак, но ситуация изменилась радикально после нескольких крупных поглощений, пик которых пришёлся на 2010 год.
<iframe style="border: 1px solid #CCC; border-width: 1px; margin-bottom: 5px; max-width: 100%;" src="//www.slideshare.net/slideshow/embed_code/key/CCo5xBcPn37QaV" width="600" height="370" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" allowfullscreen="allowfullscreen"> </iframe>

<em><a href="http:///www.slideshare.net/zlonov/hps-acquisition-of-information-security-companies" target="_blank">Приобретения компании HP в сфере информационной безопасности</a></em>

Помимо приобретения SPI Dynamics, ArcSight, Fortify и TippingPoint (в составе 3Com), в 2014 году HP анонсировала <a href="http://www.bytemag.ru/articles/detail.php?ID=25779">HP Atalla</a> для шифрования данных, но в России самым известным из всех упомянутых решений, пожалуй, является всё же ArcSight. Убедиться в его популярности мне довелось лично на <em>Встрече сообщества пользователей HP ArcSight</em> - мероприятии для заказчиков и партнёров, проходившим в конце апреля.

Что ни говори, а оценивать доли рынка, <a href="https://zlonov.ru/2013/04/tsarevs_thirteen/" target="_blank">основываясь</a> на мнениях <a href="http://www.anti-malware.ru/node/11637" target="_blank">экспертов</a> (см. изображение ниже) - это одно, а видеть аудиторию, где собрались представители реальных заказчиков - совсем другое.

[caption id="attachment_6447" align="aligncenter" width="600"]<a href="/assets/uploads/Доли-рынка-SIEM-в-России.png"><img class=" wp-image-6447" src="/assets/uploads/Доли-рынка-SIEM-в-России.png" alt="Доли рынка SIEM в России" width="600" height="368" /></a> Доли рынка SIEM в России[/caption]

Вообще, судя по аудитории, темам докладов и осуждавшимся вопросам, HP ArcSight не просто хорошо представлен у нас, но и активно используется для реальных задач. За время присутствия в России (<a href="https://twitter.com/zlonov/status/592941942251589633" target="_blank">с 2007 года</a>) продукт "<a href="https://twitter.com/zlonov/status/592960804959444992" target="_blank">оброс</a>" успешными внедрениями  (МТС, ПромСвязьБанк, ГазПромБанк...) и интеграторами с требуемыми компетенциями (Диалог Наука, Информзащита, Актуальные Технологии Безопасности...).

Такое положение дел позволяет заказчикам быть уверенным в том, что они не станут "подопытными кроликами" и не получится как в <a href="https://twitter.com/zlonov/status/593036738320310272" target="_blank">прозвучавшей</a> на семинаре шутке:
<blockquote><em>- А как конкретно работает эта функция в вашем новом продукте?</em>
<em> - Пока не знаю... Давайте сделаем пилот! </em>&#x1f600;
С другой стороны, чудес не бывает и для конкретной задачи более подходящим может оказаться другой инструмент. В конце концов, заказчика может не устроить цена, сложность настройки, или избыточный функционал. Но целью поста не является сравнение HP ArcSight с конкурентами (самые активные из них иногда делают это <a href="http://www.slideshare.net/cnpo/siem-14568617" target="_blank">самостоятельно</a> - см. изображение ниже), хотя даже <a href="https://www.facebook.com/pages/Первый-Русский-SIEM/809996055719468" target="_blank">новые</a> игроки здесь появляются и тема для дискуссии есть.

[caption id="attachment_6452" align="aligncenter" width="600"]<a href="/assets/uploads/Вопросы-компании-Эшелон-к-игрокам-рынка-SIEM.png"><img class="wp-image-6452" src="/assets/uploads/Вопросы-компании-Эшелон-к-игрокам-рынка-SIEM.png" alt="Вопросы компании Эшелон к игрокам рынка SIEM" width="600" height="463" /></a> Вопросы компании Эшелон к игрокам рынка SIEM[/caption]

К слову, краткое резюме по некоторым SIEM (IBM QRadar, HP ArcSight, Комрад, Splunk, McAffee, RSA) было представлено в подкасте Аркадия Прокудина: <a href="http://it.podfm.ru/opensec/19/" target="_blank">http://it.podfm.ru/opensec/19/</a> (обсуждение начинается с 45 минуты).

Возвращаясь непосредственно к семинару, кратко перечислю некоторые заинтересовавшие меня моменты (полный список твитов доступен по тегу <a href="https://twitter.com/hashtag/семинарHP?src=hash" target="_blank">#семинарHP</a>).

Для HP ArcSight <a href="https://twitter.com/zlonov/status/593009670463315968" target="_blank">теперь</a> будет доступен модуль корреляции событий <a href="http://www8.hp.com/us/en/hp-news/press-release.html?id=1964106" target="_blank">User Behavior Analytics</a> (UBA) на базе решений <a href="http://www.securonix.com/security-intelligence-solutions/" target="_blank">Securonix</a>, позволяющий использовать данные о поведении пользователей для более интеллектуального анализа событий безопасности. Любопытная дополнительная возможность в и без того функционально небедном продукте.

Сама компания HP разделится на <a href="http://top.rbc.ru/technology_and_media/07/10/2014/5432c315cbb20f347aa9cbd5" target="_blank">два бренда</a> - HP Inc (персональные компьютеры и принтеры) и  Hewlett-Packard Enterprise с новым логотипом, куда и <a href="https://twitter.com/zlonov/status/592941336053063680" target="_blank">будет отнесено</a> направление по безопасности (Enterprise Security).

[caption id="attachment_6453" align="aligncenter" width="609"]<a href="/assets/uploads/Логотипы-HP-Inc-и-Hewlett-Packard-Enterprise.jpeg"><img class="size-full wp-image-6453" src="/assets/uploads/Логотипы-HP-Inc-и-Hewlett-Packard-Enterprise.jpeg" alt="Логотипы HP Inc и Hewlett Packard Enterprise" width="609" height="178" /></a> Логотипы HP Inc и Hewlett Packard Enterprise[/caption]

&nbsp;

В силу тематики мероприятия про другие решения компании в области безопасности говорили немного, отдельное выступление было посвящено новинке в портфеле HP - Voltage Security. Не думаю, что про него слышали многие, но тем не менее, в России есть (как минимум одно) крупное внедрение - <a href="https://twitter.com/zlonov/status/593049431613841408" target="_blank">40 000 пользователей в 26 доменах</a>. Решения Voltage Security, предназначенные для шифрования почты, данных и токенизации, очевидно, дополнят уже упомянутое выше HP Atalla.

Из относительных новинок (новинок для тех, кто не следит за решениями HP пристально) отмечу ещё продукт для борьбы с целенаправленными атаками <a href="http://www8.hp.com/ru/ru/software-solutions/apt-advanced-persistent-threat-appliance/" target="_blank">HP TippingPoint Advanced Threat Appliance</a> (ATA), <a href="http://www.iso27000.ru/press-relizy/kompaniya-trend-micro-zaklyuchila-soglashenie-o-strategicheskom-oem-partnerstve-s-hp/" target="_blank">созданный</a> в соавторстве с Trend Micro на базе их отличнейшего Trend Micro Deep Discovery, а также межсетевой экран следующего поколения <a href="http://www8.hp.com/ru/ru/software-solutions/ngfw-next-generation-firewall/" target="_blank">HP TippingPoint Next-Generation Firewall</a> (NGFW). Да-да, оказывается межсетевые экраны TippingPoint тоже существуют.

Подытоживая, скажу, что моё представление о HP как о security-вендоре после более близкого знакомства с портфелем решений поменялось с "<em>знаю, что у них есть SIEM, IPS и что-то ещё</em>" на "<em>это действительно сильный игрок со значительным портфелем решений по информационной безопасности</em>". Полный каталог HP по Enterprise Security (не так давно стал доступен на русском языке) представлен на <a href="http://www8.hp.com/ru/ru/software-solutions/enterprise-security.html" target="_blank">сайте</a> и в <a href="http://www.slideshare.net/zlonov/hp-information-security-portfolio-48050135" target="_blank">диаграмме связей (майндкарте)</a>.

P.S. Свежая аналитика от HP - о<span lang="RU">тчёт </span><a href="http://www8.hp.com/uk/en/software-solutions/cyber-risk-report-security-vulnerability/" target="_blank"><em>HP Security Research</em></a><span lang="RU"><em><a href="http://www8.hp.com/uk/en/software-solutions/cyber-risk-report-security-vulnerability/" target="_blank"> 2015</a>.</em></span>
