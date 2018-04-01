---
layout: post
title:  "Diaporama effet glitch"
date:   2018-04-04 10:34:58 +0100
intro : Un diaporama simple utilisant un effet glitch en CSS pour la transition des diaporama
categories: webdesign traduction
preview : 2018-04-04-UX-UI-difference-preview-02.jpg
---

![diaporama-glitch-effect screenshot](../../../../../assets/images/2018-04-04-diaporama-effet-glitch-01.jpg){:class="img-responsive"}

Démo : https://tympanus.net/Development/GlitchSlideshow/
Sources : https://tympanus.net/Development/GlitchSlideshow/GlitchSlideshow.zip

Après avoir joué avec l'effet de glitch CSS experimental pour textes et images, une des mes premiéres questions était

"Comment est-ce que je peux l'utiliser pour un diaporama ?"

L'animation que nous utilisons pour l'effet de glitch était configuré pour s'éxécuter de manière infini, du coup, les keyframes doivent être ré-ajustées. Dans un diaporama, le scénario est différent: nous voulons appliquer l'effet de glitch à un moment spécifique et échanger l'image actuelle par la suivante du diaporama. Ce genre d'animation peut être utilisé dans un effet de hover.

C'est exactement ce que fait ce diaporama : il fait une transition au diaporama suivant en utilisant un effet de glitch. Pour le fonctionnement, il échange les calques de glitch un par un et arrête de glitcher au moment ou la derniére image arrive.

ATTENTION : la propriété "clip-path" de CSS ne marche pas sur Internet Explorer et IE

![diaporama-glitch-effect screenshot](../../../../../assets/images/2018-04-04-diaporama-effet-glitch-02.jpg){:class="img-responsive"}
![diaporama-glitch-effect screenshot](../../../../../assets/images/2018-04-04-diaporama-effet-glitch-03.jpg){:class="img-responsive"}
![diaporama-glitch-effect screenshot](../../../../../assets/images/2018-04-04-diaporama-effet-glitch-04.jpg){:class="img-responsive"}

** Article traduit directement de Codrops, écrit par Mary Lou - https://tympanus.net/codrops/2018/03/13/glitch-effect-slideshow/ **
