---
title: Init and problems
layout: post
background: https://dev-intj.github.io/sixteenquotes/img/initandproblems/init1.png
subtitle: Choosing the right tool.
---

As all devs know, one of the big challenges is choosing the right framework/technology for the project. I have experience with three.js, babylon.js ( Both of are javascript libraries to create and display 3D graphics ) two of the most popular and powerful in that field. But, the scope of this project is really big and I haven't done anything close to it with these big tools, regardless of that I will create some prototypes.

# Hot the tests went

Creating a circle and grabbing the points ( The points will be the locations of the messages )<br>
then with this formula, I convert the square into a circle
and the unusued points get deleted.

> float dx = x * sqrtf(1.0 - (y*y/2.0) - (z*z/2.0) + (y*y*z*z/3.0));<br>

> float dy = y * sqrtf(1.0 - (z*z/2.0) - (x*x/2.0) + (z*z*x*x/3.0));<br>

> float dz = z * sqrtf(1.0 - (x*x/2.0) - (y*y/2.0) + (x*x*y*y/3.0));<br>

But alas, the problems have started rising, first of all, the perfomance.
Unless I only want 50 messages displaying at once, this is a bad way to do it.<br>

The shape generation takes too long cause of the complicated calculations.
I have thought about generating the points my self and saving them, providing the person that uses the website only the points( or maybe initializing 10 different 3D arrays which will take too long at the start of loading the website ), which takes the loading time away from the calculation but the perfomance issue still remains.

<b>Both babylon.js and three.js are unusable above 50 messages being displayed.</b>

I still want the project to be in a website form, so I have to turn into a game engine and for a front end using a framework like react.
