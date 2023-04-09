---
layout: default
title: Extra 1
parent: Interlude - Trigonométrie
nav_order: 1
---

Ici se trouvent trois théorèmes à démontrer. Les démonstrations sont guidées, et sont rédigées à la fin de la page.


# La loi des sinus

{: .cours }
> Dans un triangle, soient $a$, $b$, et $c$ les côtés opposés aux points, et $\alpha$, $\beta$, $\gamma$ leurs angles.
>
> Alors : $\dfrac{a}{\sin \alpha} = \dfrac{b}{\sin \beta} = \dfrac{c}{\sin \gamma}$

**Première démonstration : en utilisant les hauteurs.**

1. Tracer la hauteur $h$ issue de $C$.
2. Exprimer $\sin \alpha$ et $\sin \beta$ en fontion de $h$.
3. En déduire deux expressions de $h$ (en fonction de $b$ et $\alpha$, puis de $a$ et $\beta$).
4. En déduire que $\dfrac{a}{\sin \alpha}=\dfrac{b}{\sin\beta}$

5. Tracer la hauteur $h'$ issue de $A$ et répéter la démonstration pour obtenir $\dfrac{b}{\sin\beta}=\dfrac{c}{\sin \gamma}$

**Deuxième démonstration : en calculant l'aire du triangle.**

1. Tracer la hauteur $h$ issue de $C$.
2. En déduire une expression de l'aire $S$ de $ABC$.
3. Comme $h=b\sin\alpha$, en déduire que $\dfrac{a}{\sin \alpha} =\dfrac{abc}{2S}$.
4. Par symétrie des notations, la formule est vérifiée.

{: .cours }
> **Corrolaire**
> L'aire d'un triangle $ABC$ est égale à $\dfrac{1}{2}ab\sin\gamma$

Cette formule découle simplement du fait que la hauteur issue de $A$ est égale à $b\sin\gamma$. Elle est pratique lorsqu'il s'agit dee
calculer l'aide d'un triangle dont on ne connaît pas la hauteur.

# La formule d'Al-Kashi

L'objet de cette partie est de démontrer la formule d'Al-Kashi (aussi appelée *loi des cosinus*), une généralisation du théorème de Pythagore.

{: .cours }
Dans un triangle $ABC$, on a la relation : $c^2 = a^2 + b^2 - 2ab\cos\gamma$


Il y a plusieurs démonstrations ; celle proposée ici reprend le théorème de Pythagore.

**Démonstration.**

1. Tracer la hauteur issue de $B$. On note son pied (intersection de la hauteur et de la base) $H$.
2. - Montrer que $BH=a\sin\gamma$
   - Montrer que $AH=b-a\cos\gamma$
   - Montrer que $CH=a\cos\gamma$
3. En utilisant l'égalité de Pythagore, en déduire que $c^2 = b^2 - 2ab\cos\gamma + a^2(\cos^2\gamma + \sin^2\gamma)$
4. En déduire que $c^2=b^2 + a^2 - 2ab\cos\gamma$

# 
