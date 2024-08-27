---
weight: 500
title: "Ressources"
description: "Comment relier une ressource qui n'est pas sur le site"
icon: "launch"
date: "2024-08-27"
lastmod: "2024-08-27"
draft: false
toc: true
katex: false
---

### Qu'est ce qu'une ressource externe ?

Parfois, il peut être utile de mettre une ressource qui **n'est pas** hébergé sur le site de BackToBasics, comme une vidéo Youtube, ou un lien faire une documentation.

Pour les rendre accessible, il peut être intelligent de les mettre dans la selection des autres cours.

Pas de panique, il est super facile de mettre ça en place !


{{< tabs tabTotal="2">}}
{{% tab title="Lien vers une vidéo Youtube" %}}

## Mettre un lien vers une vidéo Youtube

Il suffit d'ajouter l'argument ```redif_url``` dans le nom, suivi de ```l'url de la vidéo```

Voici un example, pour une redifusion d'un live sur les espaces vectoriels :

```yaml
weight: 500
title: "Redif - Espaces vectoriels"
description: "Redif"
date: "2023-08-26T20:43:23+01:00"
lastmod: "2023-08-26T20:43:23+01:00"
draft: false

redif_url: "https://www.youtube.com/watch?v=YBCnqvUVjTo"
```

Hugo se chargera **automatiquement** de mettre la miniature de la vidéo.

Le titre affiché sera celui spécifié dans l'argument ```title```.

{{% /tab %}}
{{% tab title="Lien vers une ressource externe quelconque" %}}

## Mettre un lien vers une ressource externe

Il suffit d'ajouter l'argument ```ressource``` dans le nom, suivi de ```l'url de la ressource```

Voici un example, pour rediriger vers **les B2B sur moodle** :

```yaml
---
weight: 500
title: "Accès annonce moodle"
description: ""
icon: "web"
date: "2023-08-26T20:43:23+01:00"
lastmod: "2023-08-26T20:43:23+01:00"
draft: false

ressource: "https://moodle.cri.epita.fr/course/view.php?id=1491"
---


```

Ici, vous pouvez spécifier **l'icone**, **le titre** et la **description** de la ressource

{{% /tab %}}

{{< /tabs >}}
