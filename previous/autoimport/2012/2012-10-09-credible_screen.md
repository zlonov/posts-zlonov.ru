---
layout: zlonov/old_post
title: Экран, вызывающий доверие
date: 2012-10-09 16:00
author: admin
category: autoimport
tags: [информационная безопасность, обзор, трастскрин, ЭЦП]
---
<div dir="ltr">

Полгода назад я <a href="http://zlonov.blogspot.com/2012/02/blog-post_20.html">написал</a> о так называемых "трастскринах" - устройствах визуального контроля подписываемого с помощью смарт-карты (или токена) документа. По итогам того поста и дискуссии в комментариях Денис Калемберг (генеральный директор SafeTech) на одном из мартовских мероприятий передал мне производимое его компанией устройство "на опыты". Вот, наконец, дошли руки его пощупать и потестировать.
<a name="more"></a>Коробка базовой модели SafeTouch (<a href="http://safe-tech.ru/index.php/products-ru">остальные пока в разработке</a>) лаконична и скромна – самое то для бизнес-девайса:
<div><a href="/assets/uploads/2012/10/SafeTouch_box.png"><img class="aligncenter size-medium wp-image-2705" alt="SafeTouch_box" src="/assets/uploads/2012/10/SafeTouch_box-300x224.png" width="300" height="224" /></a></div>
В комплекте ничего лишнего: устройство, открепляемая подставка для вертикальной установки на стол и провод для подключения к USB. Провод коротковат, но так как разъёмы стандартные (USB и USB-mini), то проблем с его заменой/удлинением быть не должно:
<div><a href="/assets/uploads/2012/10/SafeTouch_complect.jpg"><img class="aligncenter size-medium wp-image-2706" alt="SafeTouch_complect" src="/assets/uploads/2012/10/SafeTouch_complect-300x224.jpg" width="300" height="224" /></a></div>
Инструкции в коробке не обнаружилось, что для нерозничного продукта, в принципе, объяснимо, так что первым делом, как оно водится, сразу подключаем устройство к компьютеру. На короткое время экран и кнопки загорелись, показывая свою работоспособность, после чего всё погасло и SafeTouch перешёл в режим ожидания.
<div><a href="/assets/uploads/2012/10/SafeTouch_on.png"><img class="aligncenter size-medium wp-image-2707" alt="SafeTouch_on" src="/assets/uploads/2012/10/SafeTouch_on-300x224.png" width="300" height="224" /></a></div>
Через пару минут автоматически (спасибо поддержке спецификации USB CCID) установились драйвера и SafeTouch, судя по всему, стал готов к работе.
<div><a href="/assets/uploads/2012/10/SafeTouch_driver.png"><img class="aligncenter size-full wp-image-2708" alt="SafeTouch_driver" src="/assets/uploads/2012/10/SafeTouch_driver.png" width="508" height="79" /></a></div>
С устройством мне досталась и тестовая смарт-карта с уже записанным цифровым сертификатом. На её подключение SafeTouch реагировал всё тем же кратковременным включением экрана и больше ничего заметного не происходило.

Что ж, для полноценного тестирования явно нужно какое-то программное обеспечение. Пойдём на <a href="http://safe-tech.ru/">сайт разработчиков</a>. На сайте обнаружился <a href="http://safe-tech.ru/index.php/products-ru/safetouch-desc-ru/safetouch-demo-ru">специальный раздел для тестирования</a>, но для работы с ним требуется установка специального плагина для браузера (Google Chrome в моём случае).

Несколько окон "Мастера установки" и готово. Кстати, прав администратора для установки плагин не запросил, что приятно.
<div><a href="/assets/uploads/2012/10/SafeTouch_plugin.png"><img class="aligncenter size-full wp-image-2709" alt="SafeTouch_plugin" src="/assets/uploads/2012/10/SafeTouch_plugin.png" width="509" height="398" /></a></div>
Вот теперь всё подготовлено к тестам и можно приступать. Заполняем поля тестового платёжного поручения (странно, что в названии получателя можно использовать только латиницу - надеюсь, в боевой версии такого ограничения нет) и нажимаем кнопку "Подписать".
<div><a href="/assets/uploads/2012/10/SafeTouch_data_for_signing_computer.png"><img class="aligncenter  wp-image-2711" alt="SafeTouch_data_for_signing_computer" src="/assets/uploads/2012/10/SafeTouch_data_for_signing_computer.png" width="823" height="553" /></a></div>
<div><span> </span></div>
Устройство реагирует выводом содержимого ключевых полей на свой экран.
<div><a href="/assets/uploads/2012/10/SafeTouch_data_for_signing.png"><img class="aligncenter size-medium wp-image-2712" alt="SafeTouch_data_for_signing" src="/assets/uploads/2012/10/SafeTouch_data_for_signing-300x224.png" width="300" height="224" /></a></div>
Сверяем то, что видим на мониторе компьютера, с тем, что ушло на подпись в устройство, и выбираем: подписать или нет.
<div><a href="/assets/uploads/2012/10/SafeTouch_yes.png"><img class="aligncenter size-medium wp-image-2713" alt="SafeTouch_yes" src="https://i0.wp.com/zlonov.ru/wp-content/uploads/2012/10/SafeTouch_yes.png?fit=300%2C224&#038;ssl=1" width="300" height="224" /></a></div>
В зависимости от нажатой кнопки на устройстве, на мониторе компьютера видим результат подписи ("<i>14 CD C7...</i>") либо сообщение об ошибке ("<i>Error in function...</i>"), которое хочется посоветовать заменить на что-то более наглядное: "<i>Подписание отклонено</i>", например.
<div><a href="/assets/uploads/2012/10/SafeTouch_sign.png"><img class="aligncenter size-full wp-image-2714" alt="SafeTouch_sign" src="/assets/uploads/2012/10/SafeTouch_sign.png" width="457" height="200" /></a></div>
<div><a href="/assets/uploads/2012/10/SafeTouch_error.png"><img class="aligncenter size-full wp-image-2715" alt="SafeTouch_error" src="/assets/uploads/2012/10/SafeTouch_error.png" width="456" height="194" /></a>Не совсем понятным осталось - почему при одних и тех же исходных данных результат подписи получается каждый раз разный. Видимо, в подписываемые данные включается ещё и время с датой.</div>
В целом, впечатления от практического тестирования SafeTouch положительные. Экран читаемый и его яркости при стандартном офисном освещении вполне хватает. Кнопки подтверждения/отмены разного размера, цвета и выпуклости - перепутать сложно.
<div><a href="/assets/uploads/2012/10/SafeTouch_buttons.png"><img class="aligncenter size-medium wp-image-2716" alt="SafeTouch_buttons" src="/assets/uploads/2012/10/SafeTouch_buttons-300x151.png" width="300" height="151" /></a>Из-за резиновых ножек подставки устройство по столу не скользит даже при подключении/отключении смарт-карты. Отсутствие необходимости установки драйверов и простая установка плагина с правами пользователя тоже импонируют.</div>
Относительно самой процедуры тестирования можно порекомендовать чуть подробнее расписать её сценарий на сайте, чтобы было нагляднее. Но, подозреваю, что к каждому, кто получает устройство на тестирование приставляется специально обученный человек, в деталях рассказывающий, что и как нажимать и что при этом происходит - и я тут просто исключение =)

P.S. Если вдруг обратили внимание на неидеально горизонтальное расположение дисплея устройства на фотографиях - не обращайте внимания: данный экземпляр я собственноручно уронил с высоты чуть более метра (собственно, после чего и получил его в подарок) на жёсткое напольное покрытие. Так что можно считать, что и краш-тест SafeTouch прошёл успешное: согласитесь, не каждый современный гаджет после такого обращения будет нормально работать.

</div>
