---
title: 'Why a Rocket Engine''s Exhaust Changes Shape as It Climbs'
description: 'A rocket nozzle can only be perfectly tuned to one altitude, and the shape of the visible plume tells you exactly how wrong it is at any given moment.'
pubDate: 'Aug 19 2026'
---

Watch a launch replay and skip ahead a minute. The flames are not the shape they were on the pad. They started tight and pinched, and now they balloon out wide behind the rocket. Nothing on the engine moved. The air did.

Most people picture a rocket nozzle as a funnel that points the fire backward. That is not what it does. A nozzle converts pressure into speed, and it only does that conversion correctly at one specific outside pressure. Pick that pressure and you have picked an altitude. Every other second of the flight the engine runs mismatched, and the plume shows it.

## What the bell is actually doing

Inside the combustion chamber you have gas at absurd pressure. Raptor, the engine on SpaceX's Starship, runs its chamber somewhere around 300 bar (1 bar is roughly sea-level atmospheric pressure, so this is about 300 atmospheres, or 4,400 psi). That pressure is not thrust. It is stored energy, and the nozzle trades it for exhaust velocity, because thrust comes from throwing mass backward fast.

The trade happens in two stages. The nozzle pinches down to a throat, where the gas hits exactly Mach 1 (the local speed of sound). Then it opens back up. Here is the part that trips people up: once flow is supersonic, widening the duct makes it go *faster*. Below Mach 1, squeezing a pipe speeds the flow up. Above Mach 1, the gas expands and cools so hard that spreading it out wins. The bell after the throat is not aiming anything. It is still accelerating gas.

How much you open it is the whole design decision. Engineers describe it with the **expansion ratio**, which is just the area of the nozzle exit divided by the area of the throat. Sea-level Raptor runs about 34. Raptor Vacuum, the version on Starship's upper stage, runs about 80. Same engine core, same propellants, wildly different bell.

I ran the numbers on that 80 myself in compressible flow, using the area-Mach relation (the equation that ties how much a supersonic duct opens up to how fast the gas leaves it). With a ratio of gas specific heats around 1.2, which is a reasonable stand-in for hot rocket exhaust, an expansion ratio of 80 puts the exit Mach number near 4.75. Push that through the isentropic pressure relation with a 300 bar chamber and the gas leaves the nozzle at roughly 0.25 bar.

That number stopped me. Sea-level air is 1.01 bar. The exhaust is exiting at about a quarter of the pressure of the air it is exiting into.

## Overexpanded, underexpanded, and the plume that tells you which

When exit pressure is below ambient, the nozzle is **overexpanded**. It kept expanding the gas past the point where the outside air could tolerate it. The atmosphere squeezes the plume back inward, and it does that squeezing through oblique shocks that fold into the exhaust just past the lip. That is the pinched, cinched-in look you see on the pad, and if the plume is bright enough you can see the shock diamonds where the flow keeps overshooting and getting compressed again.

The opposite case is **underexpanded**. Exit pressure is higher than ambient, because you are high up and the outside pressure has fallen away. Nothing holds the exhaust in, so it flares out into a wide bell of gas. It looks dramatic, but it is a small loss. That leftover pressure was velocity you never collected.

Overexpansion is the dangerous one. Mild overexpansion just costs performance. Severe overexpansion causes the flow to peel off the nozzle wall entirely, and that separation point does not sit still. It wanders around the inside of the bell, unevenly, which means the engine gets shoved sideways by forces it was never meant to carry. These are called side loads and they are strong enough to bend hardware. There is an old rule of thumb from JPL work in the 1950s, the Summerfield criterion, that says separation shows up once wall pressure near the exit drops below roughly 0.4 times ambient.

My 0.25 bar estimate sits under that threshold. My model is simplified (real exhaust does not hold one clean gamma all the way down the bell, and wall pressure at the lip is not exactly the ideal exit pressure), so it does not settle anything. But it lands in the right neighborhood, and that is the point: a vacuum nozzle at sea level is right on the edge of tearing its own flow off the wall. That is why SpaceX kept Raptor Vacuum's expansion ratio at 80 instead of the 150 or 200 that pure vacuum optimization would want. They gave up specific impulse to buy a nozzle that can survive being lit in atmosphere.

## What it costs to guess wrong

The Space Shuttle's RS-25 makes the price visible. Its nozzle ran an expansion ratio near 78, tuned for the thin air of most of its burn. **Specific impulse** (the standard efficiency measure for a rocket engine, in seconds, essentially how long a pound of propellant can produce a pound of thrust) came in at 452 seconds in vacuum. At sea level, the same engine managed 366. That is 86 seconds of efficiency thrown away at liftoff. Engineers took the hit because the vacuum phase is where the velocity actually gets bought.

This is why big rockets stage their nozzles instead of their engines. The booster gets small bells. The upper stage gets huge ones. Aerospike engines have been chased for decades because they self-adjust to ambient pressure, and they are still hard enough to cool that nobody flies one.

So the changing plume is not a lighting effect or a camera artifact. It is the atmosphere losing its grip on the exhaust as the rocket climbs. Every rocket you have watched launch was flying with the wrong nozzle for almost the entire burn, and the engineers knew it before it left the pad. They just picked which altitude to be right at.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
