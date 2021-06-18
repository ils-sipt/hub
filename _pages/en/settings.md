---
altLangPage: /fr/personnalisation
breadcrumbs:
  - title: GCWeb Jekyll
    link: /en/index
dateModified: 2021-06-31
description:
title: Settings
---
Customize your website layout, titles and more. The settings file can be found in `_config.yml`.

## Site settings
The general settings have to be set in `_config.yml`.

> **Important**: The minimum requirement to configure your website, would be to set the `remote_theme: WET-BOEW/gcweb-jekyll` in your config file

`title`
Type: *string*

The website title is used for SEO purposes and set the home page title.

Example:

```yml
# _config.yml

title: GCWeb Jekyll | A remote Jekyll theme with the Canada.ca theme.
```

`description`

Type: *string*

The website description is used for SEO purposes only.

Example:

```yml
# _config.yml

description: A reference implementation of the Canada.ca Content and Information Architecture Specification, the Canada.ca Content Style Guide and the Canada.ca Design System.
```

## Page settings

The page settings have to be set in the Front Matter of the page content

> **Important**: 

`altLangPage`

Type: *string*

The altLangPage file path is used to enable the link in the language toggle for the translation of the alternate page content. If omitted, the link in the language won't be added in the header.

Example:

```yml
# page.md

---
altLangPage: /fr/page
---
```

`dateModified`

Type: *date*

The date is used to specified the last modification date of the page in ISO format, AAAA-MM-DD.

Example:

```yml
# page.md

---
dateModified: 2021-07-01
---
```

`lang`

Type: *string*

The lang property is used to specifiy the language of the page content. By default the template support "en" for English and "fr" for French.

Example:

```yml
# page.md

---
lang: en
---
```

`layout`

Type: _string_

The page layout is used to define the page template to use. There's four templates that can be called from your page:

- *default*
- *fluid*
- *no-container*
- *without-h1*

Example:

```yml
# page.md

---
layout: default
---
```