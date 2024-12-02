---
layout: zlonov/old_post
title: '[HowTo] Как просто настроить принудительную переадресацию https на сайте с WordPress?'
date: 2017-01-30 17:10
author: admin
category: autoimport
tags: [HowTo, HTTPS, SSL, WordPress, перенаправление, плагин, сертификат]
---
Вот в этом посте "<a href="https://zlonov.ru/2017/01/free-certificate/">Выбор бесплатного сертификата для собственного домена</a>" рассмотрел пару сервисов, с помощью которых можно получить для собственного домена бесплатный сертификат для перевода сайта на протокол HTTPS.

В большинстве случаев, особенно если помогает поддержка хостинг-провайдера (у меня <a href="https://fornex.com/?server=18987">Fornex</a> и проблем не возникло никаких), всё пройдёт гладко и сайт будет доступен как при доступе через http://, так и при обращении через https://

Однако, иногда случаются трудности, да и, имея сертификат, логично всех посетителей направить на вариант с https://

Проще всего это сделать с помощью специального плагина для WordPress: <a href="https://ru.wordpress.org/plugins/https-redirection/">Easy HTTPS Redirection</a>. Устанавливается он обычным образом, а настроек имеет минимум:

[caption id="attachment_10131" align="aligncenter" width="806"]<a href="/assets/uploads/Настройки-плагина-HTTPS-Redirection-Settings-для-WordPress.jpg"><img class="size-full wp-image-10131" src="/assets/uploads/Настройки-плагина-HTTPS-Redirection-Settings-для-WordPress.jpg" alt="Настройки плагина HTTPS Redirection Settings для WordPress" width="806" height="537" /></a> Настройки плагина HTTPS Redirection Settings для WordPress[/caption]

Кстати, не забудьте в разделе <em>Настройки</em> -&gt; <em>Общие</em> указать в полях "<em>Адрес WordPress (URL)</em>" и "<em>Адрес сайта (URL)</em>" адрес сайта с https://.

Если данный плагин по каким-то причинам не подойдёт, можно попробовать ещё вот эти два:

<ul>
    <li><a href="https://ru.wordpress.org/plugins/really-simple-ssl/">Really Simple SSL</a></li>
    <li><a href="https://ru.wordpress.org/plugins/wp-force-ssl/">WP Force SSL</a></li>
</ul>
