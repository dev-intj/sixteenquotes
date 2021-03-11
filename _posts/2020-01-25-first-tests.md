---
title: First tests with Unreal are promising!
layout: post
subtitle: Perfomance, potential and systems behind it.
background: https://dev-intj.github.io/sixteenquotes/img/ue4.png
---

# Turning the code from javascript to C++/blueprints.

<b>Beyond amazed</b>
<br>Creating the 3D array was challenging but I already have made something complicated using 2D array in UE4.<br>

<a class="btn btn-primary" href="https://www.youtube.com/embed/3nEt5O6Sbjo" role="button">Check the project I am reffering to</a><br>

<br>But despite my extensive experience on 2D arrays, I discovered something new again.
This is a debug test on the performance of the sphere points creation.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Qusfgm8KKrA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

I skipped the mathematical calculations completely.
By creating a 3D array, and then spawning a sphere collision that deletes every point that it's outside of it, I managed to save many performance issues on the creation of the sphere array!

Now wether I choose to save the points, or turning the project full procedural will cause no considerable implications on the performance of the project.

The issue with packaging a project into a website utilizing unreal engine is that currently, it's unsupported in the newest releases. Epic Games(the company that owns unreal engine) turned the development to an open source, and the community is unactive<br>

Regardless of that I compiled the open source release, it produces critical errors.
So back to 4.22(the last official engine version that supports emscripten). The good news, I discovered some extensions that allow me to use react as the interface of the project.
