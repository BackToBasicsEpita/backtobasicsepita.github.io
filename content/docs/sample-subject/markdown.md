---
weight: 500
title: "Comment faire du markdown ?"
description: "Comment les sujets sont-ils écrits ?"
icon: "fluid_med"
date: "2023-08-26T20:43:23+01:00"
draft: false
toc: false
katex: true
---

# Markdown ?

Le LaTeX c'est bien beau mais si on doit faire tous nos cours comme ça, ça nous prendrait une éternité pour couvrir tous les chapitres :c.

C'est pour ça que les sujets sont écrits en **Markdown**.
Enfin, on écrit un fichier en Markdown et **Hugo** nous permet de le transformer en page **HTML** automatiquement.

Le **Markdown** est un langage de balisage (un peu comme le **HTML**) crée avec comme objectif d'offrir une syntaxe facile à lire et à écrire. 

# Pourquoi faire du Markdown ?

Si vous utilisez **Discord**, vous avez peut-être déjà entendu parler de **Markdown**, sinon vous allez voir que c'est vraiment très simple à prendre en main :)

Voici un exemple montrant la simplicité du **Markdown** par rapport au **HTML** et **LaTex**

{{< tabs tabTotal="3">}}
{{% tab title="HTML" %}}

**HTML demo**

```html
<p>Ce <b>Mot</b> en gras et celui-là <strong>aussi</strong>.</p>
```

> <p>Ce <b>Mot</b> en gras et celui-là <strong>aussi</strong>.</p>

{{% /tab %}}
{{% tab title="LaTex" %}}

**LaTeX demo**

```latex
$$
Ce \textbf{Mot} en gras et celui-là \textbf{aussi}.
$$
```

{{< katex >}}
$$
Ce\ \textbf{Mot}\ en\ gras\ et\ celui-là\ \textbf{aussi}.
$$
{{< /katex >}}

{{% /tab %}}
{{% tab title="Markdown" %}}

**MarkDown demo**

```
Ce **Mot** en gras et celui-là **aussi**.
```

> Ce **Mot** en gras et celui-là **aussi**.

{{% /tab %}}
{{< /tabs >}}

# Comment faire du Markdown ?

## Titre

Pour écrire des *titres* comme en **HTML** (`h1`, `h2`, `h3`, ...), il suffit de mettre :


```
# h1
## h2
### h3
#### h4
##### h5
###### h6
```

> # h1
> ## h2
> ### h3
> #### h4
> ##### h5
> ###### h6

## Style

Pour mettre le texte en **Gras**, *Italique*, ~~Barré~~, il suffit d'entourer votre texte avec :
- **Gras** : `**` ou `__`
- *Italique* : `*` ou `_`
- ~~Barré~~ : `~~`

```
**Texte en Gras** __Texte en Gras__
*Texte en Italique* _Texte en Italique_
~~Texte Barré~~
Il est possible de combiner ces styles pour faire : **Lorem *Ipsum* ~~dolor sit~~ amet**
```

> **Texte en Gras** __Texte en Gras__
> 
> *Texte en Italique* _Texte en Italique_
> 
> ~~Texte Barré~~
> 
> Il est possible de combiner ces styles pour faire : **Lorem *Ipsum* ~~dolor sit~~ amet**. 

## Citation (Texte)

Pour faire une citation, il faut faire rajouter le signe `>` devant votre texte.

```md
> citation
```

> C'est véritablement utile puisque c'est joli.



## Citation (Code)

Pour mettre en forme du code ou alors le démarquer du reste du texte,
plutôt que de le mettre en gras ou en italique, il faut faire une citation de code.
Pour cela, il suffit d'entourer son extrait de code avec des `` ` `` ou bien ``` `` ```. **Attention** à bien veiller à avoir le même nombre de `` ` `` au début et à la fin de l'extrait de texte sinon la citation ne fonctionnera pas.

Maintenant, pour présenter du code sur plusieurs lignes, il faudra choisir un `langage` et un bout de code à adapter.

````md
Pour insérer du `Code` sur une seule ligne et que le code contient déjà des ` alors, vous pouvez mettre votre ``Code``.

Pour insérer du code sur plusieurs lignes, vous pouvez faire de cette façon.

```python
# Il est maintenant possible d'insérer du code entre ces deux lignes et si un langage est précisé, alors, il y aura une jolie syntaxe :).

def sum(a, b):
    return a + b
```

````

> Pour insérer du `Code` sur une seule ligne mais si votre code contient déjà des `` ` `` alors, vous pouvez mettre votre ``Code``.
> 
> ```python
> # Vous pouvez maintenant insérer du code dans entre ces deux lignes et si vous avez précisé le langage alors, il y aura une jolie syntaxe :).
> 
> def sum(a, b):
>     return a + b
> ```

## Annotation

Une annotation en `Markdown` se fait de la manière suivante `[^n]` juste après un mot en remplaçant *n* par un nombre.

Ensuite, pour activer l'annotation, sur une nouvelle ligne, écrire : `[^n]: Ce qu'il faut marquer ici` et **Hugo** se chargera de mettre l'annotation en bas de la page.

> Voici un joli texte[^1]
[^1]: Ceci est un texte d'exemple.


## Liens

Il est également possible d'intégrer des liens (vers autre site, document, section) en faisant :

```markdown
Autre site : [Texte à afficher](https://googls.com)

Autre Page/document : [Texte à afficher](overview.md)

Section : [Texte à afficher](#cheat-sheet-markdown)
```

> Autre site : [Texte à afficher](https://googls.com)
> 
> Autre Page/document : [Texte à afficher](overview.md)
> 
> Section : [Texte à afficher](#cheat-sheet-markdown)

## Liste

Il existe plusieurs façons de faire une liste (avec ou sans ordre).
- Pour faire une liste **sans** ordre, il suffit de mettre le caractère `-`, `+` ou `*` au début de la ligne et suivi d'un espace pour créer une nouvel item.
- Pour faire une liste **avec** ordre, il suffit de mettre le numéro de l'item comme ceci : `n.` avec n le numéro de votre item. 

Exemple:
```
Liste sans ordre:
- item 1
* item 2
+ item 3
+ item 4
- item 5

Liste avec ordre:
1. item 1
2. item 2
3. item 3
```

## Paragraphe
Pour faire un nouveau paragraphe, il faudra **2 retours à la ligne**.

## Annuler le formatage
Pour annuler le formatage du markdown, il faut utiliser un `\` avant le charactère souhaité.
