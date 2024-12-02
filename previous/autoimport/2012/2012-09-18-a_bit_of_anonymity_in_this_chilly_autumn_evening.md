---
layout: zlonov/old_post
title: Немного анонимности в этот промозглый осенний вечер
date: 2012-09-18 20:02
author: admin
category: autoimport
tags: [privacy, интернет, информационная безопасность]
---
Как говорил мне один мудрый человек, нельзя нравится абсолютно всем: недовольные найдутся всегда, так что даже 60% - это уже хороший результат, а 80% так и вовсе отличный. На примере данного блога имел возможность лично убедиться, что посты могут вызывать у читателей прямо противоположные чувства. При этом кто-то отмалчивается, никак не реагируя на опубликованное, кто-то с открытым забралом вступает в публичную переписку/комментирование, ну а иные предпочитают писать от вымышленного либо вовсе чужого имени.

Вот только Интернет давно перестал быть анонимным и не стоит думать, что указание при комментировании в блоге чужого адреса электронной почты поможет замести следы. Как-то раз беглый анализ статистических данных счётчиков, установленных в частности, в этом блоге, позволил мне без особого труда выяснить про одного из таких комментаторов его IP-адрес и домашнего провайдера, устройство, с которого осуществлялся выход в сеть интернет и даже производителя домашней беспроводной точки. Версия браузера, операционная система, разрешение экрана, город и много другое - тоже не являются секретом (<a href="http://2ip.ru/">ссылка 1</a>, <a href="http://internet.yandex.ru/">ссылка 2</a>).

Совокупность всех этих сведений, а так же поведенческий анализ, могут позволить достаточно точно идентифицировать конкретного человека даже обычному владельцу блога, не говоря уже о провайдерах или органах правопорядка.

Вместе с тем, Интернет полон людей не желающих раскрывать своей личности и обладающих достаточными знаниями и навыками для этого. Но, что самое приятное, простые и удобные средства анонимизации доступны даже и не очень подготовленным пользователям.

В частности, <a href="http://www.torproject.us/about/corepeople.html.en">участники знаменитого проекта Tor</a> создали и регулярно поддерживают бесплатный пакет <a href="http://www.torproject.us/download/download-easy.html.en">Tor Browser Bundle </a>(доступный, кстати, и на русском языке) для платформ Windows, MacOS X, Linux и Android, включающий в себя браузер Firefox преднастроенный для работы в <a href="http://ru.wikipedia.org/wiki/Tor">сети Tor</a>.

Подключение к Tor и запуск браузера происходят автоматически:
<div><a href="http://3.bp.blogspot.com/-nQH2dOezcs0/UFifK_GAnwI/AAAAAAAABYQ/db8-fNrJJ-4/s1600/tor001.png"><img class="aligncenter" alt="" src="https://3.bp.blogspot.com/-nQH2dOezcs0/UFifK_GAnwI/AAAAAAAABYQ/db8-fNrJJ-4/s1600/tor001.png" border="0" /></a></div>
<div></div>
<div><a href="http://1.bp.blogspot.com/-nV4uD0A_GfA/UFifMwET8AI/AAAAAAAABYY/kUnUdgfE970/s1600/tor002.png"><img class="aligncenter" alt="" src="https://1.bp.blogspot.com/-nV4uD0A_GfA/UFifMwET8AI/AAAAAAAABYY/kUnUdgfE970/s640/tor002.png" width="640" height="404" border="0" /></a></div>
<div>Теперь ваш IP адрес будет определяться неверно, а кнопка "Сменить личность" позволит ещё и регулярно его менять на некий другой случайный.</div>
<div></div>
<div>Правда, настройки Tor Browser Bundle по умолчанию не позволяют оставлять комментарии с использованием Disqus (<a href="http://disqus.com/" target="_blank">система комментирования</a>, которая установлена в том числе в этом блоге), так что определённые шаги по деанонимизации придётся выполнить:</div>
<div></div>
<div><a href="http://1.bp.blogspot.com/-BrH8WrFsy6E/UFifNku6NXI/AAAAAAAABYc/2RlVwGdO9bw/s1600/tor003.png"><img class="aligncenter" alt="" src="https://1.bp.blogspot.com/-BrH8WrFsy6E/UFifNku6NXI/AAAAAAAABYc/2RlVwGdO9bw/s640/tor003.png" width="640" height="307" border="1" /></a></div>
<div></div>
<div><a href="http://3.bp.blogspot.com/-5gLScwA2GBc/UFikWMNDiBI/AAAAAAAABJc/qGUPtPYauhM/s1600/tor0045.png"><img class="aligncenter" alt="" src="https://3.bp.blogspot.com/-5gLScwA2GBc/UFikWMNDiBI/AAAAAAAABJc/qGUPtPYauhM/s1600/tor0045.png" border="2" /></a></div>
<div></div>
<div><a href="http://1.bp.blogspot.com/-Hu0a7DIe03M/UFifOKO0WhI/AAAAAAAABYk/UL-S_LyW-wk/s1600/tor004.png"><img class="aligncenter" alt="" src="https://1.bp.blogspot.com/-Hu0a7DIe03M/UFifOKO0WhI/AAAAAAAABYk/UL-S_LyW-wk/s1600/tor004.png" border="2" /></a></div>
<div></div>
<div><a href="http://3.bp.blogspot.com/-6B3CIThTWKs/UFifO22U89I/AAAAAAAABYs/nSlO__VOu6Y/s1600/tor005.png"><img class="aligncenter" alt="" src="https://3.bp.blogspot.com/-6B3CIThTWKs/UFifO22U89I/AAAAAAAABYs/nSlO__VOu6Y/s1600/tor005.png" border="2" /></a></div>
Конечно, для настоящей анонимности одного Tor Browser Bundle мало. Как справедливо указывают его создатели, для этого <a href="http://www.torproject.us/download/download-easy.html.en#warning">придётся менять свои привычки</a>.

С другой стороны, не так уж и часто порядочным людям приходится прибегать к подобным средствам. Хороший пример из жизни этого же блога - использование Tor для анонимного комментирования моего поста про новый токен JaCarta. Вот какой IP адрес был у его автора: <a href="http://www.nic.ru/whois/?query=62.113.219.6" target="_blank">62.113.219.6</a>
