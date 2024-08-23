---
weight: 500
title: "Ecrire un sujet"
description: "Comment les sujets sont écrits ?"
icon: "fluid_med"
date: "2023-08-26T20:43:23+01:00"
lastmod: "2023-08-26T20:43:23+01:00"
draft: false
toc: true
katex: true
---

### Markdown ?

Le LaTeX c'est bien beau mais si on doit faire tous nos cours comme ça, ça nous prendrait une éternité pour couvrir tous les chapitres :c.

C'est pour ça que les sujets sont écrits en `Markdown`.
Enfin, on écrit un fichier en Markdown et `Hugo` nous permet de le transformer en page `Html` automatiquement.

Le `Markdown` est un langage de balisage (un peu comme le `Html`) créer avec comme objectif d'offrire une syntaxe facile à lire et à écrire. 

#### Comment faire du Markdown ?

Si vous utilisez **Discord** alors vous avez peut-être déjà entendu parlé de `Markdown`, sinon vous allez voir que c'est vraiment très simple à prendre en main :)

Voici un exemple montrant la simplicité du `Markdown` par rapport au `Html` et `LaTex`

{{< tabs tabTotal="3">}}
{{% tab title="Html" %}}

**Html demo**

```html
<p>Ce<b>Mot</b> en gras et celui-là <strong>aussi</strong>.</p>
```

<p>Ce<b>Mot</b> en gras et celui-là <strong>aussi</strong>.</p>

{{% /tab %}}
{{% tab title="LaTex" %}}

**LaTeX demo**

```latex
Ce \textbf{Mot} en gras et celui-là \textbf{aussi}.
```

{{< katex >}}
$$
Ce\ \textbf{Mot}\ en\ gras\ et\ celui-là\ \textbf{aussi}.
$$
{{< /katex >}}

{{% /tab %}}
{{% tab title="Markdown" %}}

**MarkDown demo**

```markdown
Ce **Mot** en gras et celui-là **aussi**.
```

Ce **Mot** en gras et celui-là **aussi**.

{{% /tab %}}
{{< /tabs >}}
