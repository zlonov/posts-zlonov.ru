---
layout: zlonov/old_post
title: '[HowTo] Как добавить Яндекс.Метрику в MediaWiki'
date: 2016-07-05 17:57
author: admin
category: autoimport
tags: [CMS, HowTo, MediaWiki, скрипт, Яндекс.Метрика]
---
Для движка сайта MediaWiki есть очень простой способ добавления скрипта Яндекс.Метрики без сторонних плагинов и сложных настроек.

Достаточно в файл LocalSettings.php добавить следующий код:

<pre>$wgHooks['BeforePageDisplay'][] = 'addscripts';
 function addscripts( $out, $sk)
 {
    $out-&gt;addScript("&lt;!-- Yandex.Metrika counter --&gt;
<em>    [содержимое скрипта со всеми тегами и заменой кавычек " на слэш с кавычками \" ]</em>
    &lt;!-- /Yandex.Metrika counter --&gt;");
};</pre>
