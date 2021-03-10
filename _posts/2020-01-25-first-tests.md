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

<br>But despite of my extensive experience on 2D arrays, I learned something new again.
This is a debug test on the perfomance of the sphere points creation.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Qusfgm8KKrA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

I skipped the mathematical calculations completely.
By creating a 3D array, and then spawning a sphere collision that deletes every point that it's outside of it, I managed to save a lot of perfomance issues on the creation of the sphere array!

Now wether I choose to save the points, or turning the project full procedural will have no huge implications on the perfomance of the project.

The issue with creating a website with unreal engine is that it is not currently supported in the newest releases, and the most new release is 4.24 is upheld by some developers in github. I don't think it's very active, but you can build a custom unreal engine version from source.<br>

I tried it, it has critical errors.
So back to 4.22. At least I found some extensions that allow me to use a website as the interface of the project.
