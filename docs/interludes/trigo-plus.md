
---
layout: default
title: Méthodes
parent: Interlude - Trigonométrie
nav_order: 1
---

# Préparer la première : trigonométrie

<details markdown="block">
  <summary>
    Contenu
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Introdution

### Historiquement : pourquoi 360 degrés ?

Le degré, qui peut être divisé en minutes et secondes lorsqu'on étudie la rotation de la Terre (360 jours, 360 degrés), vient des Babyloniens et des Chinois qui comptaient en base 60.
Il est probable que les $360°$ proviennent du triangle équilatéral des Sumériens ; comme ils comptaient en base $60$, trois angles font $3\times 60 = 180°$, ce qui correspond à l'angle plat.
En plus de cette utilité astronomique, $360$ est un nombre *pratique* pour le calcul fractionnaire, puisqu'il est divisible par $2$, $3$, et $5$ (les plus petits nombres premiers), et tous leurs multiples.

### Introduction aux radians

Autant les degrés sont la méthode historique de calcul, autant c'est les radians qui ont pris le dessus au cours du $XVIII^{ième}$ siècle pour les raisons suivantes :

- Facilité de calcul des sin / cos / tan
- Lien avec la circonférence du cercle
- Lien avec les nombres complexes
- L'absence d'unité, qui lui permet de se devenir facteur à l'intérieur de fonctions



## Bases de trigonométrie

### Définition.

{: .cours}
Soient deux droites concourantes distinctes formant un secteur angulaire. Soit un cercle dont le centre est le point d'intersection des droites et de rayon $r$ quelconque.
Alors la valeur de l'angle en radians est le rapport entre la longueur $L$ de l'arc de cercle intercepté par les droites et le rayon $r$.


![](https://minio.apps.education.fr/codimd-prod/uploads/upload_1a5f4c9c140542cb463d6f7da78bfa39.png =450x)

Comme $L$ est une fraction du périmètre total du cercle $2\pi r$, une chose fantastique se passe : quelque soit le rayon du cercle choisi, le rapport $\dfrac{L}{r}$ est toujours le même.

{: .exemple }
> - Prenons un angle de $90$ degrés et un cercle de rayon 10. La longueur de l'arc de cercle intercepté est **un quart** du périmètre total : $L=\dfrac{2\pi \times 10}{4}=5\pi$.
    La valeur de cet angle en radians sera donc $\dfrac{L}{r} = \dfrac{5\pi}{10}  = \boxed{\dfrac{\pi}{2}}$
>
> - Prenons un angle de $90$ degrés, et un cercle de rayon $1$. La longueur de l'arc de cercle intercepté est **toujours un quart** du périmètre total : $L=\dfrac{2\pi \times 1 }{4}=\dfrac{\pi}{2}$.
    La valeur de cet angle en radians sera donc $\dfrac{L}{r} = \dfrac{\dfrac{\pi}{2}}{1}  = \boxed{\dfrac{\pi}{2}}$

**Remarque.** Le rayon, apparaissant au numérateur *et* au dénominateur, s'annule lors du calcul de l'angle ; il n'a donc pas d'importance.

### Le cercle trigonométrique

Par défaut, on utilise : 
- Un cercle de rayon $1$ : comme on divise par le rayon, cela revient à diviser par $1$.
- La première droite est horizontale, et toujours "vers la droite".
- Les angles sont donnés **dans le sens contraire des aiguilles d'une montre**, qu'on appelle le sens **trigonométrique**. Un angle négatif correspond à un angle pour lequel on a tourné dans le sens horaire.

Ces conditions créent ce qu'on appelle le **cercle trigonométrique**, de centre $O(0;0)$ et de rayon $1$ : 

![](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.mathforu.com%2Fassets%2Fimg%2Fimage-20171115145055.png&f=1&nofb=1&ipt=0c331e250df9c9b9d598ba3ddc7a8bd7c17ec988e9a508f19099e9c02cc792bf&ipo=images =300x)

### Les angles importants

- $360°$ est $2\pi$ : le périmètre d'un cercle de rayon $1$.
-  $180°$ est $\pi$ : le demi-périmètre d'un cercle de rayon $1$ 
- $90°$ est $\dfrac{\pi}{2}$ : le quart de périmètre d'un...
- $45°$ est $\dfrac{\pi}{4}$ : la moitié du quart de périmètre d'un...

| ![](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fmathbooks.unl.edu%2FPreCalculus%2Fimages%2FimagesChap13%2FcommonDegrees.png&f=1&nofb=1&ipt=bbbf3dce9d666583ce6e5ef13faddb4df94bab8ef69c7ff7326456e48a527eeb&ipo=images =260x) | ![](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.coolmath.com%2Fsites%2Fdefault%2Ffiles%2Fimages%2F28-trigonometry-01.gif&f=1&nofb=1&ipt=8e57a9bbdb6db8bd67f8e155aecb87e53f22c72082784a60108b4ed58783980b&ipo=images =250x) |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

### Points, nombres, et angles


- A chaque point du cercle trigonométrique, on associe un angle.
- A chaque angle, on associe un point du cercle trigonométrique.

{: .remarque }
De plus, à tout nombre réel, on peut associer un point du cercle trigonométrique. Voir [ici](https://www.geogebra.org/m/FzHa7ACR) pour un "dessin".


Par exemple, les nombres $3$, $3 +2\pi$, $3-2\pi$, et $3 + 4\pi$ correspondent tous au même angle ; $2\pi$ correspond à un tour de cercle, ce qui fait revenir sur le même point / même angle.

Les points du cercle / angles ont un réel "principal" qui leur est associé : la longueur de l'arc de cercle, c'est à dire un réel compris entre $0$ et $2\pi$. On appelera ce réel la **mesure principale**.

{: .methode }
> Deux réels ont-il la même image sur le cercle ?
>
> *Si la différence entre les deux réels est un multiple de $2\pi$, alors ils auront la même image sur le cercle.*


- Considérons $\dfrac{\pi}{4}$ et $\dfrac{17\pi}{4}$ deux réels.
Calculons la différence : $\dfrac{17\pi}{4}-\dfrac{\pi}{4} = \dfrac{17\pi-\pi}{4}=\dfrac{16\pi}{4}=4\pi = 2\times 2\pi$
Les nombres ont la même image sur le cercle.

- Considérons $\dfrac{\pi}{6}$ et $\dfrac{31\pi}{6}$ deux réels.
Calculons leur différence : $\dfrac{31\pi}{6}-\dfrac{\pi}{6}=\dfrac{30\pi}{6}=5\pi = 4\pi +\pi$
Ces nombres n'ont pas la même image sur le cercle, *mais* on note que leur différence revient à $\pi$, ce qui correspond à un demi-tour de cercle : ils sont opposés.

{: .methode }
Déterminer l'image d'un réel sur le cercle / la mesure principale d'un réel.

Soit $\dfrac{38\pi}{3}$ un réel. On doit déterminer le réel appartenant à $[0; 2\pi[$ ayant la même image que $\dfrac{38\pi}{3}$. Pour cela, on peut écrire : $\dfrac{38\pi}{3} = \dfrac{6\pi}{3}\times 6 + \dfrac{2\pi}{3} =  2\pi \times 6 + \dfrac{2\pi}{3}$

Donc l'image de $\dfrac{38\pi}{3}$ est situé au même endroit que $\dfrac{2\pi}{3}$ (il faut bien sur connaitre les angles importants pour les placer correctement).

**Détail :** 
- On travaille en tiers, donc on passe $2\pi$ en tiers : $\dfrac{6\pi}{3}$
- On fait la division euclidienne de $38$ par $6$ (qui donne : $38 =6\times 6 + 2$)
- On "supprime" le multiple de $2\pi$ ainsi trouvé.


### Lien avec sinus et cosinus

Prenons un angle sur notre cercle trigonométrique. Qu'est-ce que son **cosinus** ?

Par la définition que l'on connait ($\dfrac{\text{adjacent}}{\text{hypothénuse}}$), il nous faut d'abord un triangle **rectangle**. Qu'à cela ne tienne, dessinons-en un.

![](https://minio.apps.education.fr/codimd-prod/uploads/upload_b0aca982f862a03ec1be96987ffb7d8b.png =400x)

Par nos formules, $\cos(\alpha)=\dfrac{OB}{OA}$. Or, $OA$ est le rayon du cercle trigonométrique, qui est égal à $1$.
Donc $\cos(\alpha)=OB$, c'est-à-dire **l'abscisse du point $A$**.

De même, $\sin(\alpha)=AB$, c'est-à-dire **l'ordonnée du point $A$**.

{: .attention }
On a donc : $(\cos(\alpha),\sin(\alpha)) =(x_A;y_A)$ pour $\alpha$ =$\widehat{IOA}$.


De même que pour les degrés, on a les propositions suivantes : 

{: .cours }
> - $\cos(\alpha)^2+\sin(\alpha)^2=1$
>
> - $-1 \leq \cos(\alpha) \leq 1$
>
> - $-1 \leq \sin(\alpha) \leq 1$


*Note* : les sinus et cosinus peuvent maintenant être négatifs, de même que les angles, puisqu'il y a bien des points sur le cercle trigonométrique ayant des coordonnées négatives.

![](https://www.annales2maths.com/wp-content/uploads/2020/04/1%C3%A8re-cours-trigonom%C3%A9trie-cercle-trigonom%C3%A9trique-et-valeurs-particuli%C3%A8res-cos-sin.png =500x)

## Exercices

[Voir le pdf ici ](https://drive.google.com/file/d/1Mr6c5O_BtyLqynL8O70I2jW31UchCr4O/view?usp=share_link)


<style>h3,h4{opacity:.9!important}#doc li,p{font-size:.85em}#doc ul li,h4{margin-left:1em!important}#doc span,ins{font-weight:400!important}#doc em a,ins{text-align:justify}#doc li p,#doc ol ol{margin-left:0!important}#doc ol ol ul,#doc ol ul{margin-top:.25em!important}ins,mark{padding-left:10px}#doc em a,mark{margin-bottom:1em;display:inline-block}body:not(.night){background-color:#272725}body:not(.night) #doc{background-color:#fff}h1:first-of-type{font-size:3em;padding-top:.25em;margin-bottom:1em;border-bottom:none!important;color:}h1{color:#005738;text-align:center;margin-top:2em!important;border-bottom:1px solid #005738!important;margin-bottom:1em!important}h2{color:#008d44;padding-top:1em;border-bottom:1px solid #008d44!important;margin-bottom:.75em!important}h3{color:#a31e00;padding-top:.5em;padding-bottom:.25em;border-bottom:1px dashed #a31e00!important}h4{color:#691024;padding-top:.2em;border-bottom:1px dotted #691024!important}#doc h4 span{opacity:1!important}#doc{padding:2em 4em!important;border-radius:15px!important;margin-bottom:3em!important;max-width:1050px}#doc span{!important;opacity:1!important}#doc h3 span{opacity:.8!important;font-size:.73em!important;display:block!important;margin-left:.5em!important;margin-top:3px!important}body:not(.night) #doc h3 span{color:#a31e00!important}#doc p,#doc ul{font-family:-apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Helvetica,Arial,sans-serif}body:not(.night) #ui-toc-affix{background-color:transparent;margin-left:1em}body:not(.night) .toc .nav>li>a{color:#c90076!important}body:not(.night) .ui-toc-dropdown .nav>li.active>a{color:#aa7!important;border-left:1px solid #000!important}body:not(.night) .ui-toc-dropdown .nav>li>a:hover{border-left:1px solid #000!important}body.night .ui-toc-label{background-color:#444;border:none}h5,h6,p{margin:0 0 0 1em!important;padding:.25em!important}h5{padding-top:.5em!important;margin-top:.5em!important;margin-left:2em!important}#doc ol,#doc ul,h6{margin-left:3em!important}#doc li p{font-size:1em!important}#doc em a,ins span{font-size:.8em}p{margin-left:5em!important}body:not(.night) h5,body:not(.night) h6{color:#000!important}#doc ol{margin-bottom:.05em!important;margin-top:.05em!important;font-style:italic}#doc li{line-height:1em}ins{font-size:.6em;text-decoration:none;font-style:normal!important;border-left:1px solid #ccc}#doc em a{background-color:#eee;border-radius:10px;padding:6px 12px!important}@media screen and (min-width:600px){ins{float:right;display:block;width:170px}ins:hover{color:#600!important;border-left:1px solid #600!important}#doc{font-size:1.4em}}@media screen and (min-width:1000px){ins{margin-left:4em!important}}@media screen and (max-width:600px){#doc{padding:10px!important}#doc ol,#doc p,#doc ul{margin-left:3em!important}#doc ul li{margin-left:-1em!important}}#doc ol ol{list-style-type:lower-alpha;margin-top:.35em!important}#doc ol ul{margin-left:.25em!important;font-style:normal}#doc ol ol ul{margin-left:-1.5em!important;font-size:initial}#doc ul ul{margin-left:-.5em!important}mark{color:#000f4d;font-size:.85em;border-left:1px dotted #002366;background:0 0;margin-top:.5em}
</style>
