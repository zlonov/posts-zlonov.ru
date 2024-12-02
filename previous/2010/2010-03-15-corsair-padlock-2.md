---
layout: zlonov/old_post
title: "Corsair Padlock 2"
date: 2010-03-15
redirect_from:
    - /corsair-padlock-2/
    - /2010/03/corsair-padlock-2/
AllowComments: true
category: security
tags: ['шифрование']
post_links:
  - post_link_name: Corsair PadLock 2 – флешка с возможностью мгновенного уничтожения данных
    post_link_url: https://habr.com/ru/company/acelab/blog/256287/
---
Интересное устройство предлагает компания Corsair - [USB-флешка](http://www.corsair.com/products/padlock2/default.aspx) со встроенным шифрованием.

{% include one_image_new2.html file_name="Corsair Padlock 2.jpg" image_alt="Corsair Padlock 2" %}

Устройство не требует установки программного обеспечения на рабочее место и совместимо, таким образом, с любой операционной системой: Windows, Mac OS, Linux, etc.

Для доступа к содержимому требуется ввести 4-10 цифр. Понятно, что такой уровень безопасности не является сколько-нибудь серьёзным. Вариантов комбинаций всего лишь 10^10 или примерно 2^33.2, т.е. длина ключа равно примерно 33 битам, что на сегодняшний день является уже недостаточным. Минимальная длина ключа для эффективной защиты данных сегодня должна быть 128 бит, а лучше - 256.

Вместе с тем в устройство встроен ограничитель: при многократных (точное количество не указано) попытках ввода неправильного кода, устройство блокируется на две минуты. Этого вполне достаточно для надёжной защиты от атаки методом перебора.

Как анонсирует производитель, сами данные шифруются с помощью алгоритма AES-256. Вполне возможно, что реализация шифрования имеет определённые изъяны, но в целом подход разработчика заслуживает уважения.

Единственный казус для российских потенциальных пользователей данного устройства заключается в том, что легально ввезти на территорию нашей страны партию устройств с аппаратно реализованной криптографией AES-256 не так просто.

Ну, а если окажетесь в заграничной командировке - попробуйте купить и ввезти, должно получиться: наши таможенники всё же не настолько сильно в этих вопросах подкованы =)
