---
layout: zlonov/old_post
title: Может ли на таможне застрять партия клавиатур?
date: 2011-03-01 11:27
author: admin
category: autoimport
tags: [информационная безопасность, криптография, шифрование]
---
<div dir="ltr" trbidi="on">В моём беспроводном комплекте клавиатура+мышь+цифровой блок <a href="http://market.yandex.ru/model.xml?hid=723088&modelid=716199&clid=502">Logitech diNovo Cordless Desktop for Notebooks</a> с помощью установленного программного обеспечения Logitech SetPoint можно активировать любопытную функцию "Безопасность клавиатуры", запустив Мастер надёжного шифрования.<br /><a name="more"></a><br /><br /><div><a href="https://lh3.googleusercontent.com/-INRMiaKijbI/TWygV5PbwKI/AAAAAAAAAFA/sLUhHKEWamQ/s1600/001.png" imageanchor="1"><img border="0" height="300" src="https://lh3.googleusercontent.com/-INRMiaKijbI/TWygV5PbwKI/AAAAAAAAAFA/sLUhHKEWamQ/s400/001.png" width="400"/></a></div>
<br /><div><a href="https://lh4.googleusercontent.com/-or4RBh9C7ws/TWygWg8ZCdI/AAAAAAAAAFE/SImZLPsg5Nw/s1600/002.png" imageanchor="1"><img border="0" height="285" src="https://lh4.googleusercontent.com/-or4RBh9C7ws/TWygWg8ZCdI/AAAAAAAAAFE/SImZLPsg5Nw/s400/002.png" width="400"/></a></div>
<br /><div><a href="https://lh3.googleusercontent.com/-Pcfaa3DSJZ4/TWygWyb792I/AAAAAAAAAFI/ea8_-VQHxvo/s1600/003.png" imageanchor="1"><img border="0" height="285" src="https://lh3.googleusercontent.com/-Pcfaa3DSJZ4/TWygWyb792I/AAAAAAAAAFI/ea8_-VQHxvo/s400/003.png" width="400"/></a></div>
<br /><div><a href="https://lh6.googleusercontent.com/-Zv4gkTLzxtY/TWygXc00WaI/AAAAAAAAAFM/LsCmhr6sBPU/s1600/004.png" imageanchor="1"><img border="0" height="285" src="https://lh6.googleusercontent.com/-Zv4gkTLzxtY/TWygXc00WaI/AAAAAAAAAFM/LsCmhr6sBPU/s400/004.png" width="400"/></a></div>
<br /><div><a href="https://lh3.googleusercontent.com/-v90oKicLkXk/TWygX2SvkpI/AAAAAAAAAFQ/Ju9LUbui8wk/s1600/005.png" imageanchor="1"><img border="0" height="285" src="https://lh3.googleusercontent.com/-v90oKicLkXk/TWygX2SvkpI/AAAAAAAAAFQ/Ju9LUbui8wk/s400/005.png" width="400"/></a></div>
<br /><div><a href="https://lh5.googleusercontent.com/-FRJXN8UwDLQ/TWygYSC_-zI/AAAAAAAAAFU/zUoJstEspUU/s1600/006.png" imageanchor="1"><img border="0" height="300" src="https://lh5.googleusercontent.com/-FRJXN8UwDLQ/TWygYSC_-zI/AAAAAAAAAFU/zUoJstEspUU/s400/006.png" width="400"/></a></div>
<div><br /></div>
<div>Согласно описания, данная функция позволяет установить шифрованное соединение между клавиатурой (и цифровым блоком) и компьютером для исключения перехвата нажимаемых клавиш посторонними.</div>
<div><br /></div>
<div>Для цифрового блока предлагается ввести последовательность из 16 цифр, что даёт длину ключа = 10^16 ~ 53 бита. Такая длина ключа соответствует понятию слабой криптографии (менее 56 бит), а вот для клавиатуры нужно ввести 16 цифр и символов, что уже эквивалентно(10+26)^16 ~ 82 битам.</div>
<div><br /></div>
<div>На практике мне не известны широко распространённые алгоритмы с такой экзотической длинной ключа и, скорее всего, используется стандартный AES с ключом 128 бит. Нельзя, конечно, исключать вариант, что вводимая пользователем последовательность не целиком используется в качестве ключа, но, в любом случае, шифрование в клавиатуре и даже в цифровом блоке присутствует. Что это означает? Ровно то, что ввоз таких устройств на территорию Российской Федерации законодательно регламентируется, так что у таможенникам можно порекомендовать внимательнее приглядеться к ввозимым беспроводным клавиатурам, а не только зажигать и снимать про это клипы =)</div>
<div><br /></div>
<div></div>
<br /><div><br /></div>
<div>P.S. Вот здесь есть неплохая статья на тему ввоза: <a href="http://www.anticisco.ru/blogs/?p=161">Новые</a></div></div>
