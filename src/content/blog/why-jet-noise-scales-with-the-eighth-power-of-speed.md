---
title: 'Why Cutting a Jet''s Exhaust Speed in Half Makes It 256 Times Quieter'
description: 'Jet noise scales with roughly the eighth power of exhaust velocity, which means quieting an engine is a mixing problem, not a soundproofing problem.'
pubDate: 'Sep 05 2026'
---

Slow a jet engine's exhaust from 580 meters per second to 290 and the sound it radiates drops by a factor of about 256. Not 2. Not 4. 256.

Most people assume a loud engine is a powerful engine, and that making it quieter means wrapping it in better insulation. Both parts are wrong. The roar you hear on a runway is not made inside the engine at all. It is made in the open air behind it, in the few meters where the exhaust column shreds itself against the still air around it. Nothing solid is vibrating. The sound source is the turbulence itself, and the engine has already finished its job by the time that noise gets created.

That distinction matters because it tells you what knob to turn. If the noise came from machinery, you would fix it with damping. Because it comes from a velocity difference in the air, you fix it by making the exhaust slower, or by making it blend into the surrounding air faster. Everything the industry has done to quiet airliners since the 1960s is one of those two moves.

## The Exponent That Runs the Whole Problem

In 1952 James Lighthill rewrote the equations of fluid motion so that a chunk of turbulent air could be treated as if it were a loudspeaker sitting in otherwise still air. What fell out was a scaling law: the acoustic power a jet radiates goes roughly as the eighth power of its exhaust velocity. Write it as P proportional to V^8, where **acoustic power** is just the energy per second the jet dumps into the air as sound. Experiments have backed the exponent up well for subsonic jets, and it drifts toward lower values once the exhaust goes supersonic and new sources like shock noise take over.

An eighth power is a violent exponent. A 10% cut in exhaust speed cuts the radiated sound power by more than half. Halve the speed and you divide the sound by 2^8, which is 256. In **decibels** (a log scale where every 10 dB is a factor of 10 in power, and 3 dB is a doubling) that is about 24 dB, roughly the difference between standing next to a running lawnmower and standing next to a refrigerator.

I ran into this in a propulsion problem set. The task looked routine: back out exhaust velocity from thrust and mass flow for a 1960s turbojet and a modern high-bypass turbofan producing the same net thrust. Thrust is mass flow times the velocity you add to the air, so an engine can make its thrust by throwing a little air very fast or a lot of air moderately fast. The turbojet landed near 580 m/s. The turbofan, moving far more air, landed near 290 m/s. I plugged both into the V^8 scaling and got a ratio of 256. Same thrust, same airplane speed, two and a half orders of magnitude apart in radiated sound. I had been taught that the big fan on a modern engine was about fuel burn, and it is, but the noise result is not a nice side effect. It is the single largest quieting decision ever made in aviation, and it came out of a term in an equation.

Underneath the exponent is a **shear layer**, the ragged boundary where fast air rubs against slow air. Behind a nozzle you have three streams meeting at once: hot core exhaust, cooler bypass air from the fan, and ambient air standing still. The bigger the speed difference across those boundaries, the more violently the layer rolls up into eddies, and those eddies are the sound source. Cutting exhaust velocity shrinks the speed difference. That is why it works so hard.

## What Six Decibels Costs

Since airframers ran out of easy bypass ratio, the remaining move is to make the streams mix faster so the loud region is shorter. That is what the sawtooth notches on the back of a Boeing 787's nacelle are for. Those chevrons push small streamwise vortices, corkscrews of air spinning along the flow direction, into the shear layer. The vortices stir the core and bypass streams together sooner, which shortens the potential core (the intact high-speed slug of exhaust just behind the nozzle) and knocks down low-frequency noise.

They are not free. The same stirring that quiets the jet costs thrust, on the order of 0.25% in NASA's early nozzle tests and around 0.5% by later industry estimates, and it costs it in cruise too, where there is nobody on the ground to appreciate it. Boeing took the deal anyway. The engines came out quiet enough that they deleted roughly 600 pounds of fuselage sound insulation, which clawed back most of the performance loss. Airbus looked at the same trade and declined.

The pressure is not letting up. On 27 March 2026 the ICAO Council adopted a new Annex 16 Volume I noise standard, Chapter 16, that is 6 dB more stringent for large aircraft, following the CAEP/13 analysis. Six decibels sounds modest until you run it backward through the eighth power law. Six decibels is a factor of about 4 in acoustic power, and to buy that from exhaust velocity alone you would need to slow the jet by roughly 16%, which means moving proportionally more air to hold the same thrust. That is a bigger fan, a bigger nacelle, and more drag. And the leading candidate for the next efficiency jump, CFM's open-fan RISE architecture, throws away the nacelle entirely and reintroduces a noise source (exposed blade tips) that the duct used to contain.

Once you know the exponent, the design history stops looking like a series of clever fixes and starts looking like one constraint applied over and over. Every quiet airliner you have stood under got that way by refusing to throw air backward quickly. The engineering question was never how to absorb the sound. It was how to make thrust without making a fast jet.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
