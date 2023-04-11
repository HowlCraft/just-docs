---
title: Extra - les nombres complexes
layout: home
---

# Extra : les complexes
<details markdown="block">
  <summary>
    Contenu
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Introduction historique.

Etudions l'équation $(x+3)(x-\dfrac{1}{2})=0$.
- Dans $\mathbb{N}$, cette équation n'a pas de solutions.
- Dans $\mathbb{Z}$, elle en a une : $-3$.
- Dans $\mathbb{Q}$, elle en a deux : $-3$ et $\dfrac{1}{2}$.

**Remarque.** Soit $P$ un polynôme de degré $n$. Alors $P$ a *au plus* $n$ racines (dans $\mathbb{r}$)

Etudions l'équation $x^2-2=0$. Dans $\mathbb{Q}$, elle n'a pas de solutions. Mais dans $\mathbb{R}$, elle en a deux $\sqrt{2}$ et $-\sqrt{2}$.

La création des nombres complexes vient de l'envie de "créer" des solutions pour les équations n'en ayant pas dans l'ensemble des nombres réels. Spécifiquement, ils on été introduits au $XVI^{ième}$ siècle par Cardan pour résoudre les équations du type : $x^3+px+q=0$, avec $p$ et $q$ réels. Sa méthode demande l'existence de **racines carrées de nombres négatifs** : comme ces nombres n'existent pas,Cardan les introduit en tant que *nombres imaginaires*, des nombres ayant **un carré négatif**.

En admettant l'existence d'un nombre imaginaire $i$ tel que $i^2=-1$, on est forcé d'introduire tous les "nombres" 
de la forme $a+bi$ (addition et multiplication), avec $a$ et $b$ réels.

Grâce aux complexes, toutes les équations du second degré ont maintenant des solutions dans $\mathbb{C}$, l'ensemble des nombres complexes : 

$x^2+2=0 \Longleftrightarrow x^2=-2 \Longleftrightarrow x=\sqrt{-2}=\sqrt{-1}\sqrt{2}=i\sqrt{2}$ ou $x=-\sqrt{-2}=-\sqrt{-1}\sqrt{2}=-i\sqrt{2}$

## Présentation.

{: .cours }
> Les nombres complexes, notés $z$, se présentent sous la forme algébrique $a+ib$, où $a$ et $b$ sont des réels et $i$ (l'unité imaginaire)
est un nombre tel que $\boxed{i^2=-1}$.
> 
> $a$ est dit *partie réelle* de $z$ et $b$ est dit *partie imaginaire* de $z$.

{: .cours }
**Condition d'égalité.** Soient $z=a+ib$ et $z'=a'+ib'$ deux nombres complexes. $z=z' \Longleftrightarrow \begin{cases} a=a' \\\\ b=b' \end{cases}$

## Opérations.

### Addition.

{: .cours}
Soient $z=a+bi$ et $z'=a'+b'i$ deux nombres complexes. Alors $z+z' = (a+a') + i(b+b')$

{: .exemple }
$2+3i + 5+9i = 7+12i$

**Note.** La soustraction fonctionne de la même façon.

**Note.** Tout nombre complexe $a+bi$ admet un opposé : $-a-ib$.

### Multiplication.

{: .cours}
Soient $z=a+bi$ et $z'=a'+b'i$ deux nombres complexes. Alors $zz' = (aa'-bb') + i(ab'+b'a)$

### Le conjugué.

{: .cours}
Le conjugué du nombre complexe $z=a+ib$ est $a-ib$. On le note $\overline{z}$.

**Exemple.** Le conjugé de $5+2i$ est $5-2i$. Le conjugué de $-4-7i$ est $-4+7i$.


Pour $z=a+ib$ et $z'=a'+ib'$ deux complexes, on a :

| $\overline{\overline{z}}=z$ | $z\overline{z} = a^2+b^2$ | $\overline{z^n}=\overline{z}^n$ | $\overline{z}+\overline{z'}=\overline{z+z'}$ | $\overline{z}\overline{z'}=\overline{zz'}$ | $\overline{\frac{z}{z'}}=\frac{\overline{z}}{\overline{z'}}$ |

| -------------  | -------------| -------------| -------------| -------------| -------------|

### Module et inverse.

{: .cours}
Soit $z=a+ib\in\mathbb{C}$. On définit le **module** de $z$ par $\|z\| =\sqrt{a^2+b^2}$.

**Note.** Soit $z=a+ib$ un nombre complexe. Calculons son inverse : 

$\dfrac{1}{z}=\dfrac{1}{a+ib}=\dfrac{1\times(a-ib)}{(a+ib)(a-ib)}=\dfrac{a-ib}{a^2-b^2}=\dfrac{\overline{z}}{\|z\|^2}$

## Exercices.

### Exercice 1.
Ecrire les nombres complexes suivants sous leur forme algébrique ($a+ib$) : 
- $3+2i - (3i-2)$
- $(3-2i)(2+3i)$
- $i^3$
- $(2+4i)^2$
- $(1+i)^3$

### Exercice 2.
Déterminer la partie réelle et la partie imaginaire de chacun des nombres complexes : 
- $3+2i$
- $-2i+4$
- $\dfrac{3+5i}{2}$
- $\dfrac{2i-1}{\sqrt{2}}$
- $4i$
- $0$
- $i^2$

### Exercice 3.**
Déterminer les conjugués des nombre suivants :
- $3+2i$
- $3i-4$
- $-5-6i$
- $i$

### Exercice 4.
Soit $a$ un réel et $z=a^2+1+2i(a^2-3)$ un nomre complexe.
1. Déterminer les éventuelles valeurs de $a$ tel que $z$ soit un réel.
2. Déterminer les éventuelles valeurs de $a$ tel que $z$ soit un imaginaire pur (sa partie réelle est nulle).

## Solutions.

### Exercice 1.
- $3+2i - (3i-2) = 5-i$
- $(3-2i)(2+3i)=6+9i-4i-6i^2=6+9i-4i+6=12-5i$
- $i^3=i\times i^2 = i\times (-1) = -i$
- $(2+4i)^2 = 4-2\times 2\times 4i +(4i)^2 = 4-16i - 16 = -12-16i$
- $(1+i)^3=(1+i)(1+2i-1) = (1+i)2i =2i+2i^2 = -2 + 2i$

### Exercice 2.
- $3+2i$ Partie réelle : 3$, partie imaginaire : $2$
- $-2i+4$ Partie réelle : $4$, partie imaginaire $-2$
- $\dfrac{3+5i}{2}$ Partie réelle $\dfrac{3}{2}$, partie imaginaire : $\dfrac{5}{2}$
- $z=\dfrac{2i-1}{\sqrt{2}}$ $\Re(z)$=\sqrt{2}$, $\Im(z)=-\dfrac{\sqrt{2}{2}$
- $4i$ $\Re(4i)=0$, $\Im(2i)=4$
- $0$ $\Re(0)=0$, $\Im(0)=0$
- $i^2 \Re(i^2)=-1$, $\Im(i^2)=0$, car $i^2=-1$
