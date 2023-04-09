---
title: Interlude - Trigonométrie
layout: home
---
# Interlude : la Trigonométrie

<details markdown="block">
  <summary>
    Contenu
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Cours

<img style="float: right;" src="https://minio.apps.education.fr/codimd-prod/uploads/upload_79b8f194f6951d58087546bf9c49eafa.png" width=400>

{: .cours }
> On se place dans un triangle **rectangle**. 
> 
> - $cos(\alpha)=\dfrac{\text{adjacent}}{\text{hypothénuse}}$
> 
> - $sin(\alpha)=\dfrac{\text{opposé}}{\text{hypothénuse}}$
> 
> - $tan(\alpha)=\dfrac{\text{opposé}}{\text{adjacent}}$


Note : le côté *opposé* est le côté *qui ne touche pas* l'angle $\alpha$. Le côté *adjacent* est celui qui *touche* l'angle $\alpha$.

## Exercices

EXERCICES ICI
INDICES ET SOLUTIONS [ICI](https://codimd.apps.education.fr/s/YNeMPvLJZ#) (incomplètes pour le moment)

## Méthodes.

### Déterminer la valeur d'un angle à partir du cos/sin/tan.
{: .cours }
> La calculatrice a les trois touches ```cos``` / ```sin``` / ```tan```. Elle a aussi les touches (en général ```2nde + cos```) ```arccos```, ```arcsin```, et ```arctan```.
Sur certaines calculatrices, ces touches peuvent s'appeler ```acos``` ou ```cos-1```.
> - La touche ```cos``` permet de passer de l'angle au cosinus
> - La touche ```arccos``` permet de faire le contraire : passer du cosinus à l'angle.

Exemple : 
- $\cos(60) = 0,5$
- $\arccos(0,5)=60$

{: .attention }
Vos calculatrices doivent impérativement être en mode degré. Cherchez sur internet avec "calculatrice mode degré + marque de votre calculatrice" pour faire la manipulation.
Pour vérifier, essayez de faire les deux calculs de l'exemple ; si vous trouvez les mêmes résultats que moi, c'est que votre calculatrice est bien en degrés.


### Déterminer la valeur d'un angle à partir de longueurs

{: .methode }
Voici un énoncé : soit $ABC$ un triangle rectangle en $A$ tel que $AB=8$ et $BC=16$. Déterminer la valeur de l'angle $\widehat{ABC}$


1. On identifie la position des côtés dont on connait les longueurs par rapport à l'angle qu'on cherche.
    - $AB$ est le côté adjacent.
    - $BC$ est l'hypothénuse. 
2. On cherche la formule qui utilise les côtés que l'on connait : dans notre cas, c'est la formule du **cosinus**.
3. On calcule : $\cos(\widehat{ABC}) = \dfrac{AB}{BC}=\dfrac{8}{16}=0,5$
4. On utilise la méthode précédente pour retrouver l'angle : $\boxed{\widehat{ABC}=\arccos(0,5)=60°}$.

### Déterminer une longueur dans un triangle rectangle.

{: .methode }
Voici un énoncé : soit $ABC$ un triangle rectangle en $A$ tel que $AB=5$ et $\widehat{ACB}=22,62°$. Calculer $AC$.

1. On cherche la formule qui lie les informations données et ce qu'on cherche ($AC$)
    - On cherche le lien entre l'angle donné et le côté à déterminer. Ici, $AC$ est le côté **adjacent** à $\widehat{ACB}$.
    - On cherche le lien entre l'angle et la longueur donnés : ici, $AB$ est le côté **opposé** à $\widehat{ACB}$.
    - La formule qui lie les trois informations est $\tan{\widehat{ACB}}=\dfrac{\text{opposé}}{\text{adjacent}}=\dfrac{AB}{AC}$

2. On remplace les données connues : $\tan(22,62)=\dfrac{5}{AC}$
3. On trouve AC.
    - **Méthode 1. Le produit en croix.**
    $\tan(22,62)=\dfrac{\tan(22,62)}{1}$, donc l'égalité peut s'écrire : $\dfrac{\tan(22,62)}{1}=\dfrac{5}{AC}$
    L'égalité de deux fractions correspond à une situation de proportionnalité.
    On peut donc faire un produit en croix pour trouver $AC$.
    - **Méthode 2. L'équation.**
    On cherche $AC$ ; on cherche à exprimer $AC$ *en fonction* des autres valeurs.
    Commençons par multiplier l'égalité par $AC$ : $\color{red}{AC\times}\tan(22,62)=\color{red}{AC\times}\dfrac{5}{AC} \Longleftrightarrow AC\times\tan(22,62)=5$
    Divisons par $\tan(22,62)$ pour finir d'isoler $AC$ : $\dfrac{AC\times\tan(22,62)}{\tan(22,62)}=\dfrac{5}{\tan(22,62)} \Longleftrightarrow AC=\dfrac{5}{\tan(22,62)}$
    - Dans les deux cas, $AC$ se calcule ensuite à la calculatrice, et $\boxed{AC = 12}$

### Pour préparer la première.

Voir ce [lien](https://codimd.apps.education.fr/s/xjPSzvS3A#).
