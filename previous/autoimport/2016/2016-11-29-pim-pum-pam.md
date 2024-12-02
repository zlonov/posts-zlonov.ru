---
layout: zlonov/old_post
title: PIM, PUM, PAM!
date: 2016-11-29 06:32
author: admin
category: autoimport
tags: [Balabit, CA Technologies, Centrify, CryptoAuditor, CyberArk, FUDO, IBM, Lieberman Software, ObserveIT, PAM, PIM, PUM, SafeInspect, Shell Control Box, SSH Communication Security, Wallix, Wheel Systems, Xceedium, информационная безопасность, сертификат ФСТЭК, СКДПУ]
---
Привычна ситуация, когда для иностранного термина в области информационной безопасности нет общепринятого русского перевода и приходится использовать англоязычные понятия/аббревиатуры, а вот с <a href="https://zlonov.ru/catalog/category/pam/">контролем (действий) привилегированных пользователей</a> нет чёткости и в западных источниках.

Пожалуй, самый распространённые сокращения - те, что вынесены в заголовок этого поста:

<ul>
    <li>PIM — Privileged Identity Management;</li>
    <li>PUM — Privileged User Management;</li>
    <li>PAM — Privileged Account/Access Management.</li>
</ul>

Мне (<a href="https://www.gartner.com/doc/3398617">как и Gartner</a>) больше импонирует Privileged Access Management, а вот портал Anti-Malware этой весной делал <a href="https://www.anti-malware.ru/reviews/privileged_user_management_market_russia_2016">обзор PUM</a>. Обзор хороший, но чуть уже устаревший и, на мой взгляд, не до конца полный в части представленных на российском рынке решений.

Так, например, решение Xceedium после покупки компанией CA Technologies стало частью бандла <a href="https://zlonov.ru/catalog/ca-privileged-access-manager-bundle/">CA Privileged Access Manager Bundle</a>.

Покопавшись в архивах памяти и своей персональной базе знаний Evernote, к рассмотренным в обзоре коллег продуктам добавил ещё несколько. Все они собраны вот в этом разделе Каталога СрЗИ: <a href="https://zlonov.ru/catalog/category/pam/">Контроль привилегированных пользователей</a>.

Сначала чуть подробнее коснусь решений по контролю привилегированных пользователей c сертификатами ФСТЭК. Всё же, такая сертификация - это определённая инвестиция вендора в российский рынок и, чаще всего, демонстрация намерений активно им заниматься.

Самый ранний из действующих сертификатов ФСТЭК у решения <a href="https://zlonov.ru/catalog/cyber-ark-privileged-identity-management-and-session-management-suite-8-0/">Программный комплекс управления привилегированными учетными записями и привилегированными сессиями Cyber-Ark Privileged Identity Management and Session Management Suite 8.0</a>. Сертификат получен в ноябре 2014 года, схема сертификации - серия (т.е. можно сертифицировать любое количество изделий в зависимости от потребностей клиентов), правда, сертификат выдан только на ТУ (технические условия), без проверки на НДВ. Но, есть и ещё одна ложка дёгтя - с момента сертификации вышло уже не одно обновление, актуальная версия и вовсе 9.x (даже называется решение сейчас чуть иначе - <a href="https://zlonov.ru/catalog/cyberark-privileged-account-security/">CyberArk Privileged Account Security</a>), так что желающие использовать сертифицированный продукт CyberArk обречены работать с прошлой версией ПО.

В феврале 2015 года был получен сертификат на <a href="https://zlonov.ru/catalog/скдпу/">Программный комплекс Система контроля действий поставщиков ИТ-услуг</a>, под которым, если верить пресс-релизам, скрывается вот такой <em>зверь</em>:

<blockquote><em>СКДПУ разработана российской компанией «АйТи БАСТИОН» и создана с использованием исходного кода французской компании <a href="https://zlonov.ru/catalog/wallix-adminbastion/"><strong>Wallix</strong></a>, ОАО «НПО РусБИТех», производителя защищенной операционной системы специального назначения <strong>Astra Linux Special Edition</strong>, <strong>и собственных разработок</strong> компании «АйТи БАСТИОН»</em>.

Помимо сертификации на ТУ, у СКДУ есть и НДВ (по 4 уровню), но сертифицировано только 500 экземпляров, что, в зависимости от схемы лицензирования и архитектуры решения, может означать как потенциал в 500 проектов, так и лишь один проект, где задействованы все 500 экземпляров. Впрочем, раз процедура сертификации была однажды пройдена, можно ведь и повторить её ещё раз.

Третий из решений этого класса продукт с сертификатом ФСТЭК - это <a href="https://zlonov.ru/catalog/shell-control-box/">Программно-технический комплекс «Shell Control Box»</a> от Balabit. Тоже ТУ и тоже НДВ4, но экземпляров поменьше - только 300. Зато тут не чисто программное решение, а программно-техническое, что как-то логичнее вяжется с сертификацией ограниченного числа экземпляров.

Из остальных представленных на российском рынке PAM-решений о планах сертификации мне известно только для продукта <a href="https://zlonov.ru/catalog/safeinspect/">SafeInspect</a>. В апреле этого года <a href="http://itgrd.ru/oficialnyj-start-processa-sertifikacii-safeinspect/">были обещаны</a>: ТУ, НДВ4 и даже СВТ5. Пока ждём. Само решение позиционируется как отечественное, а в качестве прародителя по некоторым данным имеет <a href="https://www.ssh.com/products/cryptoauditor/">CryptoAuditor</a> от финской SSH Communication Security.

Про решения от IBM (<a href="https://zlonov.ru/catalog/ibm-security-privileged-identity-manager/">Security Privileged Identity Manager</a>) и Centrify (<a href="https://zlonov.ru/catalog/centrify-server-suite/">Centrify Server Suite</a>) раньше особо слышать не приходилось, но в Каталог СрЗИ всё же добавил их, тем более, что и русские описания какие-никакие, но найти удалось.

Lieberman Software (<a href="https://zlonov.ru/catalog/lieberman-software-enterprise-random-password-manager/">Enterprise Random Password Manager</a>) были замечены среди участников InfoSecurity Russia, Форума АЗИ и Уральского форума ИБ банков, так что на российском рынке они явно представлены.

С решением <a href="https://zlonov.ru/catalog/observeit/">ObserveIT</a> в своё время довелось познакомиться достаточно близко, успешные проекты в России у них есть - точно знаю.

Что же касается заключительного решения в этой категории - <a href="https://zlonov.ru/catalog/wheel-fudo-pam/">Wheel Fudo PAM</a> от Wheel Systems, то на российском рынке оно продвигается силами <a href="http://www.defsis.ru/?page=fudo">компании Дефсис</a> под своим более коротким вариантом названия: FUDO.

Общее число решений такого класса, конечно, существенно больше. Например, Forrester в отчёте Privileged Identity Management, Q3 2016 ещё называет: BeyondTrust, Bomgar, Dell, ManageEngine, Thycotic. Однако, вопрос их представленности на российском рынке остаётся открытым.
