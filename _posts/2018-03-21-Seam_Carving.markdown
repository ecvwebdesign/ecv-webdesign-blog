---
layout: post
title:  "Le Seam Carving"
date:   2018-03-21 10:34:58 +0100
intro: Si vous aussi vous avez peur des images déformées, des images trop grandes, ou trop petites pour être à leur place... cet article est fait pour vous !
categories: OUTILS CODE
preview : 2018-03-21-Seam-Carving-preview.jpg
---

![SEAM CARVING](../../../../../assets/images/2018-03-21-Seam-Carving-content.jpg){:class="img-responsive"}

Qu’est-ce que le Seam Carving ? C’est littéralement le rognage des contours d’une photo. Ariel Shamir et Shai Avidan sont deux chercheurs qui ont trouvé (pun non-intended) un algorithme permettant de redimensionner n’importe quelle image sans pour autant la déformer. (Comme vous l’avez probablement déjà fait…)
On connait tous ce moment où la photo que l’on veut utiliser en hero section - par exemple - n’est pas à la bonne taille. Frustrant n’est-ce pas ? Tu entrevois le lancement de Photoshop juste pour resizer une image ?
Grâce au Seam Carving tu seras capable d’agrandir cette image, aussi bien verticalement qu’horizontalement.

Mais comment ça marche ?

L’algo prend tout simplement compte de la partie la plus « importante » de l’image et évite de la déformer. Tu peux également déterminer manuellement quel sera l’élément central, qui devra rester immobile ou inchangé pendant tes modifications.
L’algorithme analyse et utilise les lignes horizontales et verticales de la photo, les étire, les supprime ou les reproduit pour avoir un rendu aussi naturel que possible.


Je t’invite à directement regarder cette vidéo : <iframe width="560" height="315" src="https://www.youtube.com/embed/6NcIJXTlugc" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

Et tu connais pas la meilleure ?
Ce script est en open source via ce lien GIT : https://github.com/esimov/caire

À toi de coder !
