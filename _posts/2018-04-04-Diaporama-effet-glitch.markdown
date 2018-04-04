---
layout: post
title:  "Diaporama effet glitch"
date:   2018-04-04 10:34:58 +0100
intro : Un diaporama utilisant un effet glitch en CSS pour la transition entre les images.
categories: UI
main-image: 2018-04-04-UX-UI-difference-main-image.jpg
preview : 2018-04-04-UX-UI-difference-preview.jpg
---

![diaporama-glitch-effect screenshot](../../../../../assets/images/2018-04-04-diaporama-effet-glitch-01.jpg){:class="img-responsive"}

Démo : https://tympanus.net/Development/GlitchSlideshow/
Sources : https://tympanus.net/Development/GlitchSlideshow/GlitchSlideshow.zip

Après avoir joué avec l'effet de glitch CSS experimental pour textes et images, une des mes premières questions était :

"Comment est-ce que je peux l'utiliser pour un slider ?"

L'animation que nous utilisons pour l'effet de glitch est configurée pour s'éxécuter de manière infinie, de ce fait, les keyframes doivent être ré-ajustées.

Dans un diaporama, le scénario est différent : nous voulons appliquer l'effet de glitch à un moment spécifique et changer l'image actuelle par celle qui doit suivre. Ce genre d'animation peut être utilisée avec un hover par exemple.

C'est exactement ce que fait ce slider. Pour le fonctionnement, il échange les calques de glitch un par un et s'arrête au moment où la dernière image arrive.

ATTENTION : la propriété "clip-path" de CSS ne marche pas sur Internet Explorer.

![diaporama-glitch-effect screenshot](../../../../../assets/images/2018-04-04-diaporama-effet-glitch-02.jpg){:class="img-responsive"}
![diaporama-glitch-effect screenshot](../../../../../assets/images/2018-04-04-diaporama-effet-glitch-03.jpg){:class="img-responsive"}
![diaporama-glitch-effect screenshot](../../../../../assets/images/2018-04-04-diaporama-effet-glitch-04.jpg){:class="img-responsive"}

** Article traduit directement de Codrops, écrit par Mary Lou - https://tympanus.net/codrops/2018/03/13/glitch-effect-slideshow/ **
