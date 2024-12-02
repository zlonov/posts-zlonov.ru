---
layout: single
title: 'Официальные уведомления ИТ, ИБ и АСУ ТП производителей по поводу их работы в России'
date: 2022-03-11

tags: ['Accenture', 'Acer', 'Acronis', 'Akamai', 'Algosec', 'Arbor', 'Avast', 'Barracuda Networks', 'Canonical', 'Cisco', 'Cloudera', 'Cloudflare', 'Deloitte', 'Docker', 'Elastic', 'EPAM', 'Epson', 'Ericsson', 'ESET', 'EY', 'Fortinet', 'Fujitsu', 'General Electric', 'Hitachi', 'Honeywell', 'HP', 'IBM', 'Imperva', 'Intel', 'Intuit', 'IONOS', 'Juniper', 'KPMG', 'Logitech', 'Mailchimp', 'Microsoft', 'MikroTik', 'NEC', 'NETSCOUT', 'Nokia', 'Norton', 'Nozomi Networks', 'Oracle', 'Percona', 'PwC', 'Red Hat', 'Salesforce', 'SAP', 'Sharp', 'Siemens', 'Schneider Electric', 'Slack', 'Spotify', 'SUSE', 'Toshiba', 'UserGate', 'Veeam', 'VMware', 'Xerox', 'Zabbix', 'ИнфоТеКС', 'Киберпротект', 'Код Безопасности', 'С-Терра']

categories: ["Политика", "ИБ АСУ ТП", "Средства защиты"]

toc: true
toc_label: "Содержание"
toc_icon: "cog"

header:
    teaser: /assets/images/2022/Russia.jpg
    overlay_image: /assets/images/2022/Russia.jpg
    show_overlay_excerpt: false
    overlay_filter: 0.25 # same as adding an opacity of 0.5 to a black background
last_modified_at: 2022-04-12

sidebar:
  - title: "Ссылки по теме"
    text: " - [Список российских альтернатив популярным сервисам](https://www.pachca.com/alternatives)"
  - title: ""
    text: " - [Список компаний, которые ввели ограничения или покинули российский рынок](https://всезапомним.рф)"
  - title: ""
    text: " - [Какие зарубежные ИБ-компании приостановили бизнес в России?](https://lukatsky.ru/sundries/kakie-zarubezhnye-ib-kompanii-priostanovili-biznes-v-rossii.html)"
  - title: ""
    text: " - [Каталог отечественного софта для импортозамещения от АРПП](https://catalog.arppsoft.ru/replacement)"
  - title: ""
    text: " - [Перечень иностранных компаний, ограничивших свою деятельность на территории Российской Федерации](https://safe-surf.ru/specialists/article/5298/678327/)"

canonical_url: "https://zlonov.com/vendors-official-announcements/"    
---

Неполнота информации часто рождает слухи. Ниже собрана (пополняемая) подборка пресс-релизов и постов в соцмедиа производителей с их заявлениями о принятых решениях по продажам в России. Не все ссылки доступны с российских IP-адресов. Публикации в отечественных и зарубежных СМИ как достоверный источник не рассматриваются - только официальные сайты, блоги и аккаунты в социальных сетях. Добавляйте, пожалуйста, в комментариях не вошедшие в перечень ссылки.

**Добавлено 14.03.2022** - Cloudflare, Docker, ESET, Epson, Hitachi, Logitech, MikroTik, Nokia, SUSE
{: .notice}

**Добавлено 16.03.2022** - Honeywell, Percona, Nozomi Networks, Salesforce (?Slack)
{: .notice}

**Добавлено 17.03.2022** - Accenture, Akamai, Deloitte, Elastic, EY, Intuit (Mailchimp), Juniper, KPMG, NETSCOUT (Arbor), Norton, PwC, VMware
{: .notice}

**Добавлено 18.03.2022** - Schneider Electric, Xerox
{: .notice}

**Добавлено 22.03.2022** - NEC
{: .notice}

**Добавлено 23.03.2022** - Barracuda Networks, EPAM, F5, IONOS, Sharp
{: .notice}

**Добавлено 29.03.2022** - Algosec, Cloudera, Fujitsu
{: .notice}

**Добавлено 06.04.2022** - Canonical, Intel (повторное заявление)
{: .notice}

**Добавлено 07.04.2022** - Cisco (на русском языке), Spotify
{: .notice}

**Добавлено 11.04.2022** - Acer, Ericsson
{: .notice}

**Добавлено 12.04.2022** - Nokia (повторное заявление)
{: .notice}

**Добавлено 20.04.2022** - SAP (повторное заявление), Toshiba
{: .notice}

---
{% assign current_letter = "A" %}

## {{ current_letter }}

{% for i in site.data.announcements %}

{% capture i_letter %}{{i.vendor | slice: 0 }}{% endcapture %}

{% if i_letter != current_letter %}
{% assign current_letter = i_letter %}
## {{ current_letter }}
{% endif %}

### {{ i.vendor }}
{{ i.date }} _[{{ i.excerption }}]({{ i.link }})_ [[pdf]](/assets/pdfs/announcements/{{ i.vendor }}.pdf)
{% endfor %}
