---
layout: post
title: 'Southpaw Custom Keyboard'
---

Custom keyboards have always been a passion of mine, but I've always ended up using someone else's PCB and case designs. With this [Southpaw-style](https://en.wikipedia.org/wiki/Southpaw_stance) board, derived from Boxing as well as first-person camera games, the number-pad is on the left hand side. While this is not traditional as boards usually have navigation keys (Enter and Tab) with the number pad, the Southpaw-style allows for the right hand to stay on the mouse while the left hand handles number/data entry. 

There also was the design choice of the split space, this is due to the 'rattly' nature of a 7u spacebar, where typically only a third of the bar is pressed. This usually results in the actuation starting by the stabilizers, rather than centered on the switch. Splitting the spacebar allows for each switch to be the focus of the actuation, giving a better feel to the keypress.

[This board](https://github.com/gek27/southPawKeeb) was designed in Kicad from scratch and it implements the Teensy 2.0++ board, which was chosen over a pro-micro due to the key-matrix being rather large. This board also uses the QMK firmware for easy development and changes.

{% include image.html url="https://github.com/gek27/southPawKeeb" image="projects/proj-2/kicad.jpg" %}

I learned much from this project, mainly surrounding the design and prototyping of a board in Kicad. Taking the design, routing the traces, and assuring manufacturability were all major steps in this process. The board was manufactured and created. 

While the electrical-engineering and software components were realized, the stability and mechanical design needed some work. Future revisions of the board will call for better stabilization, notably standoff support through the PCB directly, rather than just the top plate + backplate.
