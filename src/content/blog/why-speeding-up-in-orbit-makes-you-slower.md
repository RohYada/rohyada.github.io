---
title: 'Why Speeding Up in Orbit Makes You Slower'
description: 'Catching another spacecraft means dropping below it, not accelerating toward it. The orbital mechanics behind why firing your engine forward pushes you further behind.'
pubDate: 'Aug 22 2026'
---

If you are trailing another spacecraft in the same orbit and you fire your engine forward to catch it, you will fall further behind. Not for a minute or two. Permanently, and by more on every lap.

The picture most people have of orbit is a highway. Two vehicles in the same lane, and the one in back closes the gap by stepping on the gas. That model is not slightly off. It gets the sign backwards. In orbit, stepping on the gas moves you away from whatever you were chasing.

Here is why. An orbit is not a road you steer along. It is a shape, and the shape is set almost entirely by how much energy you have. Add energy and the loop gets bigger. Take energy away and it gets smaller. Your engine does not really control where you are. It controls the size of the loop, and the loop controls how fast you travel and how long a lap takes.

## Your engine sets the size of the loop, and the loop sets your speed

The equation that governs this is called vis-viva, and it is the one piece of orbital mechanics worth memorizing:

**v² = μ (2/r − 1/a)**

Three symbols. **μ** (the Greek letter mu, called the standard gravitational parameter) is just a number describing how strongly a particular body pulls; for Earth it is about 398,600 cubic kilometers per second squared. **r** is your current distance from the center of the Earth, not from the ground. **a** is the semi-major axis, which is half the long axis of your ellipse. It is the single number that sets your orbit's size and your energy.

For a circular orbit, r and a are the same thing, and the equation collapses to v = √(μ/r). The bigger your orbit, the slower you go. Not as a side effect. As a direct consequence.

Run the numbers on the International Space Station. At 420 kilometers up, it moves at 7.657 kilometers per second. Drop to 400 kilometers, twenty kilometers lower, and the required speed rises to 7.669 kilometers per second. Lower is faster. Always.

Now do the burn accounting. Say you are in that 400 kilometer circle and want the 420. The standard way is a Hohmann transfer: one burn to stretch your circle into an ellipse that just touches the higher altitude, and a second at the top to round it back out. The first burn costs about 5.6 meters per second. The second costs about 5.7. You have spent roughly 11.3 meters per second of your fuel budget, and you are now moving about 11.7 meters per second slower than when you started. You burned propellant to go slower. That is what raising an orbit is.

The part that actually matters for chasing something is the lap time. Kepler's third law says the orbital period depends only on the semi-major axis: T = 2π√(a³/μ). At 400 kilometers a lap takes 92.55 minutes. At 420 kilometers it takes 92.97 minutes. About 25 seconds longer, every lap.

I did not really believe any of this until I watched it happen. In an orbital mechanics problem set I set up a two-body propagation in MATLAB with a chaser 100 kilometers behind a target, both in the same 400 kilometer circular orbit, and gave the chaser a prograde burn to close the gap. The gap grew. It grew again on the next lap, and the one after. I spent close to an hour convinced my integrator had a sign error in the acceleration term before I accepted that the code was fine and my intuition was the broken part. I had added energy, stretched the semi-major axis, lengthened my own period, and handed the target a head start on every lap.

The fix was to do the opposite. A retrograde burn of about 5.6 meters per second, braking rather than accelerating, dropped the chaser 20 kilometers lower. Now the chaser's lap was 25 seconds shorter than the target's. Twenty-five seconds of head start at 7.66 kilometers per second works out to roughly 190 kilometers of along-track ground per orbit. The 100 kilometer gap closed in well under a lap. Then you circularize back up to meet the target where it lives. You catch something in orbit by falling below it and letting geometry do the work.

## Why it matters

Not a classroom curiosity. It is the architecture of every rendezvous flown. When a Dragon capsule launches toward the ISS, it does not aim at the station. It inserts into a lower, faster orbit deliberately behind and below, then runs a sequence of phasing burns that walk it up to the station's altitude at exactly the moment the two are in the same place. Get the phasing wrong and you do not arrive late by a few seconds; you arrive on the wrong side of the planet. That dependency showed up in September 2025 when Northrop Grumman's Cygnus XL shut its main engine down early during two separate rendezvous burns. The vehicle was healthy, but NASA and Northrop delayed the station arrival anyway, because the burns were not producing the orbit the phasing plan assumed. The same physics runs in reverse for station keeping. Atmospheric drag steadily strips energy from the ISS, which drops it lower and therefore makes it move faster, and reboosts have to put that energy back. Progress has done that job for decades, and Dragon has now joined it, performing six reboosts across its attached mission, five in 2025 and one on January 23, 2026.

The useful thing to take from this is that in orbit, speed and energy point in opposite directions. Fast means low and low means short on energy, so anything that drains energy from a satellite makes it faster on the way down. Once you stop thinking of thrust as something that moves you toward a target and start thinking of it as something that resizes your loop, rendezvous stops looking like chasing and starts looking like scheduling.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
