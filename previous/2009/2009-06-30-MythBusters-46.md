---
layout: zlonov/old_post
title: "Разрушители мифов. Миф №46"
date: 2009-06-30
redirect_from:
  - /razrushiteli-mifov-mif-46/
  - /2009/06/razrushiteli-mifov-mif-46/
  - /2009/06/razrushiteli-mifov-mif----46/
  - /razrushiteli-mifov-mif----46/
AllowComments: true
category: security
tags: [мифы, 'персональные данные', ПДн]
---
Давно присматриваюсь к мифам уважаемого [Алексея Лукацкого](http://lukatsky.blogspot.com/), но всё никак не доходили руки прокомментировать, а прокомментировать есть что. Начнём, например, вот с этого:

[Миф №46](http://www.bankir.ru/news/experts/lukatsky/2195845) "Снижение класса защиты ИСПДн приведет к снижению затрат на защиту персональных данных"

Для начала пробежимся по самым спорным моментам.

> В итоге мы получаем парадоксальную ситуацию - социальная сеть, в которой сотни тысяч пользователей сами раскрывают свои персональные данные и не сильно заботятся об их защищенности, должна выполнять требования более жесткие, чем поликлиника, утечка ПДн пациентов из которой может привести к гораздо более серьезным последствиям.

Не совсем так. Если в информационной системе персональных данных (ИСПДн) содержится информация о здоровье, то её класс будет первым. Это прописано в [Порядке проведения классификации информационных систем персональных данных](https://rg.ru/2008/04/12/informaciya-doc.html), а первому классу самые высокие требования. Так что данные в поликлинике нужно защищать "по максимуму".

Следующая цитата.

> Возьмем другой тип защитных средств - системы защиты от несанкционированного доступа. К их числу можно отнести такие средства как Secret Net, Аккорд, Панцирь, Броня и т.п. Они тоже практически не дифференцируются в зависимости от класса ИСПДн. Если мы возьмем, например, Secret Net 5.0, то цена решения будет одной и той же и для ИСПДн 4-го класса и для ИСПДн 1-го класса.

Немного неполная информация. Для защиты ИСПДн третьего класса (K3) достаточно использовать [Security Studio](http://securitycode.ru/products/security_studio/), который стоит дешевле, чем Secret Net.

Ну, а теперь по сути вывода.

> В итоге мы приходим к тому, что какой бы класс ИСПДн мы себе не выбрали, средства защиты для них будут одними и теми же, а значит уменьшить затраты мы не сможем.

На практике понижение класса позволяет серьёзно сэкономить как на стоимости продуктов, так и на стоимости аттестации ИСПДн. Для К3 в соответствии с требованиями даже аттестация ИСПДн не обязательна (хотя пока этому вопросу много разногласий). Единственное на чём не получится сэкономить - так это на консалтинге.

Любой специалист, выполнивший хотя бы несколько проектов по приведению информационных систем заказчика в соответствие ФЗ-152 прочитав этот миф, думаю, улыбнётся. Понижайте класс ИСПДн всеми способами, господа, и никого не слушайте =) И улыбайтесь!