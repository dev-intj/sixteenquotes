---
title: Init and problems
layout: post
background: https://dev-intj.github.io/sixteenquotes/img/initandproblems/init1.png
subtitle: Choosing the right tool.
---

One of the most complex challenges in the making of a project is carefully choosing the right framework/technology. I have experience with three.Js, Babylon.Js (Both of them are open source JavaScript libraries to construct and generate 3D graphics.) two of the most popular and powerful in that field.The scope of this project is vast. I haven’t developed anything close on the level of difficulty with these tools, regardless of that the development of prototypes has begin.

# Hot the tests went

Creating a circle and grabbing the points ( The points will be the locations of the messages )<br>
then with this formula, I convert the square into a circle
and the unusued points get deleted.

> float dx = x * sqrtf(1.0 - (y*y/2.0) - (z*z/2.0) + (y*y*z*z/3.0));<br>

> float dy = y * sqrtf(1.0 - (z*z/2.0) - (x*x/2.0) + (z*z*x*x/3.0));<br>

> float dz = z * sqrtf(1.0 - (x*x/2.0) - (y*y/2.0) + (x*x*y*y/3.0));<br>

But alas, the problems have started rising, for example the performance.
Unless I set nothing but 50 messages displaying at once, this is an undesirable way to do it.<br>

The shape generation takes too long cause of the complex calculations.
I have thought about generating the points my self and saving them, providing the person that uses the website only the points. (or maybe initializing 10 different 3D arrays which will take extremely long at the start of loading the website) Which takes the loading time away from the calculation but the performance issue still remains.

<b>Both babylon.js and three.js are unusable above 50 messages being displayed.</b>

However, I want the project to remain in a website form. I will most likely have to rely in a game engine, and the interface will be handled from a front-end technology, like, react.
