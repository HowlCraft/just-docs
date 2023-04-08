---
layout: default
title: 10. Colinéarité
nav_order: 2
---

# Customization
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

# Methodes : la colinéarité 

## Calculer le déterminant de deux vecteurs.
::: success
**Formule** : $det(\vec{u},\vec{v}) = 2\times 3 - 4\times (-5) = 6+20=26$, pour $\vec{u}\begin{pmatrix}x \\ y \end{pmatrix}$ et $\vec{v}\begin{pmatrix}x' \\ y' \end{pmatrix}$
:::

:::info
Exemple : Si $\vec{u}\begin{pmatrix}2 \\ -5 \end{pmatrix}$ et $\vec{v}\begin{pmatrix}4 \\ 3 \end{pmatrix}$, alors $det(\vec{u},\vec{v}) = 2\times 3 - 4\times (-5) = 6+20=26$

:::

**Exercice.**
Calculer les déterminant des vecteurs $\vec{u}$ et $\vec{v}$ dans les cas suivants : 
- $\vec{u}\begin{pmatrix}3 \\ -6 \end{pmatrix}$ et $\vec{v}\begin{pmatrix}1 \\ 2 \end{pmatrix}$
- $\vec{u}\begin{pmatrix}-1 \\ 2 \end{pmatrix}$ et $\vec{v}\begin{pmatrix}-3 \\ -1 \end{pmatrix}$
- $\vec{u}\begin{pmatrix}0,5 \\ 4 \end{pmatrix}$ et $\vec{v}\begin{pmatrix}-1 \\ -8 \end{pmatrix}$

<details>
  <summary markdown="span">Solutions (clique ici)</summary>

- Cas 1 : $det(\vec{u},\vec{v}) = 3\times 2 - 1\times (-6) = 12$
- Cas 2 : $det(\vec{u},\vec{v}) = (-1)\times (-1) - (-3)\times 2 = 7$
- Cas 3 : $det(\vec{u},\vec{v}) = 0,5\times (-8) - (-1)\times 4 = 0$
</details>


:::info
Rappel : si $A(x_A;y_A)$ et $B(x_B;y_B)$, alors $\vec{AB}\begin{pmatrix}x_B-x_A \\ y_B-y_A \end{pmatrix}$
"point d'arrivé moins point de départ"
:::

**Exercice.**
Soient $A(7;-2)$, $B(1;2)$, $C(6;3)$, et $D(5;0)$ des points. Calculer le déterminant de $\vec{AB}$ et $\vec{CD}$.

<details>
  <summary markdown="span">Solutions (clique ici)</summary>
    
**Etape 1.** 
    On calcule les coordonnées des vecteurs : 
- $\vec{AB}\begin{pmatrix}1-7 \\ 2-(-2) \end{pmatrix}$ donc $\vec{AB}\begin{pmatrix}-6 \\ 4 \end{pmatrix}$
- $\vec{CD}\begin{pmatrix}5-6 \\ 0-3 \end{pmatrix}$ donc $\vec{CD}\begin{pmatrix}-1 \\ -3 \end{pmatrix}$
    
**Etape 2.** On calcule le déterminant : 
    $det(\vec{AB};\vec{CD})=(-6)\times(-3) - (-1)\times 4 =  18+4=\boxed{22}$
</details>

:::danger
**Rappel** Deux vecteurs non nuls sont **colinéaires** si et seulement si leur déterminant est nul (égal à $0$)
:::

## Vérifier si deux vecteurs sont colinéaires.

:::success
**Méthode** On calcule le déterminant. S'il est égal à $0$, les vecteurs sont colinéaires. Sinon, les vecteurs ne sont pas colinéaires.
:::

**Exercice**
Les vecteurs $\vec{u}\begin{pmatrix}-6 \\ 4 \end{pmatrix}$ et $\vec{v}\begin{pmatrix}3 \\ -2 \end{pmatrix}$ sont-ils colinéaires ? Justifier.

<details>
  <summary markdown="span">Solutions (clique ici)</summary>
    
**Etape 1.** On calcule le déterminant.
$det(\vec{u};\vec{v})=(-6)\times (-2) - 4\times 3 = 12 - 12 = 0$
**Etape 2.** Conclure.
Le déterminant est nul, donc les vecteurs $\vec{u}$ et $\vec{v}$ sont colinéaires.
</details>


## Vérifier si deux droites sont parallèles.


:::success
**Méthode.** On veut savoir si les droites $(GH)$ et $(DE)$ sont parallèles.
1) On calculer les coordonnées des vecteurs $\vec{GH}$ et $\vec{DE}$.
2) On calcule le déterminant de $\vec{GH}$ et $\vec{DE}$.
3) Si le déterminant est égal à $0$, les **vecteurs** sont colinéaires, et onc les **droites** sont parallèles. Sinon, les vecteurs ne sont pas colinéaires et les droites ne sont pas parallèles.
:::

**Exercice.**
![](https://minio.apps.education.fr/codimd-prod/uploads/upload_1f703898d38b79638de0c0405eba46a0.png =500x)


<details>
  <summary markdown="span">Solutions (clique ici)</summary>
    
**Question 1.** 
Calculons les coordonnées des vecteurs $\vec{AB}$ et $\vec{CD}$ : 
- $\vec{AB}\begin{pmatrix}1-(-3) \\ 3-2 \end{pmatrix}$ donc $\vec{AB}\begin{pmatrix}4 \\ 1 \end{pmatrix}$
- $\vec{CD}\begin{pmatrix}0,5-(-2) \\ 4-0 \end{pmatrix}$ donc $\vec{CD}\begin{pmatrix}2,5 \\ 4 \end{pmatrix}$
Calculons le déterminant : $det(\vec{AB},\vec{CD})=4\times 4 - 2,5\times 1=13,5\neq 0$.
Donc les vecteurs $\vec{AB}$ et $\vec{CD}$ ne sont pas colinéaires, et les droites $(AB)$ et $(CD)$ ne sont pas parallèles.

**Question 2.**
Calculons les coordonnées des vecteurs $\vec{AC}$ et $\vec{BD}$ : 
- $\vec{AB}\begin{pmatrix}-2-(-3) \\ 0-2 \end{pmatrix}$ donc $\vec{AB}\begin{pmatrix}1 \\ -2 \end{pmatrix}$
- $\vec{CD}\begin{pmatrix}0,5-1 \\ 4-3 \end{pmatrix}$ donc $\vec{CD}\begin{pmatrix}-0,5 \\ 1 \end{pmatrix}$
Calculons le déterminant : $det(\vec{AC},\vec{BD})=1\times 1 - (-0,5)\times (-2)=1-1= 0$.
Donc les vecteurs $\vec{AB}$ et $\vec{CD}$ sont colinéaires, et les droites $(AB)$ et $(CD)$ sont parallèles.
</details>

## Vérifier si trois points sont alignés.

:::success
Soient trois points $M$, $N$, et $P$.
Pour savoir s'ils sont alignés, on construit deux vecteurs à partir de ces points (*n'importe lesquels*), et on calcule le déterminant de ces vecteurs.
Si le déterminant est nul, les points sont alignés. Sinon, les points ne sont pas alignés.
:::

:::info
**Exemple**
Soient $A(3;1)$, $B(4; 5)$ et $C(7; 17)$.
On choisit les vecteurs $\vec{AB}$ et $\vec{AC}$.

$\vec{AB}\begin{pmatrix}1\\ 4 \end{pmatrix}$ et $\vec{AC}\begin{pmatrix}4 \\ 16 \end{pmatrix}$

Donc $det(\vec{AB},\vec{AC})=1\times 16 - 4\times 4 =0$.
Les vecteurs sont colinéaires, donc les points sont alignés.
:::

**Exercice.**
Dans chacun des cas, dire si les points sont alignés ou non :
- $E(4;-1)$, $F(6; -2)$, $G(-2; 2)$
- $M(0;5)$, $N(2;4)$, $P(1;6)$
- $A(-4;-7)$, $B(0;-7,5)$, $C(-12 ; -6)$


<details>
  <summary markdown="span">Solutions (clique ici)</summary>
    
- Oui
- Non
- Oui
</details>



## Trouver les coordonnés d'un point (sachant que les vecteurs sont colinéaires)

:::success
**Méthode** Calculer le déterminant avec les inconnues ($x$ ou $y$ en général).
Cela donne une équation $=0$, car le déterminant doit être nul.
Résoudre l'équation.
:::

:::info
**Exemple.**
Soient $\vec{u}\begin{pmatrix}x \\ 3 \end{pmatrix}$ et $\vec{v}\begin{pmatrix}5 \\ -2 \end{pmatrix}$
-deux vecteurs colinéaires. Déterminer $x$.

On calcule le déterminant : $det(\vec{u};\vec{v})=x\times (-2) -3\times 5 = -2x - 15$
Or, les vecteurs sont colinéaires, sont le déterminant est nul.

On a donc : $-2x-15=0 \Longrightarrow -2x-12\color{red}{+15}=0\color{red} {+15} \Longrightarrow -2x = 15$

$\Longrightarrow \dfrac{-2x}{\color{red}{-2}} = \dfrac{15}{\color{red}{-2}} \Longrightarrow \boxed{x = \dfrac{15}{-2}}$
:::

**Exercice** Déterminer $x$ et $y$ tels que les vecteurs soient colinéaires
- $\vec{u}\begin{pmatrix}x \\ 15 \end{pmatrix}$ et $\vec{v}\begin{pmatrix}2 \\ 6 \end{pmatrix}$
- $\vec{u}\begin{pmatrix}4 \\ y \end{pmatrix}$ et $\vec{v}\begin{pmatrix}6 \\ 11 \end{pmatrix}$


<details>
  <summary markdown="span">Solutions (clique ici)</summary>
    
- $x=5$ (on résout l'équation $6x-30=0$)
- $y=\dfrac{22}{3}$ (on résout l'équation $44-6y=0$)
</details>

**Problème**
Soient $A(x;4)$, $B(7;3)$, $C(2;1)$ et $D(6;-2)$ quatre points. Déterminer $x$ tel que $(AB)$ et $(CD)$ soient parallèles.

<details>
  <summary markdown="span">Indice (clique ici)</summary>
    
Si les droites $(AB)$ et $(CD)$ sont parallèles, quels vecteurs doivent être colinéaires ? Calculer leurs coordonnées.
</details>

<details>
  <summary markdown="span">Solutions (clique ici)</summary>
 
**Etape 1.** Calculer les coordonnées de $\vec{AB}$ et $\vec{CD}$ : 
$\vec{AB}\begin{pmatrix}7-x\\-1\end{pmatrix}$ et $\vec{CD}\begin{pmatrix}4\\-3\end{pmatrix}$ 

**Etape 2.** Calculer le déterminant de ces vecteurs : 
$det(\vec{AB},\vec{CD})=(7-x)\times (-3) - 4\times (-1)= 7\times (-3) -x\times (-3) + 4 = -21 + 3x + 4 = 3x - 17$


*Note : on utilise la distributivité pour simplifier l'expression*
**Etape 3** Les vecteurs sont colinéaires, donc le determinant est nul : on a une équation à résoudre.
$3x-17=0 \Longleftrightarrow 3x=17 \Longleftrightarrow \boxed{x = \dfrac{17}{3}}$
</details>
