---
layout: zlonov/old_post
title: Цикл хайпа для технологий управления учётными данными и доступом от Гартнер
date: 2018-07-20 06:12
author: admin
category: autoimport
tags: [CAC, EDRM, FIDO, Gartner, Hype cycle, IAM, IDaaS, OAuth, OpenID, PAM, SCIM, SIEM, UEBA, UMA, аналитика, аутентификация, биометрия, информационная безопасность, токен]
---
<!-- wp:paragraph {"align":"center","backgroundColor":"very-light-gray"} -->
<p style="text-align:center" class="has-background has-very-light-gray-background-color"><strong>Добавлено 07.08.2019</strong> — доступен свежий цикл хайпа за 2019 год: <a href="https://zlonov.ru/gartner/hc/#IAM">https://zlonov.ru/gartner/hc/#IAM</a>


Подумать только - понятие <a href="https://www.gartner.com/technology/research/methodologies/hype-cycle.jsp">Hype cycle</a> (цикл хайпа/ажиотажа/шумихи/зрелости/общественного интереса/ожиданий/признания) аналитическая компания Gartner ввела ещё в далёком 1995 году! И, несмотря на критику (например, <a href="https://www.linkedin.com/pulse/8-lessons-from-20-years-hype-cycles-michael-mullany">отмечается</a>, что очень немногие технологии фактически проходят через классический Hype cycle, и на практике большинство важных технологий не были идентифицированы Gartner на своём раннем этапе цикла), Циклы хайпа уверено продолжают выходить и по сей день, неизменно продаваясь за классические $1995 за штуку.
Что такое Циклы хайпа и как их читать, можно узнать в <a href="https://ru.wikipedia.org/wiki/Gartner#Цикл_хайпа">статье из Википедии</a>, а можно рассмотреть на конкретном примере - свежем июльском отчёте <a href="https://www.gartner.com/doc/3882269">Hype Cycle for Identity and Access Management (IAM) Technologies 2018</a>.
Текст самого отчёта традиционно можно разве что купить, но картинка из него <a href="https://zlonov.ru/hack-the-gartner-via-address-bar">не менее традиционно</a> вполне себе доступна:
[caption id="" align="aligncenter" width="1419"]<a href="https://www.gartner.com/resources/337700/337774/337774_0001.png"><img class="size-large" src="https://www.gartner.com/resources/337700/337774/337774_0001.png" alt="Hype Cycle for Identity and Access Management Technologies 2018" width="1419" height="939" /></a> Hype Cycle for Identity and Access Management Technologies 2018[/caption]
Вот какие технологии мы видим на кривой цикла слева направо по этапам (не ставя целью рассмотреть/описать каждую из технологий детально, постарался дать наиболее информативные ссылки на дополнительные по ним материалы):
<ul>
<li><strong>На подъёме (Innovation Trigger)</strong>
<ul>
<li><strong>UMA</strong> (<a href="https://en.wikipedia.org/wiki/User-Managed_Access">user-managed access</a>) - управляемый пользователем доступ (подробнее <a href="https://kantarainitiative.org/confluence/display/uma/UMA+FAQ">тут</a>), выход на Плато продуктивности через 5-10 лет;</li>
<li><strong>Internet of Things Authentication</strong> - аутентификация для Интернета Вещей, выход на Плато продуктивности через 2-5 лет;</li>
<li><strong>Blockchain for IAM</strong> - блокчейн для идентификации и управления доступом, выход на Плато продуктивности через 5-10 лет;</li>
<li><strong>Identity Proofing and Corroboration</strong> - проверка и подтверждение личности/учётных данных (подробнее <a href="https://www.gartner.com/doc/reprints?id=1-4Y6TJD6&amp;ct=180502&amp;st=sb">тут</a>, особенно обратите внимание на <a href="https://www.gartner.com/resources/325700/325713/325713_0001.png">схематическое пояснение</a>), выход на Плато продуктивности через 2-5 лет;</li>
<li><strong>Multiparty Computing</strong> - <a href="https://ru.wikipedia.org/wiki/Протокол_конфиденциального_вычисления">протокол конфиденциального вычисления</a> (согласен, не самый лучший вариант перевода), выход на Плато продуктивности через 5-10 лет.</li>
</ul>
</li>
<li><strong>На пике завышенных ожиданий (Peak of Inflated Expectation)</strong>
<ul>
<li><strong>FIDO Authentication Protocols</strong> - протоколы аутентификации альянса <a href="https://fidoalliance.org">FIDO (Fast IDentity Online)</a>, выход на Плато продуктивности через 2-5 лет;</li>
<li><strong>SCIM</strong> (<a href="https://en.wikipedia.org/wiki/System_for_Cross-domain_Identity_Management">System for Cross-domain Identity Management</a>) - система междоменного управления идентификацией (открытый стандарт, опубликован в RFC <a href="https://tools.ietf.org/html/rfc7643">7643</a> и <a href="https://tools.ietf.org/html/rfc7644">7644</a>), выход на Плато продуктивности через 5-10 лет;</li>
<li><strong>OpenID Connect</strong> - стандарт от OpenID Foundation (подробнее <a href="https://openid.net/connect/">тут</a>), выход на Плато продуктивности через 5-10 лет.</li>
</ul>
</li>
<li><strong>Соскальзывание во впадину разочарования (Trough of Disillusionment)</strong>
<ul>
<li><strong>Full Life Cycle API Management</strong> - <a href="https://www.gartner.com/reviews/market/full-life-cycle-api-management">системы управления полным жизненным циклом API</a> (application programming interface - интерфейс прикладного программирования), выход на Плато продуктивности менее, чем через 2 года;</li>
<li><strong>User and Entity Behavior Analytics</strong> - <a href="https://www.anti-malware.ru/analytics/Market_Analysis/user-and-entity-behavioral-analytics-ubaueba">системы поведенческого анализа</a> (или же, как любят "тонко" шутить транслитералы, УЕБА), выход на Плато продуктивности через 2-5 лет;</li>
<li><strong>Common Access Cards</strong> - универсальные карты доступа (или же единые карты сотрудника), в России не смогли "взлететь" под брендом <a href="https://ru.wikipedia.org/wiki/Универсальная_электронная_карта">Универсальная электронная карта</a>, да и по мнению Гартнер устарели, так и не достигнув Плато продуктивности;</li>
<li><strong>Externalized Authorization Management</strong> - системы управления внешними авторизациями (в целом, смысл понятен из названия, а внятного объяснения сути что-то не попалось, разве что вот <a href="https://www.nextlabs.com/solutions/technology-solutions/externalized-authorization-management/">здесь с полурекламным, правда, уклоном</a>), выход на Плато продуктивности через 5-10 лет.</li>
</ul>
</li>
<li><strong>Восхождение на склон просветления/просвещения (Slope of Enlightenment)</strong>
<ul>
<li><strong>Enterprise Digital Rights Management</strong> - корпоративные системы управления цифровыми правами (чуть подробнее <a href="https://www2.deloitte.com/ch/en/pages/risk/articles/enterprise-digital-rights-management.html">тут</a> или <a href="http://www.vaultize.com/solutions/digital-rights-management/">тут</a>), также известные как ERM – Enterprise Rights Management, IRM – Information Rights Management или RMS – Rights Management Services, выход на Плато продуктивности через 5-10 лет;</li>
<li><strong>IAM Managed Services</strong> - управляемые услуги по управлению идентификацией и доступом (да-да, выше был ещё не самый жуткий дословный перевод 😀), опять-таки устаревшая на взгляд Гартнер технология, тем не менее всё ещё <a href="https://www.ibm.com/security/services/identity-access-management">предлагаемая</a> некоторыми компаниями;</li>
<li><strong>IDaaS</strong> - управление идентификацией и доступом как услуга, технология, наиболее известной реализацией которой в России является, пожалуй, <a href="https://ru.wikipedia.org/wiki/Единая_система_идентификации_и_аутентификации">ЕСИА</a>, выход на Плато продуктивности через 2-5 лет;</li>
<li><strong>OAuth 2</strong> - вторая версия открытого протокола (RFC <a href="https://tools.ietf.org/html/rfc6749">6749</a>), близкого к уже упомянутому OpenID, но с акцентом именно на авторизации (предоставление доступа), а не на аутентификации (проверка подлинности), выход на Плато продуктивности через 2-5 лет;</li>
<li><strong>SIEM</strong> (security information and event management) - технология с не нуждающаяся в расшифровке аббревиатурой, призванная, по мнению Гартнер, упрощать работу IAM-решений за счёт интеграции с ними, но, конечно, не полностью заменять, выход на Плато продуктивности через 2-5 лет;</li>
<li><strong>Biometric Authentication Methods</strong> - наиболее часто <a href="https://www.conferencecast.tv/talk/6346/parol-umer-da-zdravstvuyet-parol">критикуемые</a> мной биометрические методы аутентификации, выход на Плато продуктивности через 2-5 лет;</li>
<li><strong>Privileged Access Management</strong> - <a href="https://zlonov.ru/pim-pum-pam/">контроль (действий) привилегированных пользователей</a>, выход на Плато продуктивности через 2-5 лет;</li>
<li><strong>X.509 Smart Hardware Tokens for User Authentication</strong> - классические токены с цифровыми сертификатами по мнению Гартнер (сюрприз-сюрприз!) устарели, хотя, положа руку на сердце, стоит отметить, что это <a href="https://zlonov.ru/private-keys-keepers-evolution/">было понятно ещё в 2013 году</a>.</li>
</ul>
</li>
<li><strong>Выход на плато продуктивности (Plateau of Productivity)</strong>
<ul>
<li><strong>Phone-as-a-Token Authentication Methods</strong> - как бы кому-то (особенно, полагаю, производителям токенов 😀) это ни не нравилось, но технология телефон-как-токен ожидается Гартнер на Плато продуктивности менее, чем через 2 года;</li>
<li><strong>Identity Governance and Administration</strong> - обобщённое название целого спектра технологий по администрированию и управлению учётными данными, введённое Гартнер в 2013 году, суть которого лучше всего описана, конечно же, самой компанией Гартнер, например, вот в этом свежем отчёте: <a href="https://www.gartner.com/doc/reprints?id=1-4S1ZVG0&amp;ct=180228">Magic Quadrant for Identity Governance and Administration 2018</a> (там же сразу можно познакомиться и с основными игроками), выход на Плато продуктивности менее, чем через 2 года;</li>
<li><strong>Virtual Directories</strong> - технология виртуальных директорий (<a href="https://www.oracle.com/technetwork/middleware/id-mgmt/index-093158.html">отдельный портал с описанием этой технологии от Oracle</a>), одна из самых старых (известна примерно с 2000 года) технологий выйдет на Плато продуктивности с точки зрения Гартнер тоже менее, чем через 2 года.</li>
</ul>
</li>
</ul>
В завершение приведу прошлогоднюю картинку из отчёта <a href="https://www.gartner.com/doc/3755464">Hype Cycle for Identity and Access Management Technologies 2017</a>. Можно наглядно посмотреть, как (по мнению Гартнер, само собой) движутся технологии по пути от своего зарождения до полноценного Продуктивного использования:
[caption id="" align="aligncenter" width="589"]<a href="https://www.gartner.com/resources/313800/313858/313858_0001.gif"><img class="size-large" src="https://www.gartner.com/resources/313800/313858/313858_0001.gif" alt="Hype Cycle for Identity and Access Management Technologies 2017" width="589" height="479" /></a> Hype Cycle for Identity and Access Management Technologies 2017[/caption]
Ещё больше Циклов хайпа <a href="https://zlonov.ru/gartner/hc/">тут</a>, квадратов Гартнер <a href="https://zlonov.ru/gartner/mq/">тут</a>, а квадратов конкретно по безопасности <a href="https://zlonov.ru/gartner/mqs/">здесь</a>.

<!-- wp:block {"ref":73025} /-->
