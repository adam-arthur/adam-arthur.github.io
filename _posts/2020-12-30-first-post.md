---
layout: post
title: First Post! Topics of interest
---

Hello all! 

I've decided to start contributing more heavily to open source, and plan to blog about the journey along the way. A lot of the work I've done over the past years could provide value if exposed in a generic, public (and legal!) way.

There are also certain areas of focus that could use more discussion and public solutions.

## "Microfrontend" Design
When I was coming up with the design for microfrontends at ThousandEyes, I found there wasn't much info on how to structure frontend services "properly". In the case where articles do cover design, there usually aren't concrete examples. After extensive research and successful implementation, I want to put forward a working design along with an end-to-end, working reference architecture.

## Theory underlying Quality Code
Often discussions around best practices and code quality fall short of the rigor that these topics deserve. Everyone has their own stylistic preferences, but it's important to objectively quantify the differences between various stylistic approaches.

If you have a long line, where do you place the line break, and why? A lot of these discussions fall into habit, or convention, rather than rigorous justification. The process by which the brain parses and converts visual regions into structured information is super important, and style should have more focus on "visual fragments".

For example, [prettier](https://prettier.io/) has taken off in the JS world, but the code it produces is quantifiably "poor" from a UX standpoint. Often linebreaks are placed in non-ergonomic ways, and implementation details are made more prominent by how they're positioned. I have plans to implement my own version of prettier that asserts more rigorous justification around the style of the output.


## JS Based Game Networking/Engine
Every developer seems to build their own game engine at some point, and it's certainly a bloated market. However, there aren't any robust and intuitive JS based game engines out there that are built with an appropriate separation of concerns. 

[Phaser](https://phaser.io/) is certainly nice for building small games, but I grew frustrated with some of the design decisions, such as a hardcoded "health" property for game objects, and a plugin system that's a bit awkward. It's also difficult and inefficient to run it on the server for networked games, and nobody wants to maintain two largely duplicated branches of code for both the client/server. 

Beyond the engine, I plan to implement a networking component that makes it easy to create JS-based multiplayer games that can be deployed to the cloud.

<!-- <div>
{% prismc javascript %}
var gem = "jekyll-prismjs-compile";

console.log("gem");
{% endprismc %}
</div> -->