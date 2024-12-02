---
layout: zlonov/old_post
title: '[HowTo] Как избавиться от сообщения "Microsoft Lync хочет использовать связку ключей OC_KeyContainer_..."?'
date: 2016-11-01 10:21
author: admin
category: autoimport
tags: [HowTo, macOS, macOS Sierra, Microsoft Lync, OC_KeyContainer, OS X, ошибка, сообщение]
---
Порой при обновлении OS X (например, до macOS Sierra) может возникать ошибка с постоянно всплывающим текстом сообщения "Microsoft Lync хочет использовать связку ключей OC_KeyContainer_...&lt;адрес электронной почты&gt;":

[caption id="attachment_9785" align="aligncenter" width="551"]<a href="/assets/uploads/OC_KeyContainer_.jpg"><img class="size-full wp-image-9785" src="/assets/uploads/OC_KeyContainer_.jpg" alt="OC_KeyContainer_" width="551" height="318" /></a> OC_KeyContainer_[/caption]

Чтобы избавиться от него, нужно открыть Finder, выбрать в меню <em>Переход</em> -&gt; <em>Переход к папке</em> (или нажать Cmd+Shift+G) и ввести путь "~/Library/Keychains".

По этому пути будет находиться файл "<em>OC_KeyContainer_...&lt;адрес электронной почты&gt;"</em>, который и надо удалить.

Закройте и запустите Lync, данный файл будет пересоздан заново и проблема пропадёт.
