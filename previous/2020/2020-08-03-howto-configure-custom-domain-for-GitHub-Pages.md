---
layout: single
classes: wide

title: "Как для GitHub Pages настроить собственное доменное имя?"
date: 2020-08-03
tags: [домен, 'GitHub Pages', porkbun]
categories: ['blogging', 'HowTo']
topicID: 0
AllowComments: true
LinkedLinks: ""
---
Вообще, настройка собственного доменного имени для сайта на GitHub Pages описана в справке самого сервиса:
[Configuring a custom domain for your GitHub Pages](https://docs.github.com/en/github/working-with-github-pages/configuring-a-custom-domain-for-your-github-pages-site).

Однако хотелось бы (для себя прежде всего) зафиксировать максимально краткую пошаговую инструкцию:

1. В настройках репозитория, долистав то раздела `GitHub Pages`, в поле `Custom domain` надо указать желаемое имя домена. Например, `zlonov.com`.
2. В личном кабинете своего доменного регистратора для указанного домена надо добавить CNAME запись, привязывающую этот домен к адресу `<пользователь>.github.io`, где  `<пользователь>` - это имя пользователя на GitHub.
3. Подождать. Самая трудная часть, так как хочется, чтобы всё произошло побыстрее =)
4. Командой в терминале `dig <домен> +nostats +nocomments +nocmd` убедиться, что произошло корректное обновление DNS-записей.
5. В настройках репозитория, в том же разделе `GitHub Pages` выбрать опцию `Enforce HTTPS`. Опция может появиться не сразу - иногда надо повторить шаг 3.
6. Некоторое время после включения опции `Enforce HTTPS` в насройках репозитория можно наблюдать предупреждение: _"Domain does not resolve to the GitHub Pages server. For more information, see https://help.github.com/articles/setting-up-a-custom-domain-with-github-pages/"_. В этом случае, как уже можно догадаться - опять-таки повторяем шаг 3 =) По опыту - сократить время ожидания можно, если удалить имя домена из поля `Custom domain` и тут же снова добавить. Или можно ещё сходить пообедать =)

Отдельные доменные регистраторы, к слову, упрощают для пользователей этот процесс. Например, в **porkbun** всё можно сделать простым визардом: [How to connect your domain to Github Pages](https://kb.porkbun.com/article/64-how-to-connect-your-domain-to-github-pages)
