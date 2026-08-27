---
title: 'The 16-Hertz Bounce That Almost Broke Apollo 13'
description: 'A rocket can shake itself apart through its own fuel lines, with no wind and no engine failure involved. Here is the feedback loop, and why the fix is a bottle of gas.'
pubDate: 'Aug 27 2026'
---

Two minutes into Apollo 13's climb, the center engine on the second stage shut itself off early. Nothing had exploded or leaked. The engine was bouncing up and down 16 times a second, pulling 68 g, flexing the frame it was bolted to by about three inches. Postflight analysis said one more cycle of growth would have cracked the structure.

Most people assume a rocket shakes because combustion is violent, or because it is punching through thick air. Pogo is neither. It needs no wind and no outside kick. It is a loop the rocket runs on itself, between the metal of the vehicle and the liquid in its own plumbing, and once that loop closes it feeds on the engine's thrust. Engineers named it after the pogo stick, because from the outside that is what the vehicle is doing.

## The loop, one step at a time

Start with the fact that a rocket is not rigid. A Saturn V was 363 feet of thin-walled aluminum tank with heavy engines hung off the bottom. Along its long axis it behaves like a very stiff spring with a weight on the end. Push it and it springs back at a set rate. That rate is its **natural frequency** (how many times per second a structure oscillates on its own after you disturb it, measured in **hertz**, or cycles per second). For a big launch vehicle bouncing along its length, that lands somewhere between a few hertz and about twenty.

Now hang the plumbing on it. The engine is fed by a **turbopump** (a pump spun by its own small turbine, shoving propellant into the chamber at thousands of pounds per square inch). Between the tank and that pump sits a long column of liquid oxygen. The column has mass, the flexible tank above it acts like a spring, and so the fluid side has a natural frequency of its own, completely separate from the structure's.

Here is where it goes wrong. The structure twitches, so the engine moves. The pump moves with it, but the liquid in the line does not move in step, so pressure at the pump inlet rises and falls. Inlet pressure sets how much propellant reaches the chamber, so chamber pressure swings, so thrust swings. And thrust is the force pushing on the structure that twitched in the first place. If that thrust pulse arrives at the right moment in the cycle, it pushes the structure the way it was already going. That is positive feedback. Amplitude does not settle. It doubles, and doubles again.

What makes pogo nasty is that you cannot design the two frequencies apart once and walk away. As the tanks drain, the vehicle gets lighter and its structural frequency climbs through the burn. The feed system's frequency drifts too. Somewhere in the ascent, the two curves cross. Every liquid rocket has a few seconds where the plumbing and the airframe agree on a number, and the only question is how strong the loop is when they meet.

I got why the standard fix works from a homework problem that had nothing to do with rockets. In my system dynamics coursework I built a two-mass, two-spring model in MATLAB and swept the forcing frequency to plot the response. Then I softened one spring and reran it. The two natural frequencies split apart, and the peak that had been sitting directly under my forcing frequency slid sideways down the axis. The amplitude there collapsed, and I had not added a single unit of damping. Nothing was absorbing energy. I had moved the resonance out of the way. That is the trick rockets use.

The fix is called a **pogo accumulator**, and it is the least glamorous part of a launch vehicle: a small bottle of gas plumbed into the liquid oxygen line right before the pump. Liquid oxygen barely compresses, which is what makes that column such a stiff spring. Add a pocket of gas and you have installed a soft spring in the middle of it. The feed system's frequency drops well below anything the structure can do, the two never line up again, and the loop never closes. NASA got there with a working group of roughly a thousand people, and the answer was helium injected into the LOX feed lines.

## Why it still shows up on the flight schedule

Pogo has been shaking crews around since before Apollo. It nearly cost Gemini its ride: the Titan II first stage bounced hard enough in development that the rocket was not cleared to carry astronauts until it was fixed. Apollo 13 got the extreme version, and what saved that stage was not a suppression system working. It was the engine's own sensors giving up and shutting it down before the structure did. The other stages burned longer to cover the lost thrust.

It is not a historical problem. Artemis II flew on April 1, 2026, and each of its four RS-25 engines carries a pogo accumulator just upstream of the high pressure oxidizer turbopump, precharged with helium and then kept charged with gaseous oxygen bled from the engine's own heat exchanger. A 1960s fix, still riding to orbit. It is also not finished work. Papers from 2025 are still refining how to calculate flow resistance at an accumulator's port, and another thread is chasing active suppression, using sensors and control loops instead of a fixed gas volume, because heavy-lift vehicles have so many closely spaced structural modes that one bottle tuned to one frequency stops being enough.

Pogo is not a materials failure or an engine failure. Every part works as designed. The failure lives in the connection between them, in a loop nobody drew on purpose, and you will not find it by testing the pump and the tank separately. That is also why the fix is a gas bubble and not a stronger bracket. You do not out-muscle a resonance. You move it.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
