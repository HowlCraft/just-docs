---
layout: default
title: Extra
parent: 10 - La Colinéarité
nav_order: 2
---

# Les homothéties

Le terme d'homoéthétie semble être dû au mathématicien français Michel **Chasles** (oui, le même que celui de la *relation de Chasles* !). Son préfixe, *homo-*, veut dire "semblable", et *thésis* signifie "position".
Il traduit la correspondance entre deux figures de même forme.

## Définition du collège

{: .cours }
> Une homothétie est une transformation géométrique permettant d'agrandir ou de rétrécir une figure en respectant toutes ses proportions. Elle est définie grâce à un centre et un rapport (le *coefficient* d'agrandissement ou de diminution).
> 
> L'image $M'$ du point $M$ du plan par une homothétie de centre $O$ et de rapport $k$ (non nul) est défini par :
> 
>   - OM' = k×OM ;
  >  - si $k > 0$, $M'\in[OM)$ ($M$ et $M'$ sont du même côté par rapport à $O$)
  >  - si $k < 0$, $M'\in[MO)$ ($M$ et $M'$ sont opposés par rapport à $O$)

## Définition vectorielle

{: .cours }
L'image du point $M$ par l'homothétie de centre $O$ et de rapport $k$ est le point $M'$ tel que $\overrightarrow{OM'}=k\overrightarrow{OM}$

{: .cours }
Toute homothétie transforme une droite en une droite qui lui est parallèle.

**Démonstration.**
Soit $M'$ l'image de $M$ et $N'$ l'image de $N$ par l'homoéthétie de centre $O$ det de rapport $k$.
Alors :
- $\overrightarrow{OM'}=k\overrightarrow{OM}$
- $\overrightarrow{ON'}=k\overrightarrow{ON}$

Donc $\overrightarrow{M'N'}=\overrightarrow{M'0}+\overrightarrow{ON'}$ (par la relation de Chasles)

Donc $\overrightarrow{M'N'}=\overrightarrow{ON'}-\overrightarrow{0M'}$ (en utilisant la relation $\overrightarrow{M'0}=-\overrightarrow{OM'}$)

Donc $\overrightarrow{M'N'}=k\overrightarrow{ON}-k\overrightarrow{0M}=k(\overrightarrow{ON}-\overrightarrow{OM})$

Donc $\overrightarrow{M'N'}=k(\overrightarrow{MO}+\overrightarrow{ON})=k\overrightarrow{MN}$

Les vecteurs sont colinéaires, donc les droites $(M'N')$ et $(MN)$ sont parallèles.

