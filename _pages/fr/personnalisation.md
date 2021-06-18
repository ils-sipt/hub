---
altLangPage: /en/settings
breadcrumbs:
  - title: "GCWeb Jekyll"
    link: "/fr/index"
dateModified: 2021-06-31
description:
title: Personnalisation
---

Personnalisez la mise en page de votre site Web, les titres et plus encore. Les paramètres se trouvent dans le fichier `_config.yml`.

## Paramètres du site

Les paramètres généraux doivent être définis dans `_config.yml`.

> **Important** : La configuration minimale requise pour configurer votre site Web serait de définir le `remote_theme: WET-BOEW/gcweb-jekyll` dans votre fichier de configuration

`title`
Type : *chaîne de caractères*

Le titre du site Web est utilisé à des fins de référencement et définit le titre de la page d'accueil.

Exemple :

```yml
# _config.yml

title: GCWeb Jekyll | Un thème Jekyll à distance avec le thème Canada.ca.
```

`description`

Type : *chaîne de caractères*

La description du site Web est utilisée uniquement à des fins de référencement.

Exemple :

```yml
# _config.yml

description: Une mise en œuvre de référence de la spécification de l'architecture du contenu et de l'information de Canada.ca, du guide de style de contenu de Canada.ca et du système de conception de Canada.ca.
```

## Paramètres de la page

Les paramètres de la page doivent être définis dans le Front Matter du contenu de la page

> **Important** :

`altLangPage`

Type : *chaîne de caractères*

Le chemin du fichier altLangPage est utilisé pour activer le lien dans la bascule de langue pour la traduction du contenu de la page alternative. S'il est omis, le lien dans la langue ne sera pas ajouté dans l'en-tête.

Exemple :

```yml
# page.md

---
altLangPage: /fr/page
---
```

`dateModified`

Type : *date*

La date permet de préciser la date de dernière modification de la page au format ISO, AAAA-MM-JJ.

Exemple:

```yml
# page.md

---
dateModified: 2021-07-01
---
```

`lang`

Type : *chaîne de caractères*

La propriété lang est utilisée pour spécifier la langue du contenu de la page. Par défaut, le modèle prend en charge "en" pour l'anglais et "fr" pour le français.

Exemple :

```yml
# page.md

---
lang: fr
---
```

`mise en page`

Type : _chaîne de caractères_

La mise en page permet de définir le modèle de page à utiliser. Quatre modèles peuvent être appelés à partir de votre page :

- *défault*
- *fluid*
- *no-container*
- *without-h1*

Exemple :

```yml
# page.md

---
layout: défault
---
```