---
layout: post
title:  "Transition de pages 'morphing' en SVG"
date:   2018-03-10 10:34:58 +0100
intro : Ceci est article à propos de ce qui doit être fait.
categories: webdesign traduction
---

** Article traduit directement de Codrops, écrit par Mary Lou - https://tympanus.net/codrops/2017/08/08/morphing-page-transition/ **

Demo : https://tympanus.net/Development/MorphingPageTransition/
Code source : https://tympanus.net/Development/MorphingPageTransition/MorphingPageTransition.zip

Aujourd'hui, nous aimerions partager un effet de transition morphing entre deux pages. L'idée est de transformer un chemin SVG tout en déplaçant une page vers le haut, créant un visuel intéressant et fluide.
Pour les animations, nous utilisons anime.js et pour certains effets de lettres, nous utilisons Charming. Dans la démo, nous utilisons une "transition d'intro" pour mettre en évidence l'effet, mais ce n'est que l'un des nombreux cas d'utilisation possible.
*** Attention: Dans la demo, nous utilisons des propriétés récentes de CSS, tel que Flexblox ou des variables CSS sans "fallback", veillez à utiliser un navigateur compatible. ***
Le code qui nous permet de faire bouger la forme avec la page d'introduction est celui-ci :


{% highlight html %}
<div class="content content--intro">
	<div class="content__inner">
		<!-- ... -->
	</div>
	<div class="shape-wrap">
		<svg class="shape" width="100%" height="100vh" preserveAspectRatio="none" viewBox="0 0 1440 800" xmlns:pathdata="http://www.codrops.com/">
			<path
				d="M -44,-50 C -52.71,28.52 15.86,8.186 184,14.69 383.3,22.39 462.5,12.58 638,14 835.5,15.6 987,6.4 1194,13.86 1661,30.68 1652,-36.74 1582,-140.1 1512,-243.5 15.88,-589.5 -44,-50 Z"
				pathdata:id="M -44,-50 C -137.1,117.4 67.86,445.5 236,452 435.3,459.7 500.5,242.6 676,244 873.5,245.6 957,522.4 1154,594 1593,753.7 1793,226.3 1582,-126 1371,-478.3 219.8,-524.2 -44,-50 Z">
			</path>
		</svg>
	</div>
</div><!-- /content--intro -->

<div class="content content--fixed">
	<div class="content__inner">
		<!-- ... -->
	</div>
</div><!-- /content--fixed -->

{% endhighlight %}

Le contenu fixe (content--fixed) se situe en dessous du contenue de l'introduction (content--intro). Quand l'introduction se déplace, le contenu fixe est révélé. En même temps, nous transformon le chemin SVG en un autre défini dans le "pathdata:id". Quand nous créeons les deux chemins, nous devons être sur qu'ils possédent le même nombre de points pour avoir une transition fluide et lisse.
Nous espérons que vous aimerez ce petit effet et qu'il vous sera utile !

![TransitionSVG screenshot](../../../../../assets/images/2018-03-08-TransitionSVG/2018-03-08-TransitionSVG-01.jpg){:class="img-responsive"}
![TransitionSVG screenshot](../../../../../assets/images/2018-03-08-TransitionSVG/2018-03-08-TransitionSVG-02.jpg){:class="img-responsive"}


anime.js : http://animejs.com/
Charming : https://github.com/yuanqing/charming
