---
layout: zlonov/old_post
title: 'Ваши селфи в ваших руках'
date: 2020-03-03

header:
    teaser: /assets/images/2020/Pinkman.jpeg
    overlay_image: /assets/images/2020/Pinkman.jpeg
    show_overlay_excerpt: true
    overlay_filter: 0.25 # same as adding an opacity of 0.5 to a black background
    
category: security
tags: ['63-ФЗ', 'аутсорсинг', 'случай из жизни', 'электронная подпись']
AllowComments: true
LinkedLinks: ""
---
Волею судеб близко познакомился с некоторыми особенностями оказания аутсорсинговых услуг одним из сервисов (Сервис) вот с таким красивым рекламным слоганом:

> Берём на себя бухгалтерию, юридические вопросы, общение с банками и налоговой, вы — развиваете бизнес.

Забегая вперёд констатирую - юридические вопросы "берут на себя", прямо скажем, так себе. Не ставлю своей целью дискредитировать коллег и не призываю отказаться от использования услуг этого Сервиса, но хочу в очередной раз обратить внимание на очевидное: аутсорсинг - это всё равно риски, которые нести в конечном итоге вам, "развивающим бизнес".

---
Итак, для начала небольшая преамбула.

Принятые в конце прошлого года [поправки](/laws/476-фз-от-27-12-2019) в Федеральный закон «Об электронной подписи» в числе прочего уточняют порядок проверки реальности личности обратившегося в Удостоверяющий центр.

Текущая отменяемая редакция подпункта 1) пункта 1 статьи 18 гласит:


> Статья 18. Выдача квалифицированного сертификата
> 1.При выдаче квалифицированного сертификата аккредитованный удостоверяющий центр обязан:
> **1) установить личность заявителя - физического лица, обратившегося к нему за получением квалифицированного сертификата;**

Новая вводимая редакция (привожу полностью, но для дальнейшего обсуждения важны первые два абзаца):

> Статья 18. Выдача квалифицированного сертификата

> 1.При выдаче квалифицированного сертификата аккредитованный удостоверяющий центр обязан:

> 1) в порядке, установленном настоящим Федеральным законом, **идентифицировать заявителя** - физическое лицо, обратившееся к нему за получением квалифицированного сертификата. Идентификация заявителя проводится **при его личном присутствии** или посредством идентификации заявителя **без его личного присутствия с использованием квалифицированной электронной подписи** при наличии действующего квалифицированного сертификата либо посредством идентификации заявителя - гражданина Российской Федерации с применением информационных технологий без его личного присутствия **путем предоставления информации, указанной в документе, удостоверяющем личность гражданина Российской Федерации за пределами территории Российской Федерации, содержащем электронный носитель информации с записанными на нем персональными данными владельца паспорта, включая биометрические персональные данные**, или путем предоставления **сведений из единой системы идентификации и аутентификации и единой биометрической системы** в порядке, установленном Федеральным законом от 27 июля 2006 года N 149-ФЗ "Об информации, информационных технологиях и о защите информации".

> При этом в случае, если физическое лицо для предоставления своих биометрических персональных данных в целях проведения идентификации без личного присутствия путем предоставления сведений из единой системы идентификации и аутентификации и единой биометрической системы отказывается от использования шифровальных (криптографических) средств, указанных в части 19 статьи 14.1 Федерального закона от 27 июля 2006 года N 149-ФЗ "Об информации, информационных технологиях и о защите информации", удостоверяющий центр обязан отказать такому лицу в проведении указанной идентификации.

> Устанавливаются:

> а) в отношении физического лица - фамилия, имя, а также отчество (при наличии), дата рождения, реквизиты документа, удостоверяющего личность, идентификационный номер налогоплательщика, страховой номер индивидуального лицевого счета гражданина в системе обязательного пенсионного страхования;

> б) в отношении юридического лица, зарегистрированного в соответствии с законодательством Российской Федерации, - наименование, организационно-правовая форма, идентификационный номер налогоплательщика, а также основной государственный регистрационный номер и адрес юридического лица;

> в) для юридического лица, зарегистрированного в соответствии с законодательством иностранного государства, - наименование, регистрационный номер, место регистрации и адрес юридического лица на территории государства, в котором оно зарегистрировано;

Как видно, добавлено сразу несколько вариантов для случаев проверки реальности заявителя (оставим на совести законотворцев использование термина "идентификация") без его личного присутствия.

Не будем сейчас каждый из описанных вариантов рассматривать детально, а отметим лишь два момента:

- Ни один из вариантов не предполагает использования [селфи с паспортом](http://emeliyannikov.blogspot.com/2019/06/blog-post.html);
 - Никак не уточняется по сравнению с действующей редакцией вариант проверки при личном присутствии.

---

Но вернёмся к сервису аутсорсинга.

Договор с ними для общего удобства свободно размещён на сайте и заключается путём оплаты первого счёта на предоставление права использования Сервиса. При этом далеко не все важные нюансы в Договоре детально отражены.

Конкретно в описываемом мной случае оказалось, что для начала полноценной работы необходимо... в течение суток предоставить селфи руководителя с паспортом в руках.

> Для подачи заявки нам нужен скан подписанного заявления на подключение интернет-отчётности и фото руководителя*, на котором у него в руках разворот первой страницы паспорта (только внутренний). На фото должно быть видно лицо, первую страницу паспорта.

> [...] Заполненный бланк заявления [...]. Всё заполнено, редактировать не нужно. Распечатайте его, поставьте подпись от руки и печать. Это завершающий этап подключения в сервис. После подключения отчётности ваша база 1С попадёт в работу бухгалтеру. Сейчас бухгалтер не работает в базе 1С. Поэтому, пожалуйста, отправьте документы в течение суток.

> *Примечание: В соответствии с законом о выпуске ЭЦП ФЗ-63 - [consultant.ru/...6217886574af6](http://www.consultant.ru/document/cons_doc_LAW_112701/8431d104d9d3f38ead39f587b9f6217886574af6/) аккредитованный центр (оператор интернет-отчётности) должен установить личность заявителя [...]. В данном случае фото с разворотом паспорта, как раз и будет являться подтверждением личного обращения руководителя за выпуском сертификата.

Всё дальнейшее общение приводить не буду, перейду сразу к итогу:

> **Для ведения учёта и сдачи отчётности необходим сертификат от конкретного удостоверяющего центра (УЦ), полученный через конкретного "Оператора", и для получения этого сертификата руководителю нужно сделать и выслать селфи с паспортом либо приехать в офис регистрации, чтобы на месте сделать фото с паспортом.**

Какие-либо законные основания для такого требования, а особенно "порадовало" фотографирование при личном визите, представители Сервиса не смогли предоставить. Да и в целом их позиция: "Лицензиар не несет ответственности перед Лицензиатом за действия удостоверяющего центра, оказывающего услуги в соответствии с регламентом соответствующего удостоверяющего центра".

При этом, к сожалению, коллеги даже не смогли внятно объяснить суть взаимоотношений между УЦ, Сервисом и Оператором, _"поскольку с ними подписано соглашение о неразглашении и все условия сделки конфиденциальны"_. Доходило до забавного - присылали ссылку на Политику обработки ПДн одного юрлица (УЦ), а подписать заявление предлагали в адрес совсем другого (Оператора).

Собственно, это мной для удобства чтения те, кто собрался что-то делать с селфи с паспортом, названы УЦ, Оператор и Сервис. Из ответов коллег цепочка их взаимоотношений может быть выстроена лишь приблизительно. Могу предположить, что есть некий внутренний регламент УЦ, по которому его партнёры (центры регистрации) могут принимать заявления, но при этом обязаны сфотографировать заявителя с паспортом в руках. Одним из таких центров регистрации, видимо, и является упомянутый выше Оператор, с которым в свою заключен Договор уже непосредственно Сервисом.

{% include one_image_new2.html picture_name="Схема движения селфи с паспортом" picture_path="2020/scheme.png" %}

Понимаю, что фото с паспортом в руках сейчас [никого уже не удивишь](https://yandex.ru/images/search?text=фото%20с%20паспортом), но неужели, раз уж так эта процедура с селфи необходима, нельзя было юридически грамотно всё оформить? В ходе общения даже Политики обработки персональных данных ни Сервиса ни Оператора не были предоставлены. Их просто нет в природе, как и формы согласия на обработку биометрических персональных данных?

Даже предполагать не хочу, что Сервис, Оператор и/или УЦ работают в какой-то _серой_ законодательной зоне, но по факту - предлагается некая процедура, не имеющая своего отражения ни в действующей, ни в новой редакции федерального законодательства, без детального пояснения схемы и юридически грамотного оформления.

Как там в слогане? Берём на себя юридические вопросы? Ну, не знаю... Неужели имеется в виду вот это?

> При этом так как вы являетесь нашим клиентом, у нас есть небольшая договоренность с центром регистрации, и чтобы не тратить ваше время на посещение офиса партнера, мы вам предлагаем сделать фото с паспортом по примеру в вашем офисе и предоставить его нам по любым удобным каналам связи.

А как же строгость соблюдения регламента УЦ? Принесена в жертву удобству?

В заключение несколько избранных цитат:

 - _"Мы работаем только с этим партнером, другая ЭЦП не подойдет."_
 - _"Другого способа идентификации нет."_
 - _"Это не навязывание услуги, это обязательный момент при подключении к нашему сервису, другого решения нет."_
 - _"...установить личность заявителя можно при личном посещении офиса оператора [...] там также попросят сфотографироваться с паспортом для досье. Так как эту фотографию оператор прикладывают в электронную заявку, которую отправляет в удостоверяющий центр. Никто не может выпустить на вашу компанию сертификат, пока не удостоверится в вашей личности. Делается это для вашей же безопасности."_
 - _"Так как вы выбрали способ личной подачи, они сделают фото с паспортом, которое будет загружено на сервер  [УЦ] для выпуска сертификата. Нужно понимать также, что [УЦ] подчиняется закону о ФЗ-23 о защите данных и с защищенного сервера Ваши документы никому быть переданы не могут"._
 - _"Мы вынуждены прекратить текущее обслуживания из-за невозможности продолжить работу. Мне очень жаль, я впервые с таким сталкиваюсь. Деньги будут возвращены пропорциональны неиспользованным дням."_

Деньги действительно вернули, тут к коллегам вопросов нет.