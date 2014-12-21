---
layout: more_page
title: Planetoids
---

<div onselectstart="return false;"><canvas id="Canvas_Planetoids" style="border: none; position: relative;" width="800" height="600" oncontextmenu="return false;"></canvas></div>

## Planetoids

For my exams of my first year of DAE I had to remake a classic game. It was for my maths & physics class so graphics weren't that important. I chose to remake Asteroids, but give it my own spin. I added my own controlls and upgraded the spaceship's laser.

Then years later I decided to remake Planetoids. I first used WebGL for it's graphics, though later decided to use the HTML5 canvas instead. Now Planetoids is fully playable in any browser.

### Physics

In the original I wrote all physics myself, they were very basic, glitchy and really rough. Rocks couldn't turn, and their collision wasn't very good, but still for a first year programmer not bad at all. Now for the remake I decided to use an external library: [Box2D Web](https://code.google.com/p/box2dweb/). A javascript version of the Box2D physics engine. This gives much nicer physics and reduced the code I had to write myself.

### Graphics

For graphics, in the original, I used the engine of my teacher, Kevin Hoefman, it was very basic but more than enough when only using vector graphics. For the remake I use the HTML5 canvis, without any additional libraries.



<script src="../js/jquery-2.1.1.min.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/Box2dWeb-2.1.a.3.min.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/01-RequestAnimFrame.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/02-Planetoids_Init.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/03-Planetoids_Game.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/04-Helpers.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/05-SpaceShip.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/06-Lasers.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/07-Rocks.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/08-Powerups.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/09-Stars.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/10-SlicePoint.js"></script>
<script type="text/javascript" src="../planetoids_v2_0/JS/11-Input.js"></script>

<script type="text/javascript">
	$(document).ready(function() {
		InitPlanetoids(document.getElementById('Canvas_Planetoids'), 10);
	});
</script>