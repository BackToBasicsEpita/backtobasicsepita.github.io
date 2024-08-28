---
weight: 500
title: "Comment écrire un sujet ?"
description: "Comment les sujets sont écrits ?"
icon: "fluid_med"
date: "2023-08-26T20:43:23+01:00"
lastmod: "2023-08-26T20:43:23+01:00"
draft: false
toc: true
katex: true
---

## Markdown ?

Le LaTeX c'est bien beau mais si on doit faire tous nos cours comme ça, ça nous prendrait une éternité pour couvrir tous les chapitres :c.

C'est pour ça que les sujets sont écrits en `Markdown`.
Enfin, on écrit un fichier en Markdown et `Hugo` nous permet de le transformer en page `Html` automatiquement.

Le `Markdown` est un langage de balisage (un peu comme le `Html`) créer avec comme objectif d'offrire une syntaxe facile à lire et à écrire. 

### Pourquoi faire du Markdown ?

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

### Comment faire du Markdown ?

{{< tabs tabTotal="4">}}
{{% tab title="Titre" %}}

Vous pouvez mettre des titres comment en `HTML` (`h1`, `h2`, `h3`, ...), pour cela il suffit de mettre :


```md
# h1
## h2
### h3
#### h4
##### h5
###### h6
```

Résultat :

# h1
## h2
### h3
#### h4
##### h5
###### h6
{{% /tab %}}
{{% tab title="Style" %}}

Vous pouvez aussi mettre votre texte en **Gras**, *Italique*, ~~Barré~~, pour cela, il suffit :

```md
**Texte en Gras** __Texte en Gras__
*Texte en Italique* _Texte en Italique_
~~Texte Barré~~

**Lorem *Ipsum* ~~dolor sit~~ amet**
```

**Texte en Gras** __Texte en Gras__

*Texte en Italique* _Texte en Italique_

~~Texte Barré~~

Après, libre à vous de combiner ces styles pour faire : **Lorem *Ipsum* ~~dolor sit~~ amet** 
{{% /tab %}}
{{% tab title="Citation (Texte)" %}}
Maintenant, si vous voulez citer quelqu'un, vous pouvez faire : `> citation`

> C'est véritablement utile puisque c'est joli


{{% /tab %}}

{{% tab title="Citation (Code)" %}}
Vous voulez présenter un code, alors il vous faudra choisir un `langage` et un bout de code à adapter
```md
Pour insérer du `Code` sur une seule ligne mais si votre code contient déjà des \` alors, vous pouvez mettre votre ``Code``.

Pour insérer du code sur plusieurs lignes, vous pouvez faire de cette façon.

\`\`\`python

# Vous pouvez maintenant insérer du code dans entre ces deux lignes et si vous avez précisé le langage alors, il y aura une jolie syntaxe :).

def sum(a, b):
    return a + b

\`\`\`

```

Pour insérer du `Code` sur une seule ligne mais si votre code contient déjà des ` alors, vous pouvez mettre votre ``Code``.

```python

# Vous pouvez maintenant insérer du code dans entre ces deux lignes et si vous avez précisé le langage alors, il y aura une jolie syntaxe :).

def sum(a, b):
    return a + b

```


{{% /tab %}}
{{% tab title="Liens" %}}
Il est également possible d'intégrer des liens (vers autre site, document, section)

{{% /tab %}}
{{< /tabs >}}


### Cheat-sheet Markdown

|Format|Syntaxe|Exemple|
|--------|--------|--------|
|    header   |   `#`, `#`, ...  |          `# texte en h1`|
|    Italique    |    `* *` ou `_ _`    |   `*lorem ipsum*`       |
|    Gras    |    `** **` ou `__ __`      |   `**lorem ipsum**`     |
|    Gras + italique    |    `*** ***`       |   `***lorem ipsum***`     |
|    Barré    |    `~~ ~~`       |   `~~lorem ipsum~~`     |
|    Citation (Texte)    |    `> `       |   `> lorem ipsum`     |
|    Citation (Code une ligne)           |   `` ` ` `` ou ``` `` `` ```       | ``` ``Hello`` ```|
|    Citation (Code multi-ligne)         |    \`\`\`langage retour à la ligne \`\`\`    | *cf exemple au dessus* |

