==HTML== est un **langage de balisage.** il permet d'écrire du contenu .

-les balises de html utilises des *chevrons <>*
-les balises indiquent la nature de ce qu'elle encadrent , comme par exemple,< P></p> pour indiquer les paragraphes
-on a deux types de balises :
	*en paires* qui ont un début et une fin, et qui peuvent contenir d'autres balises en suivant une organisation hiérarchisée du types parent- enfant , et contiennent des textes , et
	l*es balises orphelines* tels que  les balises d'images comme  
	
	<img>
	
-**un fichier de contenu en HTML** - aura l'extension  `.html`

-html suit une mise en forme précise :
	
<!DOCTYPE html>
```
<html lang="fr">
    <head>
        <meta charset="utf-8">
        <title>Ma page</title>
    </head>
    <body>
        <p>Ceci est le contenu de mon premier paragraphe</p>
        <p>Ceci est le contenu de mon deuxième paragraphe</p>
    </body>
</html>
```
- La balise `**<title>**`n'affiche rien sur la page web, elle affiche le titre de la page dans l'onglet du navigateur.



Le texte affiché sur une page web est compris entre les balises **`<body> </body>:

.Les balises **`<p> </p>`** permettent de délimiter des paragraphes en HTML :<!DOCTYPE html>
```
<html lang="fr">
    <head>
        <meta charset="utf-8">
        <title>Ma page</title>
    </head>
    <body>
        <p>Ceci est le contenu de mon premier paragraphe</p>
        <p>Ceci est le contenu de mon deuxième paragraphe</p>
    </body>
</html>
```
.Pour revenir à la ligne, on utilise la balise orpheline  `<br>` (pour _break_), on n'a donc pas besoin de la fermer:<!DOCTYPE html>
```
<html lang="fr">
    <head>
        <meta charset="utf-8">
        <title>Ma page</title>
    </head>
    <body>
        <p>Ceci est le contenu de mon premier paragraphe, <br>dont le contenu est particulièrement long.</p>
        <p>Ceci est le contenu de mon deuxième paragraphe</p>
    </body>
</html>
```
donc 'ici grace a br , le texte revient à la ligne sans changer de paragraphe.Alors que pour le deuxieme quand on utilise p, on saute une ligne pour créer un nouveau paragraphe .

-Les balises de titres vont de `**<h1> </h1>**` jusqu'à `**<h6> </h6>**`, ce qui permet de hiérarchiser et structurer le texte dans différentes sections, du niveau le plus grand, au niveau le plus petit:
<!DOCTYPE html>
```
<html lang="fr">
    <head>
        <meta charset="UTF-8">
        <title>Ma page</title>
    </head>
    <body>
        <h1>Bienvenue sur ma page</h1>
        <p>Ceci est le contenu de mon premier paragraphe</p>
        <p>Ceci est le contenu de mon deuxième paragraphe</p>
        <h2>Voilà mon sous-titre 1</h2>
        <h3>Une sous-partie</h3>
        <p>Un paragraphe</p>
        <h3>Une autre sous-partie</h3>
        <p>Tiens encore un paragraphe</p>
        <h2>Voilà mon sous-titre 2</h2>
        …
    </body>
</html>
```


-Pour baliser les éléments qu'on veut mettre dans une liste, on utilise **`<li> </li>`**  (pour "list item" ou "élément de la liste" en français). Puis on les insère tous à l'intérieur d'une autre balise pour indiquer s'il s'agit d'une liste à puces ou d'une liste numérotée.
-Les balises **`<ul> </ul>`**(pour "unordered list") permettent d'indiquer qu'on démarre une liste non ordonnée, c'est-à-dire, ce que l'on appelle en français **une liste à puces**.
Les balises `**<ol> </ol>**`(pour "ordered list") permettent d'indiquer qu'on démarre une liste ordonnée, autrement dit en français **une liste numérotée**.
```
<h1>Les fruits rouges</h1>
```
```
<ul>
   <li>Fraises</li>
   <li>Framboises</li>
   <li>Groseilles</li>
</ul>
```

```
<h1>Ma journée</h1>
```
```
<ol>
   <li>Je me lève.</li>
   <li>Je mange et je bois de l'eau.</li>
   <li>Je retourne me coucher.</li>
</ol>
```

| **Balises**            | **Traduction par le navigateur** |
| ---------------------- | -------------------------------- |
| <mark           /mark> | surligner                        |
| stong                  | gras                             |
| em                     | italique                         |



```
<p>Bonjour !<br>Ceci est mon deuxième test pour mettre des mots en avant, alors <strong>soyez indulgent</strong> s'il vous plaît, j'apprends petit à petit comment ça marche.</p>
```
```
<p>Bonjour !<br>Ceci est mon troisième test pour mettre des mots en avant, alors <mark>soyez indulgent</mark> s'il vous plaît, j'apprends petit à petit comment ça marche.</p>
```
```

```
LIEN HYPERTEXTE
On reconnaît facilement un **lien hypertexte** (ou **hyperlien**) sur une page web : par défaut, il est en bleu et souligné dans le navigateur et un curseur en forme de main apparaît lorsqu'on pointe dessus ; mais on peut modifier ce style en CSS.
Pour faire un lien hypertexte :

1. on utilise la balise`**<a>**`(pour "anchor") pour indiquer qu'on va rediriger vers un autre endroit,
    
2. puis, on ajoute l'attribut **`href`** suivi de**`=`**pour annoncer l'endroit vers lequel on veut rediriger,
    
3. on indique explicitement entre  **`" "`**  l'endroit vers lequel le lien doit rediriger,
    
4. enfin, on écrit le texte qui doit s'afficher sur l'hyperlien.
    

À partir de là, il y a des subtilités selon l'endroit où l'on veut rediriger l'utilisateur.

-Si vous voulez faire ==un lien vers un autre site existant en ligne==, rien de plus simple, il suffit d'utiliser la méthode de copier l'URL du site entre **`" "`**à la suite de l'attribut, comme ceci :

```
<a href="https://openclassrooms.com/fr/">Accédez à OpenClassrooms</a>
```

Ce type de lien hypertexte s'appelle un **lien absolu** : il indique une adresse complète.

-créez un lien hypertexte ==d'une page à une autre sur votre site==

Souvenez-vous : pour l’instant nous n’avons pas d’URL disponible car le site n’est pas encore en ligne. On va donc créer des liens entre nos pages en *utilisant leur nom*, et en indiquant leur arborescence dans notre dossier en local.

Ce type de lien hypertexte s'appelle un **lien relatif** : il indique où trouver notre fichier HTML.

cas n°1 : les deux pages sont situées dans un même dossier en local
Si les pages sont dans le même dossier, il suffit d'écrire comme cible du lien hypertexte le nom du fichier vers lequel on veut amener, par exemple le fichier nommé page2.html.

Si on veut aller de la page 1 à la page 2, voici ce que nous écrirons dans le fichier de page1.html  :

```
<a href="page2.html">Page 2</a>
```

-cas n°2 : les deux pages sont situées dans deux dossiers différents en local

Si on veut créer un fichier page 3 et le déplacer dans un autre dossier, par exemple un dossier  `/contenu` , on va donc indiquer le chemin à suivre pour trouver ce fichier :

```
<a href="contenu/page3.html">Page 3</a>
```

Et s'il y a plusieurs sous-dossiers, on écrira ceci :

```
<a href="contenu/autredossier/page3.html">Page 3</a>
```

Et si le fichier ne se trouve pas dans un sous-dossier, mais dans un dossier “parent”, on fait comment ?

Si votre fichier cible est placé dans un dossier qui se trouve “plus haut” dans l'arborescence, il faut écrire deux points  `..`  , comme ceci :

```
<a href="../page3.html">Page 3</a>
```

### créez une ancre avec les attributs  `id`  et  `href`

Une ancre est un repère que l'on peut mettre dans une page HTML si elle est très longue, cela aide à la navigation et rend un contenu plus facile à parcourir. Cela permet par exemple aux visiteurs d'un site web d'aller directement à la partie qui les intéresse.

Ce comportement est typique d'un site web "one page" où tout se situe sur la même page. 

Pour créer une ancre, il suffit de rajouter l'attribut  `id`  à une balise qui va alors servir de repère. Ce peut être n'importe quelle balise, une balise de titre par exemple. Voyons comment faire :

La première étape consiste à ajouter l'attribut  `id` suivi de `=`  pour donner un nom à l'ancre entre  `" "` :

```
<h2 id="mon_ancre">Titre</h2>
```

L'attribut  `id`  sert à donner un nom “unique” à une balise, pour s'en servir de repère. Et, croyez-moi, vous n'avez pas fini d'entendre parler de cet attribut. Ici, on s'en sert pour faire un lien vers une ancre mais, en CSS, il pourra nous être utile pour repérer une balise précise, vous verrez.

Évitez de créer des `id`  avec des espaces ou des caractères spéciaux ; utilisez simplement, dans la mesure du possible, des lettres et des chiffres pour que la valeur soit reconnue par tous les navigateurs.

La seconde étape consiste à indiquer où se situe l'ancre. La méthode pour se faire varie selon que :

1. l'ancre est plus bas sur la même page
    
2. l'ancre est située sur une autre page
    

#### **Cas n°1 : l'ancre est plus bas sur la même page**

Dans ce premier cas, on crée un lien avec l'attribut `href`  (il contient un dièse `#`  suivi du nom de l'ancre) :

```
<a href="#mon_ancre">Aller vers l'ancre</a>
```

Voici un exemple de page comportant beaucoup de texte et utilisant les ancres :

```
<h1>Ma grande page</h1>
<p>
Découvrez nos conseils d’aménagement pour :<br>
    <a href="#cuisine">La cuisine</a><br>
    <a href="#jardin">Le jardin</a><br>
    <a href="#salon">Le salon</a><br>
</p>
<h2 id="cuisine">La cuisine</h2>
<p>... (beaucoup de texte) ...</p>
<h2 id="jardin">Le jardin</h2>
<p>... (beaucoup de texte) ...</p>
<h2 id="salon">Le salon</h2>
<p>... (beaucoup de texte) ...</p>
```

**Testez pour voir avec le [CodePen P1C5](https://codepen.io/nicolaspatschkowski/pen/YzLQrJB?editors=1001)**

Vous avez peut-être remarqué que l’on a commencé à utiliser du latin pour remplir des zones de texte dans notre code. C'est normal, pas de panique ! Il s'agit du "[lorem ipsum](https://fr.wikipedia.org/wiki/Lorem_ipsum)", un “faux texte” qu'on peut ajouter provisoirement, de manière à calibrer une mise en page avant la validation d’un texte définitif.

#### **Cas n°2 : l'ancre est située dans une autre page**

Dans ce cas-là, on tape le nom de la page cible avant le dièse `#` et enfin le nom de l'ancre :

```
<a href="index.html#jardin">Le jardin</a>
```

Voici une nouvelle page qui contient trois liens, chacun amenant vers une des ancres de la page de l'exemple précédent :

```
<h1>Le Mégamix</h1>
<p>
Rendez-vous quelque part sur la page :<br>
    <a href="index.html#cuisine">La cuisine</a><br>
    <a href="index.html#jardin">Le jardin</a><br>
    <a href="index.html#salon">Le salon</a><br>
</p>
```

Et voilà pour tout ce que vous devez savoir sur les liens !

Sachez qu'il est possible de configurer un lien pour qu'il ait un comportement un peu particulier.

- `target="_blank"`  fait en sorte que le lien hypertexte ouvre un nouvel onglet :
    

```
<p>Bonjour. Souhaitez-vous apprendre sur <a href="https://openclassrooms.com" target="_blank">OpenClassrooms</a> ?</p>
```

- `href="[mailto:NOMDUMAIL@MAIL.COM](mailto:NOMDUMAIL@MAIL.COM)"`  crée un lien hypertexte qui ouvre la boîte mail avec un nouveau message vide.
    
- `href="NOMDEFICHIER.EXTENSION"`  crée un lien hypertexte qui permet de télécharger un fichier que vous avez placé au préalable dans le même dossier que votre page web.


| Objectif                             | Code                             |
| ------------------------------------ | -------------------------------- |
| Lien vers un site                    | `` `href="https://..."` ``       |
| Lien vers une page du site           | `` `href="page.html"` ``         |
| Lien vers un sous-dossier            | `` `href="dossier/page.html"` `` |
| Remonter d’un dossier                | `` `href="../page.html"` ``      |
| Lien vers une ancre                  | `` `href="#nom"` ``              |
| Lien vers une ancre d’une autre page | `` `href="page.html#nom"` ``     |
| Ouvrir dans un nouvel onglet         | `` `target="_blank"` ``          |
| Ouvrir un mail                       | `` `href="mailto:..."` ``        |