---
layout: zlonov/old_post
title: Спасибо за Forbidden!
date: 2013-08-08 23:30
author: admin
category: autoimport
tags: [SpaceWeb, WordPress, благодарность, блог, информационная безопасность, сайтоведение, случай из жизни]
---
В очередной раз создам исключение из правила о том, что недовольный клиент пожалуется десяти другим, а довольный ни единого слова доброго не скажет. Сейчас скажу парочку в адрес хостинг-провайдера <a href="http://sweb.ru/" target="_blank">SpaceWeb</a> &gt;:-) В общем, дело было так... 

Попытавшись на днях зайти в админскую часть своего блога, столкнулся с <em>дружелюбной</em> надписью: <del><strong>Ты кто такой? Давай, до свидания!</strong></del>  <strong>You don't have permission to access /wp-login.php on this server</strong>.

[box type="info" style="rounded"]UPD. 28.11.2013 После обновления на серверах SpaceWeb надпись стала гласить: <strong>You don't have permission to access the requested object. It is either read-protected or not readable by the server. If you think this is a server error, please contact the webmaster. Error 403.</strong>[/box]

Свой отдельный сайт в отличие от блогов на площадках <em>livejournal.com</em>, <em>blogspot.com</em> и пр. имеет значимое для меня количество преимуществ, но и требует затрат на сопровождение. Поэтому, привычно засучив рукава, начал разбираться.

Разбор, впрочем, был не долгим. Всё объяснило найденное в полуспаме письмо самого SpaceWeb, полностью <em>признавшего</em> <em>свою вину</em>:

[quote]В связи с массовыми атаками на сайты, работающие на основе CMS Joomla и Wordpress, с целью предотвращения несанкционированного доступа были введены ограничения для входа в административные панели сайтов.

Для возможности предоставления безопасного доступа к административной панели сайта в файл .htaccess был добавлен следующий блок:
- в случае CMS Joomla (в папку administrator)
# SpaceWeb
&lt;Files index.php&gt;
order deny,allow
deny from all
#allow from My_IP
&lt;/files&gt;

- в случае CMS Wordpress:
# SpaceWeb
&lt;Files wp-login.php&gt;
order deny,allow
deny from all
#allow from My_IP
&lt;/files&gt;

Для получения доступа необходимо в секции "&lt;Files&gt;" в строке "#allow from My_IP" убрать знак "#" и вместо "My_IP" прописать внешний IP-адрес компьютера, с которого производится работа с административной панелью сайта.[/quote]

Узнать <a href="http://internet.yandex.ru/" target="_blank">свой текущий IP</a> было делом десяти секунд. Вписать его в <em>.htaccess</em> - ещё пятнадцати. Моя признательность SpaceWeb продолжается до сих пор.

К слову, всем владельцам сайтов на движках WordPress и Joomla, являющимся клиентами других, менее заботливых хостинг-провайдеров, настоятельно рекомендую прописать в <em>.htaccess</em> подобное ограничение. Такое повышение безопасности вполне уместно.
