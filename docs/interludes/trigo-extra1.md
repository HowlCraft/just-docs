---
layout: default
title: Extra 1
parent: Interlude - Trigonométrie
nav_order: 1
---

Ici se trouvent deux théorèmes à démontrer. Les démonstrations sont guidées et sont rédigées en fin de la page.


# La loi des sinus

{: .cours }
> Dans un triangle $ABC$, notons $\alpha$, $\beta$, et $\gamma$ les angles des points $A$, $B$, et $C$, et $a$, $b$, $c$ leurs côtés opposés.
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
> **Corollaire**
> L'aire d'un triangle $ABC$ est égale à $\dfrac{1}{2}ab\sin\gamma$

Cette formule découle simplement du fait que la hauteur issue de $A$ est égale à $b\sin\gamma$. Elle est pratique lorsqu'il s'agit de calculer l'aide d'un triangle dont on ne connaît pas la hauteur.

# La formule d'Al-Kashi

L'objet de cette partie est de démontrer la formule d'Al-Kashi (aussi appelée *loi des cosinus*), une généralisation du théorème de Pythagore.

{: .cours }
Dans un triangle $ABC$, on a la relation : $c^2 = a^2 + b^2 - 2ab\cos\gamma$


Il y a plusieurs démonstrations ; celle proposée ici reprend le théorème de Pythagore.

**Démonstration.**

1. Tracer la hauteur issue de $B$. On note son pied (intersection de la hauteur et de la base) $H$.
2. - Montrer que $BH=a\sin\gamma$
   - Montrer que $AH=b-a\cos\gamma$
3. En utilisant l'égalité de Pythagore, en déduire que $c^2 = b^2 - 2ab\cos\gamma + a^2(\cos^2\gamma + \sin^2\gamma)$
4. En déduire que $c^2=b^2 + a^2 - 2ab\cos\gamma$

# Solutions.

## La loi des sinus -méthode des hauteurs

Soit $h$ la hauteur issue de $C$, et $H$ son pied.
- $CAH$ est un triangle rectangle en $H$. On a donc $\sin\alpha=\dfrac{h}{b}$, d'où $h=b\sin\alpha$
- $CBH$ est un triangle rectangle en $H$. On a donc $\sin\beta=\dfrac{h}{a}$, d'où $h=a\sin\beta$

On en déduit que $a\sin\beta=b\sin\alpha$, d'où $\boxed{\dfrac{a}{\sin \alpha}=\dfrac{b}{\sin\beta}}$

De même, soit $h'$ la hauteur issue de $A$, et $H'$ son pied.
- $ABH$ est un triangle rectangle en $H$, donc $\sin\beta=\dfrac{h'}{c}, d'où $h'=c\sin\beta$
- $ACH$ est un triangle rectangle en $H$, donc $\sin\gamma=\dfrac{h'}{b}$, d'où $h'=b\sin\gamma$

On en déduit que $c\sin\beta=b\sin\gamma$, d'où  $\boxed{\dfrac{b}{\sin \beta}=\dfrac{c}{\sin\gamma}}$

## La loi des sinus -méthode de l'aire

Soit $h$ la hauteur issue de $C$, et $H$ son pied. L'aire de $ABC$ est donc $S=\dfrac{ch}{2}$.
Or, $AHC$ étant un triangle rectangle, $\sin\alpha=\dfrac{h}{b}$, d'où $h=b\sin\alpha$.
Donc $S=\dfrac{bc\sin\alpha}{2} \Longleftrightarrow 1=\dfrac{bc\sin\alpha}{2S} \Longleftrightarrow \dfrac{1}{\sin\alpha} = \dfrac{bc}{2S} \Longleftrightarrow \dfrac{a}{\sin\alpha}=\dfrac{abc}{2S}$

De même, $\dfrac{c}{\sin\gamma}=\dfrac{abc}{2S}$ et $\dfrac{b}{\sin\beta}=\dfrac{abc}{2S}$

## Théorème d'Al-Kashi

Soit $h$ la hauteur issue de $B$, et $H$ son pied.
Alors : 
- $CBH$ est un triangle rectangle en $H$, donc $\sin\gamma=\dfrac{BH}{a}$, d'où $BH=a\sin\gamma$
- $CBH$ est un triangle rectangle en $H$, donc $\cos\gamma=\dfrac{CH}{a}, d'où $CH=a\cos\gamma$
  Or, $AH=AC-CH$, donc $AH=b-a\cos\gamma$
  
De plus, $ABH$ est un triangle rectangle en $H$, donc $c^2 = BH^2 + AH^2$
Donc $c^2=(a\sin\gamma)^2 + (b-a\cos\gamma)^2 = a^2\sin^2\gamma + b^2 - 2ab\cos\gamma +(a\cos\gamma)^2 = a^2\sin^2\gamma + b^2 - 2ab\cos\gamma +a^2\cos^2\gamma$

En factorisant par $a^2$, on obtient : $c^2 = b^2-2ab\cos\gamma + a^2(\sin^2\gamma + \cos^2\gamma)$
Or, $\cos^2\gamma+\sin^2\gamma=1$, donc $\boxed{c^2 = b^2+a^2-2ab\cos\gamma}$
