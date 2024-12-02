---
title: Первоначальные настройки сайта на Quartz 4
tags:
  - Quartz
  - appearance
---
Основные настройки сайта указываются в файле `quartz.config.ts`.

> [!info] Справка по теме
> https://quartz.jzhao.xyz/configuration

## Файл quartz.config.ts

Для редактирования можно использовать любой текстовый редактор либо специализированные [[Git GUI clients|редакторы кода]].

### Аналитика
- Изначально: `provider: "plausible",`
- Мой вариант: `provider: "yandex",`
- Дополнительно надо в файле `/quartz/plugins/emitters/componentResources.ts` добавить поддержку Яндекс метрики:
```
else if (cfg.analytics?.provider === "yandex") {
  componentResources.afterDOMLoaded.push(`
  (function(m,e,t,r,i,k,a){m[i]=m[i]||function(){(m[i].a=m[i].a||[]).push(arguments)};
  m[i].l=1*new Date();
  for (var j = 0; j < document.scripts.length; j++) {if (document.scripts[j].src === r) { return; }}
  k=e.createElement(t),a=e.getElementsByTagName(t)[0],k.async=1,k.src=r,a.parentNode.insertBefore(k,a)})
  (window, document, "script", "https://mc.yandex.ru/metrika/tag.js", "ym");

  ym(96251472, "init", {
       clickmap:true,
       trackLinks:true,
       accurateTrackBounce:true
  });
  `)
  }
```
### pageTitle
Название сайта, также используется при создании RSS-канала.
- Изначально: `pageTitle: "🪴 Quartz 4.0",`
- Мой вариант: `pageTitle: "🌳 ZLONOV.com",`
- Мой другой вариант: `pageTitle: "🧩 Хаб Злонова`
- Текущий вариант: `🟢 Хаб Злонова (β)`
### locale
Выбор локали (языка) для названий и форматирования даты.
- Изначально: `locale: "en-US",`
- Мой вариант: `locale: "ru-RU",`
### baseUrl
Базовый URL используется для карт сайта и RSS-каналов, которым требуется абсолютный URL-адрес. В Quartz 4, насколько это возможно, используются относительные URL-адреса, чтобы сайт работал корректно вне зависимости от места его фактического размещения.
- Изначально: `baseUrl: "quartz.jzhao.xyz",`
- Мой вариант: `baseUrl: "zlonov.com",`
- Мой другой вариант: `baseUrl: "hub.zlonov.ru",`
### typography
Шрифты. Можно выбрать любые из доступных Google Fonts. Кириллические по ссылке: https://fonts.google.com/?subset=cyrillic
- Изначально:
```
      typography: {
        header: "Schibsted Grotesk",
        body: "Source Sans Pro",
        code: "IBM Plex Mono",
      },
```
- Мой вариант:
```
      typography: {
        header: "Roboto Condensed",
        body: "Roboto Flex",
        code: "Roboto Mono",
      },
```

### colors
Цвета сайта:
- `light`: page background // фон страницы
- `lightgray`: borders // границы
- `gray`: graph links, heavier borders // ссылки на Графе, более крупные границы
- `darkgray`: body text // основной текст
- `dark`: header text and icons // текст заголовков и иконки
- `secondary`: link colour, current graph node // цвет ссылок, текущий узел Графа
- `tertiary`: hover states and visited graph nodes // состояния наведения и посещенные узлы Графа
- `highlight`: internal link background, highlighted text, highlighted lines of code // фон внутренней ссылки, выделенный текст, выделенные строки кода

- Изначально:
```
      colors: {
        lightMode: {
          light: "#faf8f8",
          lightgray: "#e5e5e5",
          gray: "#b8b8b8",
          darkgray: "#4e4e4e",
          dark: "#2b2b2b",
          secondary: "#284b63",
          tertiary: "#84a59d",
          highlight: "rgba(143, 159, 169, 0.15)",
        },
        darkMode: {
          light: "#161618",
          lightgray: "#393639",
          gray: "#646464",
          darkgray: "#d4d4d4",
          dark: "#ebebec",
          secondary: "#7b97aa",
          tertiary: "#84a59d",
          highlight: "rgba(143, 159, 169, 0.15)",
        },
      },
```
- Мой вариант:
```
      colors: {
        lightMode: {
          light: "#fdfdfd",
          lightgray: "#e5e5e5",
          gray: "#b8b8b8",
          darkgray: "#2f4f4f",
          dark: "#284e39",
          secondary: "#00a86b",
          tertiary: "#84a59d",
          highlight: "rgba(143, 159, 169, 0.15)",
        },
        darkMode: {
          light: "#161618",
          lightgray: "#393639",
          gray: "#646464",
          darkgray: "#d4d4d4",
          dark: "#ebebec",
          secondary: "#0d7952",
          tertiary: "#84a59d",
          highlight: "rgba(143, 159, 169, 0.15)",
        },
      },
```

### Plugin LaTex

Если не планируется использование [математических формул](https://quartz.jzhao.xyz/features/Latex), можно исключить это [плагин](https://quartz.jzhao.xyz/plugins/Latex):
- Изначально: `Plugin.Latex({ renderEngine: "katex" })`
- Мой вариант: ``
### Plugin transformer mermaid
Отключение поддержки mermaid сокращает размер страниц с 2,5 МБ до нескольких КБ. 
В файле `quartz/plugins/transformers/ofm.ts`:
- Изначально: `mermaid: true,`
- Мой вариант: `mermaid: false,`
## Файлы с новыми компонентами
### Файл `quartz/components/zlonovAds.tsx`
```
import { QuartzComponentConstructor, QuartzComponentProps } from "./types"
import style from "./styles/backlinks.scss"
import { classNames } from "../util/lang"

function zlonovAds({ fileData, displayClass, cfg }: QuartzComponentProps) {
    return(
    <div class={classNames(displayClass, "backlinks")}>
      <h3>Реклама (эксперимент)</h3>
    <div id="yandex_rtb_R-A-11816496-1"></div>
    </div>)
}

zlonovAds.css = style
zlonovAds.afterDOMLoaded = `
window.yaContextCb.push(() => {
    Ya.Context.AdvManager.render({
        "blockId": "R-A-11816496-1",
        "renderTo": "yandex_rtb_R-A-11816496-1"
    })
})
 `

export default (() => zlonovAds) satisfies QuartzComponentConstructor

```

### Файл `quartz/components/zlonovDetails.tsx`
```
import { QuartzComponentConstructor, QuartzComponentProps } from "./types"
import fs from 'fs';
import style from "./styles/backlinks.scss"
import { classNames } from "../util/lang"

function zlonovDetails({ fileData, displayClass, cfg }: QuartzComponentProps) {
  const title = fileData.frontmatter?.title ?? "Untitled"
  const vendor = fileData.frontmatter?.vendor
  const website = fileData.frontmatter.website
  let booklet_url = ''
  if (fs.existsSync('./content/catalog/assets/booklets/Брошюра '+title+'.pdf')) {
     booklet_url = '../assets/booklets/Брошюра-'+title.replaceAll(' ','-')+'.pdf'
  }
  let presentation_url = ''
  if (fs.existsSync('./content/catalog/assets/presentations/Презентация '+title+'.pdf')) {
    presentation_url = '../assets/presentations/Презентация-'+title.replaceAll(' ','-')+'.pdf'
  }

  let vendor_url =''
  if (vendor){vendor_url = '../catalog/vendors/'+vendor.replace(' ','-')}

  if (website || presentation_url != '' || booklet_url != ''){
    return(
    <>
    <div class={classNames(displayClass, "backlinks")}>
      <h3>Подробности</h3>
    {(website || presentation_url != '' || booklet_url != '') && (
      <p>
        <ul>
      {website && (<li><a href={website} target="_blank">🌐 Сайт</a></li>)}
      {booklet_url != '' && (<li><a href={booklet_url} target="_blank">📗 Брошюра</a></li>)}
      {presentation_url != '' && (<li><a href={presentation_url} target="_blank">🎤 Презентация</a></li>)}
      </ul>
      </p>
    )}
    </div>
    </>)
  }
  else {
    return null
  }
}

zlonovDetails.css = style
export default (() => zlonovDetails) satisfies QuartzComponentConstructor

```

### Файл `quartz/components/zlonovExcerpt.tsx`
Пока не оптимальный, но работает.
```
import { QuartzComponentConstructor, QuartzComponentProps } from "./types"
import fs from 'fs';
import { parse } from '@vanillaes/csv'

function zlonovExcerpt({ fileData, displayClass }: QuartzComponentProps) {
  const title = fileData.frontmatter?.title ?? "Untitled"
  const excerpt = fileData.frontmatter?.excerpt
  const vendor = fileData.frontmatter?.vendor
  const website = fileData.frontmatter.website

  //N,start_date,end_date,name,docs,type,lab,organ,applicant,address,support_end_date
  //N [0],start_date [1],end_date [2],name [3],docs [4],type [5],lab [6],organ [7],applicant [8],address [9],support_end_date [10]
  const certs = fileData.frontmatter?.fstec
  let parsed = ''
  if (certs && certs.length > 0){parsed = parse(fs.readFileSync('./quartz/static/csvs/certs_fstec.csv', 'utf-8'))}
  let vendor_url =''
  if (vendor){vendor_url = '../vendors/'+vendor.replaceAll(' ','-')}


  // Рег. номер сертификата соответствия [0]
  // Дата начала [1]
  // Дата окончания [2]
  // Условное наименование (индекс) [3]
  // Выполняемая функция [4]
  const certs_fsb = fileData.frontmatter?.fsb
  let parsed_fsb = ''
  if (fs.existsSync('./quartz/static/csvs/certs_fsb.csv')) {
    if (certs_fsb && certs_fsb.length > 0){parsed_fsb = parse(fs.readFileSync('./quartz/static/csvs/certs_fsb.csv', 'utf-8'))}
  }


  //[0] Регистрационный номер
  //[1] Наименование ПО
  //[2] Альтернативные названия ПО
  //[3] Класс ПО
  //[4] Код продукции
  //[5] Дата исключения
  //[6] Сайт с документацией по установке и эксплуатации ПО
  //[7] Наличие у ПО функционала поддержки работы пользователей с ограничениями по зрению
  //[8] Наличие у ПО функционала поддержки работы пользователей с ограничениями по слуху
  //[9] Соответствие ПП №325 от 23.03.2017
  //[10] Программное обеспечение относится к сфере искусственного интеллекта
  //[11] Наименование (ФИО) правообладателя
  //[12] Сокращенное наименование (ФИО) правообладателя
  //[13] Статус правообладателя
  //[14] Идентификационный номер (ИНН)
  //[15] Основной государственный регистрационный номер (ОГРН)
  //[16] Сведения об основаниях возникновения у правообладателя исключительного права на ПО
  //[17] Номер решения уполномоченного органа о включении сведений о ПО в реестр
  //[18] Дата решения уполномоченного органа о включении сведений о ПО в реестр
  //[19] Ссылка на решения уполномоченного органа о включении сведений о ПО в реестр
  //[20] Номер заявления о включении
  //[21] Дата регистрации заявления о включении
  const po_records = fileData.frontmatter?.reestr_po
  let parsed_po_records = ''
  if (fs.existsSync('./quartz/static/csvs/reestr_po.csv')) {
    if (po_records && po_records.length > 0){parsed_po_records = parse(fs.readFileSync('./quartz/static/csvs/reestr_po.csv', 'utf-8'))}
  }

//[0] Регистрационный номер
//[1] Наименование ПАК
//[2] Альтернативные названия ПАК
//[3] Класс ПАК
//[4] Код продукции
//[5] Дата исключения
//[6] Наименование (ФИО) производителя
//[7] Сокращенное наименование (ФИО) производителя
//[8] Статус производителя
//[9] Идентификационный номер (ИНН)
//[10] Основной государственный регистрационный номер (ОГРН)
//[11] Сведения об основаниях возникновения у производителя ПАК права на использование программного обеспечения в составе ПАК
//[12] Номер решения уполномоченного органа о включении сведений о ПАК в реестр
//[13] Дата решения уполномоченного органа о включении сведений о ПАК в реестр
//[14] Ссылка на решения уполномоченного органа о включении сведений о ПАК в реестр
//[15] Номер заявления о включении
//[16] Дата регистрации заявления о включении

  const pak_records = fileData.frontmatter?.reestr_pak
  let parsed_pak_records = ''
  if (fs.existsSync('./quartz/static/csvs/reestr_pak.csv')) {
    if (pak_records && pak_records.length > 0){parsed_pak_records = parse(fs.readFileSync('./quartz/static/csvs/reestr_pak.csv', 'utf-8'))}
  }

  if (excerpt || vendor || website || po_records || pak_records || certs || certs_fsb){
    let vendor_text = <a href={vendor_url}>{vendor}</a>
    return(<>
    {excerpt && (<><big>{excerpt} от компании {vendor_text}</big></>)}
    {po_records && (<>
          {po_records.map((number) =>
            {for (var item of parsed_po_records){
                  if (item[0] == number){
                      let alternative_names_text = ''
                      if (item[2] != '' && item[2] != ' ') {
                        alternative_names_text = ', альтернативные названия ПО: ' + item[2]
                      }
                      let copyright_holder = item[12]
                      if (copyright_holder = '-') {
                        copyright_holder = item[11]
                      }
                      const item_name = `${number}`
                      const record_url = 'https://reestr.digital.gov.ru/search/?q='+title.replaceAll(' ','+')+'+'+item_name
                      const display = (
                        <blockquote class="callout tip is-collapsible is-collapsed" data-callout="info" data-callout-fold="" style="max-height: 57px;">
                          <div class="callout-title">
                            <div class="callout-icon"></div>
                            <div class="callout-title-inner"><p>Запись в Реестре ПО Минцифры <a href={record_url}>№{item_name}</a> от {item[18]}</p></div>
                            <div class="fold-callout-icon"></div>
                          </div>
                          <div class="callout-content">
                          <p>
                            Наименование ПО: <strong>{item[1]}</strong><br />
                            Класс ПО: <i>{item[3]}</i><br />
                            Код продукции: <i>{item[4]}</i><br />
                            <small>Правообладатель: {copyright_holder}{alternative_names_text}.</small>
                          </p>
                        </div>
                        </blockquote>)
                      return (display)
                    };
              }
            })
          }
    </>)}
    {pak_records && (<>
          {pak_records.map((number) =>
            {for (var item of parsed_pak_records){
                  if (item[0] == number){
                      let alternative_names_text = ''
                      if (item[2] != '' && item[2] != ' ') {
                        alternative_names_text = ', альтернативные названия ПАК: ' + item[2]
                      }
                      const item_name = `${number}`
                      const record_url = 'https://reestr.digital.gov.ru/search/?q='+title.replaceAll(' ','+')+'+'+item_name
                      const display = (
                        <blockquote class="callout info is-collapsible is-collapsed" data-callout="info" data-callout-fold="" style="max-height: 57px;">
                          <div class="callout-title">
                            <div class="callout-icon"></div>
                            <div class="callout-title-inner"><p>Запись в Реестре ПАК Минцифры <a href={record_url}>№{item_name}</a> от {item[13]}</p></div>
                            <div class="fold-callout-icon"></div>
                          </div>
                          <div class="callout-content">
                          <p>
                            Наименование ПАК: <strong>{item[1]}</strong><br />
                            Класс ПАК: <i>{item[3]}</i><br />
                            Код продукции: <i>{item[4]}</i><br />
                            <small>Производитель: {item[7]}{alternative_names_text}.</small>
                          </p>
                        </div>
                        </blockquote>)
                      return (display)
                    };
              }
            })
          }
    </>)}
      {certs && (<>
            {certs.map((cert) =>
              {for (var item of parsed){
                    if (item[0] == cert){
                        let support_end_date =''
                        let cert_number = ''
                        if (item[10]){ support_end_date = ', техподдержка до ' + item[10].substr(8,2) + '.' + item[10].substr(5,2) + '.' + item[10].substr(0,4)}
                        if (fs.existsSync('./quartz/static/certs/'+item[0].replaceAll('/','-')+' '+title+'.pdf')) {
                          let cert_url = '../../static/certs/'+item[0].replaceAll('/','-')+' '+title+'.pdf'
                          cert_number = <a href={cert_url}>№{item[0]}</a>
                        }
                        else
                        {
                          cert_number = '№'+item[0]
                        }
                        const display = (
                          <blockquote class="callout tip is-collapsible is-collapsed" data-callout="info" data-callout-fold="" style="max-height: 57px;">
                            <div class="callout-title">
                              <div class="callout-icon"></div>
                              <div class="callout-title-inner"><p>Сертификат ФСТЭК {cert_number} от {item[1].substr(8,2)}.{item[1].substr(5,2)}.{item[1].substr(0,4)} (до {item[2].substr(8,2)}.{item[2].substr(5,2)}.{item[2].substr(0,4)}){support_end_date}</p></div>
                              <div class="fold-callout-icon"></div>
                            </div>
                            <div class="callout-content">
                            <p>
                              Наименование средства: <strong>{item[3]}</strong><br />
                              <i>{item[4]}</i><br />
                              <small>Схема сертификации: {item[5]}, испытательная лаборатория: {item[6]}, орган сертификации: {item[7]}, заявитель: {item[8]}.</small>
                            </p>
                          </div>
                          </blockquote>)
                        return (display)
                     };
                }
              })
            }
      </>)}
      {certs_fsb && (<>
            {certs_fsb.map((cert) =>
              {for (var item of parsed_fsb){
                    if (item[0] == cert){
                      let cert_number = ''
                      if (fs.existsSync('./quartz/static/certs/'+item[0].replaceAll('/','-')+' '+title+'.pdf')) {
                          let cert_url = '../../static/certs/'+item[0].replaceAll('/','-')+' '+title+'.pdf'
                          cert_number = <a href={cert_url}>№{item[0]}</a>
                        }
                        else
                        {
                          cert_number = '№'+item[0]
                        }
                        let display = ''
                        let display2 = ''
                        let display3 = ''
                        display = (
                          <blockquote class="callout tip is-collapsible is-collapsed" data-callout="info" data-callout-fold="" style="max-height: 57px;">
                            <div class="callout-title">
                              <div class="callout-icon"></div>
                              <div class="callout-title-inner"><p>Сертификат ФСБ {cert_number} от {item[1]} (до {item[2]})</p></div>
                              <div class="fold-callout-icon"></div>
                            </div>
                            <div class="callout-content">
                            <p>
                              <strong>{item[3]}</strong><br />
                              <i>{item[4]}</i>
                            </p>
                          </div>
                          </blockquote>)
                        display2 = callout_for_display ('Сертификат ФСБ' + cert_number +' от ' + item[1] + ' (до ' + item[2] +')','<strong>' + item[3] + '</strong><br /><i>' + item[4] + '</i>')

                        let x1 = 'Сертификат ФСБ' + cert_number +' от ' + item[1] + ' (до ' + item[2] +')' as object
                        let x2 = '<strong>' + item[3] + '</strong><br /><i>' + item[4] + '</i>' as object
                        display3 = callout_for_display (x1, x2)

                        let display4_1 = (
                          <div class="callout-title">
                          <div class="callout-icon"></div>
                          <div class="callout-title-inner"><p>Сертификат ФСБ {cert_number} от {item[1]} (до {item[2]})</p></div>
                          <div class="fold-callout-icon"></div>
                        </div>
                        )
                        let display4_2 = (
                          <div class="callout-content"><p>
                              <strong>{item[3]}</strong><br />
                              <i>{item[4]}</i>
                            </p></div>
                        )
                        let display4 =(
                          <blockquote class="callout tip is-collapsible is-collapsed" data-callout="info" data-callout-fold="" style="max-height: 57px;">
                            {display4_1}
                            {display4_2}
                          </blockquote>
                        )

                      return (display)
                     };
                }
              })
            }
      </>)}
    <hr />
    </>)
  }
  else {
    return null
  }
}

export default (() => zlonovExcerpt) satisfies QuartzComponentConstructor


function callout_for_display({callout_title}, {callout_title_inner}) {
  let display = (
    <blockquote class="callout tip is-collapsible is-collapsed" data-callout="info" data-callout-fold="" style="max-height: 57px;">
    <div class="callout-title">
      <div class="callout-icon"></div>
      <div class="callout-title-inner"><p>{callout_title}</p></div>
      <div class="fold-callout-icon"></div>
    </div>
    <div class="callout-content">
    <p>{callout_title_inner}</p></div>
  </blockquote>)
  return display
}

function testme (input: object) {
  return input
}

function callout_for_display2(callout_title = {}, callout_title_inner = {}) {
  let display = (
    <blockquote class="callout tip is-collapsible is-collapsed" data-callout="info" data-callout-fold="" style="max-height: 57px;">
    <div class="callout-title">
      <div class="callout-icon"></div>
      <div class="callout-title-inner"><p>{...callout_title}</p></div>
      <div class="fold-callout-icon"></div>
    </div>
    <div class="callout-content">
    <p>{...callout_title_inner}</p></div>
  </blockquote>)
  return display
}
```

### Файл `quartz/components/zlonovPageTitle.tsx`
```
import { pathToRoot } from "../util/path"
import { QuartzComponent, QuartzComponentConstructor, QuartzComponentProps } from "./types"
import { classNames } from "../util/lang"
import { i18n } from "../i18n"

const zlonovPageTitle: QuartzComponent = ({ fileData, cfg, displayClass }: QuartzComponentProps) => {
  const title = cfg?.pageTitle ?? i18n(cfg.locale).propertyDefaults.title
  const baseDir = pathToRoot(fileData.slug!)
  return (
    <div>
    <div class={classNames(displayClass, "zlonov-inline-block")}><img src ="https://hub.zlonov.ru/static/icon.png" height="48" width="48"/></div>
    <div class={classNames(displayClass, "zlonov-inline-block")}><h2 class={classNames(displayClass, "page-title")}><a href={baseDir}>{title}</a></h2></div>
  </div>
  )
}

zlonovPageTitle.css = `
.page-title {
  font-size: 1.75rem;
  margin: 0;
}

.zlonov-inline-block {
  display: inline-block;
  vertical-align: middle;
  margin: 5px;
}
`

export default (() => zlonovPageTitle) satisfies QuartzComponentConstructor
```
## Файл quartz.layouts.ts
### Для `components shared across all pages`
- Изначально
```
// components shared across all pages
export const sharedPageComponents: SharedLayout = {
  head: Component.Head(),
  header: [],
  afterBody: [],
  footer: Component.Footer({
    links: {
      GitHub: "https://github.com/jackyzha0/quartz",
      "Discord Community": "https://discord.gg/cRFFHYye7t",
    },
  }),
}
```
- Мой вариант
```
// components shared across all pages
export const sharedPageComponents: SharedLayout = {
  head: Component.Head(),
  header: [Component.zlonovPageTitle(), Component.MobileOnly(Component.Spacer()), Component.DesktopOnly(Component.Search()), Component.Darkmode(),],
  afterBody: [],
  footer: Component.Footer({
    links: {
      Telegram: "https://t.me/zlonov",
      "ZLONOV.ru": "https://ZLONOV.ru",
      GitFlic: "https://gitflic.ru/user/zlonov",
      GitHub: "https://github.com/zlonov/",
    },
  }),
}
```

### Для `components for pages that display a single page (e.g. a single note)`
- Изначально
```
// components for pages that display a single page (e.g. a single note)
export const defaultContentPageLayout: PageLayout = {
  beforeBody: [
    Component.Breadcrumbs(),
    Component.ArticleTitle(),
    Component.ContentMeta(),
    Component.TagList(),
  ],
  left: [
    Component.PageTitle(),
    Component.MobileOnly(Component.Spacer()),
    Component.Search(),
    Component.Darkmode(),
    Component.DesktopOnly(Component.Explorer()),
  ],
  right: [
    Component.Graph(),
    Component.DesktopOnly(Component.TableOfContents()),
    Component.Backlinks(),
  ],
}
```
- Мой вариант
```
// components for pages that display a single page (e.g. a single note)
export const defaultContentPageLayout: PageLayout = {
  beforeBody: [
    Component.Breadcrumbs({
      rootName: "Главная", // name of first/root element
      showCurrentPage: false, // whether to display the current page in the breadcrumbs
    }),
    Component.ArticleTitle(),
    Component.ContentMeta(),
    Component.TagList(),
    Component.zlonovExcerpt(),
  ],
  left: [],
  right: [
    Component.DesktopOnly(Component.zlonovDetails()),
    Component.DesktopOnly(Component.TableOfContents()),
    Component.DesktopOnly(Component.RecentNotes({
        title: "Недавние НПА",
        limit: 2,
        filter: (f) =>
          f.slug!.startsWith("laws/") && !f.frontmatter?.noindex && !f.slug.includes("index"),
        })),
    Component.DesktopOnly((Component.RecentNotes({
        title: "Недавние новости",
        limit: 2,
        filter: (f) =>
          f.slug!.startsWith("catalog/news/") && !f.frontmatter?.noindex && !f.slug.includes("index"),
        }))),
    Component.MobileOnly(Component.zlonovAds()),
  ],
  afterBody: [
    Component.MobileOnly(Component.zlonovDetails()),
    Component.Backlinks(),
    Component.DesktopOnly(Component.zlonovAds()),
  ],
}
```

### Для `components for pages that display lists of pages  (e.g. tags or folders)`
- Изначально
```
// components for pages that display lists of pages  (e.g. tags or folders)
export const defaultListPageLayout: PageLayout = {
  beforeBody: [Component.Breadcrumbs(), Component.ArticleTitle(), Component.ContentMeta()],
  left: [
    Component.PageTitle(),
    Component.MobileOnly(Component.Spacer()),
    Component.Search(),
    Component.Darkmode(),
    Component.DesktopOnly(Component.Explorer()),
  ],
  right: [],
}
```
- Мой вариант
```
// components for pages that display lists of pages  (e.g. tags or folders)
export const defaultListPageLayout: PageLayout = {
  beforeBody: [Component.Breadcrumbs(), Component.ArticleTitle(), Component.ContentMeta()],
  left: [],
  right: [],
}
```

## Файл quartz/styles/variables.scss
- Изначально
```
$breakpoints: (
  mobile: 800px,
  desktop: 1200px,
);

$mobile: "(max-width: #{map-get($breakpoints, mobile)})";
$tablet: "(min-width: #{map-get($breakpoints, mobile)}) and (max-width: #{map-get($breakpoints, desktop)})";
$desktop: "(min-width: #{map-get($breakpoints, desktop)})";

$pageWidth: #{map-get($breakpoints, mobile)};
$sidePanelWidth: 320px; //380px;
$topSpacing: 6rem;
$boldWeight: 700;
$semiBoldWeight: 600;
$normalWeight: 400;

$mobileGrid: (
  templateRows: "auto auto auto auto auto",
  templateColumns: "auto",
  rowGap: "5px",
  columnGap: "5px",
  templateAreas:
    '"grid-sidebar-left"\
      "grid-header"\
      "grid-center"\
      "grid-sidebar-right"\
      "grid-footer"',
);
$tabletGrid: (
  templateRows: "auto auto auto auto",
  templateColumns: "#{$sidePanelWidth} auto",
  rowGap: "5px",
  columnGap: "5px",
  templateAreas:
    '"grid-sidebar-left grid-header"\
      "grid-sidebar-left grid-center"\
      "grid-sidebar-left grid-sidebar-right"\
      "grid-sidebar-left grid-footer"',
);
$desktopGrid: (
  templateRows: "auto auto auto",
  templateColumns: "#{$sidePanelWidth} auto #{$sidePanelWidth}",
  rowGap: "5px",
  columnGap: "5px",
  templateAreas:
    '"grid-sidebar-left grid-header grid-sidebar-right"\
      "grid-sidebar-left grid-center grid-sidebar-right"\
      "grid-sidebar-left grid-footer grid-sidebar-right"',
);
```
- Мой вариант
```
$breakpoints: (
  mobile: 800px,
  desktop: 1200px,
);

$mobile: "(max-width: #{map-get($breakpoints, mobile)})";
$tablet: "(min-width: #{map-get($breakpoints, mobile)}) and (max-width: #{map-get($breakpoints, desktop)})";
$desktop: "(min-width: #{map-get($breakpoints, desktop)})";

$pageWidth: #{map-get($breakpoints, mobile)};
$sidePanelWidth: 320px; //380px;
$sidePanelLeftWidth: 10px;
$sidePanelRightWidth: 320px; //380px;
$topSpacing: 2rem;
$boldWeight: 700;
$semiBoldWeight: 600;
$normalWeight: 400;

$mobileGrid: (
  templateRows: "auto auto auto auto auto",
  templateColumns: "auto",
  rowGap: "5px",
  columnGap: "5px",
  templateAreas:
    '"grid-sidebar-left"\
      "grid-header"\
      "grid-center"\
      "grid-sidebar-right"\
      "grid-footer"',
);
$tabletGrid: (
  templateRows: "auto auto auto auto",
  templateColumns: "#{$sidePanelLeftWidth} auto",
  rowGap: "5px",
  columnGap: "5px",
  templateAreas:
    '"grid-sidebar-left grid-header"\
      "grid-sidebar-left grid-center"\
      "grid-sidebar-left grid-sidebar-right"\
      "grid-sidebar-left grid-footer"',
);
$desktopGrid: (
  templateRows: "auto auto auto",
  templateColumns: "#{$sidePanelLeftWidth} auto #{$sidePanelRightWidth}",
  rowGap: "5px",
  columnGap: "5px",
  templateAreas:
    '"grid-sidebar-left grid-header grid-sidebar-right"\
      "grid-sidebar-left grid-center grid-sidebar-right"\
      "grid-sidebar-left grid-footer grid-sidebar-right"',
);
```