---
layout: zlonov/old_post
title: Bitdefender USB Immunizer. Бесплатная защита компьютера от autorun вирусов.
date: 2012-08-02 12:02
author: admin
category: autoimport
tags: [Bitdefender, антивирус, информационная безопасность, обзор]
---
<div dir="ltr">
<div><a href="http://1.bp.blogspot.com/-xP0HLTUZ6T4/UBo01zuJ6RI/AAAAAAAAABQ/pKRbexURjN8/s1600/USB+Immunizer.png"><img alt="" src="https://1.bp.blogspot.com/-xP0HLTUZ6T4/UBo01zuJ6RI/AAAAAAAAABQ/pKRbexURjN8/s640/USB+Immunizer.png" width="640" height="218" border="0" /></a></div>
Многие крупные компании имеют свои собственные Лаборатории - инкубаторы идей, в рамках которых реализуют разнообразные интересные проекты, связанные с основной деятельностью, но не включаемые в итоговые версии продуктов. Очень известен, например, <a href="http://ru.wikipedia.org/wiki/%D0%9B%D0%B0%D0%B1%D0%BE%D1%80%D0%B0%D1%82%D0%BE%D1%80%D0%B8%D1%8F_Google">Google Labs</a>, закрытый, к сожалению, в октябре прошлого года. А вот аналогичная лаборатория от Bitdefender к нашей радости продолжает работать и радовать интересными и бесплатными для пользователей разработками. Сейчас у Bitdefender LABS <a href="http://labs.bitdefender.com/projects/">5 проектов</a>: Mobile Security, Bitdefender Quickscan, Bitdefender TrafficLight, Bitdefender 4Blogs (beta) и USB Immunizer, который сегодня и хотел бы рассмотреть подробнее.
<a name="more"></a>
USB Immunizer защищает флешки, карты памяти и внешние жёсткие диски от заражения их так называемыми autorun-вирусами, суть которых состоит в использовании механизма автозапуска исполняемых файлов в ОС Windows при подключении внешних носителей. Такой механизм, в частности, использовался червём Conficker, который размещал на заражённом устройстве файл автозапуска (autorun.inf), сконфигурированный так, что пользователю вместо имени исполняемого файла выводилось предложение просмотреть содержимое устройства с соответствующей иконкой:
<div><a href="http://1.bp.blogspot.com/-0xdFDyddNtE/UBo7vEubAYI/AAAAAAAAACY/Fc0_tZO7VQk/s1600/Conficker.jpg"><img alt="" src="https://1.bp.blogspot.com/-0xdFDyddNtE/UBo7vEubAYI/AAAAAAAAACY/Fc0_tZO7VQk/s320/Conficker.jpg" width="294" height="320" border="0" /></a></div>
Интерфейс у программки лаконичный и по мне так очень симпатичный:
<div><a href="http://2.bp.blogspot.com/-FM8qfmulIlg/UBo5Ia9NiZI/AAAAAAAAABg/B9pueOsukZM/s1600/001.png"><img alt="" src="https://2.bp.blogspot.com/-FM8qfmulIlg/UBo5Ia9NiZI/AAAAAAAAABg/B9pueOsukZM/s320/001.png" width="320" height="292" border="0" /></a></div>
Для иммунизации устройства достаточно подключить его к компьютеру и в окне программы нажать соответствующую иконку:
<div><a href="http://4.bp.blogspot.com/-QvAYgsL0sEs/UBo5JNuZOqI/AAAAAAAAABk/bONuMZsYFkU/s1600/002.png"><img alt="" src="https://4.bp.blogspot.com/-QvAYgsL0sEs/UBo5JNuZOqI/AAAAAAAAABk/bONuMZsYFkU/s640/002.png" width="640" height="300" border="0" /></a></div>
Защищённые устройства отображаются зелёным цветом, незащищённые - красным:
<div><a href="http://3.bp.blogspot.com/-zSdOCP6aq0Q/UBo85l2iKyI/AAAAAAAAACg/qCA0LoiIRts/s1600/003.png"><img alt="" src="https://3.bp.blogspot.com/-zSdOCP6aq0Q/UBo85l2iKyI/AAAAAAAAACg/qCA0LoiIRts/s320/003.png" width="320" height="292" border="0" /></a></div>
<div></div>
На защищённом устройстве создаётся файл autorun.inf, права на который заданы таким образом, что в среде Windows пользователь даже с правами администратора просто так его не сотрёт. Удалить файл можно только форматированием носителя или в другой операционной системе (Linux, MacOS).
<div><a href="http://4.bp.blogspot.com/-1W-Ye6cuU-k/UBo5KfQpG1I/AAAAAAAAAB0/zJ6iO9sK6xE/s1600/004.png"><img alt="" src="https://4.bp.blogspot.com/-1W-Ye6cuU-k/UBo5KfQpG1I/AAAAAAAAAB0/zJ6iO9sK6xE/s640/004.png" width="640" height="305" border="0" /></a></div>
<div><a href="http://2.bp.blogspot.com/-vXHGeNah8pA/UBo9ulWSk6I/AAAAAAAAACo/YBh2EOU_GUc/s1600/0075.png"><img alt="" src="https://2.bp.blogspot.com/-vXHGeNah8pA/UBo9ulWSk6I/AAAAAAAAACo/YBh2EOU_GUc/s400/0075.png" width="400" height="200" border="0" /></a></div>
<div><a href="http://2.bp.blogspot.com/-e-NbD4Rt7Gk/UBo5MCwdfsI/AAAAAAAAACA/bTpmA6FSduQ/s1600/005.png"><img alt="" src="https://2.bp.blogspot.com/-e-NbD4Rt7Gk/UBo5MCwdfsI/AAAAAAAAACA/bTpmA6FSduQ/s400/005.png" width="400" height="236" border="0" /></a></div>
В настройках программы можно задать автоматическую иммунизацию всех подключаемых носителей:
<div><a href="http://4.bp.blogspot.com/-9p59Ig8LscY/UBo5Mewmd4I/AAAAAAAAACE/StkY3uJFNt4/s1600/006.png"><img alt="" src="https://4.bp.blogspot.com/-9p59Ig8LscY/UBo5Mewmd4I/AAAAAAAAACE/StkY3uJFNt4/s320/006.png" width="320" height="210" border="0" /></a></div>
Иммунизированное устройство остаётся защищённым и при подключении к другим Windows-компьютерам, так что теперь можно будет с меньшей опаской давать флешки другим.

Скачать дистрибутив можно здесь: <a href="http://labs.bitdefender.com/projects/usb-immunizer/overview/">http://labs.bitdefender.com/projects/usb-immunizer/overview/</a>

</div>
