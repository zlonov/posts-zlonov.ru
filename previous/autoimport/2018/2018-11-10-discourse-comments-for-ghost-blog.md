---
layout: zlonov/old_post
title: '[HowTo] Как интегрировать в блог на Ghost комментарии от Discourse'
date: 2018-11-10 07:51
author: admin
category: autoimport
tags: [Discourse, Ghost, HowTo]
---
Ниже приведён пример последовательности действий для блога [https://blog.zlonov.ru](https://blog.zlonov.ru/) и форума с комментариями [https://ruCyberSecurity.ru](https://rucybersecurity.ru/). Публиковаться всё будет в разделе «[Комментарии блога и сайта](https://forum.zlonov.ru/c/comments)«.
1. В админке Discourse ([https://ruCyberSecurity.ru/admin/customize/embedding](https://rucybersecurity.ru/admin/customize/embedding)) добавить разрешённый хост:
	- Разрешённые хосты: *blog.zlonov.ru*
	- Опубликовать в разделе: *Комментарии блога и сайта*
	- Имя пользователя, которое будет использоваться для создания темы: *system*
	- Максимальное количество вложенных сообщений: *100*
	- Обрезать встроенные сообщения: *+*
7. Отредактировать файл *post.hbs* вашей темы Ghost (в моём случае - перейти в командную строку управления сервером с установленным Ghost и ввести *sudo nano /var/www/ghost/content/themes/casper/post.hbs)*
	- Раскомментировать секцию: *\<section class=»post-full-comments»\> \</section\>*
	- Вписать в неё встроенный код, скопированный из админки Discourse ([https://ruCyberSecurity.ru/admin/customize/embedding](https://rucybersecurity.ru/admin/customize/embedding))
			{% raw %}<div id='discourse-comments'></div>
			                <script type="text/javascript">
			                  DiscourseEmbed = { discourseUrl: 'https://ruCyberSecurity.ru/',
			                                     discourseEmbedUrl: '{{@blog.url}}{{url}}' };
			                  (function() {
			                    var d = document.createElement('script'); d.type = 'text/javascript'; d.async = true;
			                    d.src = DiscourseEmbed.discourseUrl + 'javascripts/embed.js';
			                    (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(d);
			                  })();
			                </script>{% endraw %}

	- В коде в предыдущем пункте *REPLACE\_ME* заменён на *{@blog.url}{url}*
	- Сохранить *post.hbs*
13. Перезагрузить Ghost:
	- *sudo -i -u ghost-mgr*
	- *cd /var/www/ghost*
	- *ghost restart*
Использованные материалы:
- https://webcache.googleusercontent.com/search?q=cache:llRvtq9MMhoJ:https://help.ghost.org/en-us/article/35-discourse+&cd=3&hl=ru&ct=clnk&gl=de
- https://docs.ghost.org/api/ghost-cli/restart/
