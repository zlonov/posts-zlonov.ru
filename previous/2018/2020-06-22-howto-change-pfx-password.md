---
layout: single
classes: wide

title: 'Как изменить пароль .pfx файла?'
date: 2020-06-22

header:
    teaser: /assets/images/2020/PFX.png
    overlay_image: /assets/images/2020/PFX.png
    show_overlay_excerpt: true
    overlay_filter: 0.25

excerpt: 'Три простых шага для изменения пароля файла с сертификатом и закрытым ключом.'

featured-image-alt: PFX-файл
category: HowTo
tags: ['пароль', 'macOS', 'электронная почта', 'сертификат', 'экспорт']
topicID: 977
AllowComments: true
LinkedLinks: ""
---
В случае необходимости изменения пароля от имеющегося файла _.pfx_ можно воспользоваться следующими командами, введёнными в Терминале.

В примере ниже предполагается, что имеющийся сертификат и закрытый ключ хранятся в файле _cert.pfx_, а файл с новым паролем будет сохранён в файле _newcert.pfx_


1. Экспортируем имеющийся сертификат и закрытый ключ в _.pem_ файл без пароля, указывая текущий пароль:\
  > **`openssl pkcs12 -in cert.pfx -out cert.pem -nodes`**\
  > `Enter Import Password:`\
  > `MAC verified OK`

2. Конвертируем _.pem_ файл обратно в _.pfx_ c указанием нового желаемого пароля:\
  > **`openssl pkcs12 -export -out newcert.pfx -in cert.pem`**\
  > `Enter Export Password:`\
  > `Verifying - Enter Export Password:`

3. Ненужный файл _.pem_ удаляем из соображений безопасности:\
  > **`rm cert.pem`**

[Источник](http://www.1st-setup.nl/wordpress/howto-change-password-on-pfx-certificate-using-openssl/)
