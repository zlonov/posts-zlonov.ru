---
title: Скрытие файлов/папок в боковой панели навигации Obsidian
tags:
  - Obsidian
  - appearance
---
Ссылки:
- https://www.reddit.com/r/ObsidianMD/comments/10dqvem/comment/j4qq0k7/
- https://help.obsidian.md/Extending+Obsidian/CSS+snippets
- https://www.reddit.com/r/ObsidianMD/comments/10dqvem/just_started_using_obsidian_is_there_a_way_to/?rdt=36196
- https://forum.obsidian.md/t/snippet-custom-css-to-hide-attachments-folder-in-every-folder/49494
- https://www.reddit.com/r/ObsidianMD/comments/1cu0gly/comment/l4httba/


To add a CSS snippet on **Desktop** ![lucide-monitor-check.svg > icon](https://publish-01.obsidian.md/access/f786db9fac45774fa4f0d8112e232d67/Attachments/icons/lucide-monitor-check.svg), follow these steps:
1. Open **Settings**.
2. Under **Appearance → CSS snippets**, select **Open snippets folder** ( ![lucide-folder-plus.svg > icon](https://publish-01.obsidian.md/access/f786db9fac45774fa4f0d8112e232d67/Attachments/icons/lucide-folder-plus.svg) ).
3. In the snippets folder, create a CSS file that contains your snippet.
4. In Obsidian, under **Appearance → CSS snippets**, select **Reload snippets** ( ![lucide-refresh-cw.svg > icon](https://publish-01.obsidian.md/access/f786db9fac45774fa4f0d8112e232d67/Attachments/icons/lucide-refresh-cw.svg) ) to see the snippet in the list.

Add `snippet.css` with this content:

```css
/* Hiding the "catalog" folder */
div[data-path='catalog'],
div[data-path='catalog'] + div.nav-folder-children
{
display: none;
}
/* Hiding the "blogs" folder */
div[data-path='blogs'],
div[data-path='blogs'] + div.nav-folder-children
{
display: none;
}
/* Hiding the "index.md" file */
div[data-path='index.md'],
div[data-path='index.md'] + div.nav-folder-children
{
display: none;
}


/* Hiding the folder */
div[data-path="Templates"], div[data-path="Templates"] + div.nav-folder-children
{
    display: none;
}
/* Hiding the paths */
div[data-path*='assets'], div[data-path*='assets'] + div.nav-folder-children
{
    display: none;
}
/* Hiding files */
div[data-path='index.md'], div[data-path='index.md'] + div.nav-folder-children
{
  display: none;
}
div[data-path='changelog.md'], div[data-path='changelog.md'] + div.nav-folder-children
{
  display: none;
}
div[data-path='principles.md'], div[data-path='principles.md'] + div.nav-folder-children
{
  display: none;
}
div[data-path='README.md'], div[data-path='README.md'] + div.nav-folder-children
{
  display: none;
}
```