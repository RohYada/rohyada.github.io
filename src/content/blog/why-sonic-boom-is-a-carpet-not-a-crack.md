---
title: 'Why a Sonic Boom Is a Carpet, Not a Crack'
description: 'Most people think the sonic boom happens once, when a plane breaks the sound barrier. It doesn''t. Understanding why is changing how engineers design the next generation of supersonic jets.'
pubDate: 'Jun 19 2026'
---

Most people think you hear a sonic boom because a plane just broke the sound barrier. In reality, the plane has been making that boom continuously for the entire supersonic leg of its flight, and you hear it because you were standing on the ground when the boom's geometry swept past you.

When any aircraft moves through air, it pushes pressure waves outward in all directions. Those waves travel at the speed of sound, roughly 767 mph at sea level. As long as the aircraft stays subsonic, the pressure waves spread out ahead of it, and the air in front has time to see the plane coming and move aside. Go faster than sound, though, and the aircraft outruns its own pressure field. The waves can't get ahead of the plane anymore. They pile up behind it concentrically, stacking into a cone shape that trails the aircraft at all times. Every point on that cone is a shock wave, a sudden, sharp discontinuity in pressure, where all those stacked-up waves have merged into one boundary. This cone has a name: the Mach cone.

## Why the Cone Determines Everything

The geometry of that cone depends entirely on how fast the aircraft is going relative to the speed of sound. The Mach number (M) is just that ratio: aircraft speed divided by local speed of sound. The half-angle of the cone, called the Mach angle (represented by the Greek letter μ), follows one formula: μ = arcsin(1/M). The faster the aircraft, the narrower the cone.

In my aerodynamics class we worked through this for several cases. At Mach 1.5, μ comes out to about 42 degrees (a fairly wide cone). At Mach 2, it narrows to roughly 30 degrees. At Mach 3, it's down to 19 degrees. The next step was mapping that geometry onto a real flight profile. If a Concorde cruises at 50,000 feet at Mach 2, how wide a strip of ground does the cone intercept? The answer follows from trigonometry: roughly one mile of ground width per 1,000 feet of altitude. At 50,000 feet, the Mach cone sweeps a path about 50 miles wide across the surface below. Every person in that 50-mile corridor hears the boom as the cone moves through their location. Not because the plane passed directly overhead, but because the cone's geometry happened to intersect where they were standing.

This is what engineers mean by the boom carpet. As the aircraft moves forward, the cone sweeps continuously across the ground. It is not a single event. It is a persistent geometric consequence of supersonic flight, unrolling across the landscape for the entire duration the aircraft stays above Mach 1.

The pressure signature that actually reaches your ears is not a simple spike. It takes an N shape. There is a sharp upward pressure jump as the nose shock reaches you, a gradual fall to below ambient pressure as the aircraft's body passes overhead, then a sharp return to normal as the tail shock arrives. Those two sharp steps are why a sonic boom sounds like two cracks in quick succession rather than one. Each edge of the N-wave is a distinct shock, and each shock produces a distinct sound. The rise time at each edge is typically 2 to 20 milliseconds; the full waveform from first crack to second lasts somewhere between 100 and 400 milliseconds, depending on the size of the aircraft.

## Why This Led to a 52-Year Ban

The N-wave from a large supersonic aircraft is genuinely disruptive at ground level. Concorde-era booms measured above 100 PLdB. PLdB stands for Perceived Level decibels, a unit specifically designed to capture how annoying impulsive sounds are, rather than measuring them the same way you'd measure highway noise. In practical terms, a 100-plus PLdB boom sounds like close thunder, twice in quick succession, without warning. In 1973, the FAA banned supersonic flight over land in the United States under Title 14 CFR Section 91.817. The regulation stood for 52 years.

What engineers realized is that the N-wave is not inevitable. It is the result of the shock waves from a conventional aircraft's nose, cockpit, wings, and tail all merging as they propagate downward. If you design the aircraft so those shocks stay separated, the N-wave never forms. Instead of two sharp cracks, the ground observer hears a low-frequency thump.

NASA's X-59 QueSST (Quiet SuperSonic Technology) aircraft is built around exactly this principle. The X-59 has an unusually long, tapered nose, carefully profiled to keep the leading shocks separated during their descent. NASA's target is 75 PLdB at ground level, approximately equivalent to a car door closing across a parking lot, compared to Concorde-era peaks above 105 PLdB. The X-59 flew supersonic for the first time on June 5, 2026. Phase 2 testing, where the aircraft will overfly communities and researchers will measure whether residents even notice it, is scheduled for later this year.

Boom Supersonic's XB-1 demonstrator tried a different approach: Mach cutoff, flying at a precise altitude and speed where atmospheric refraction bends the shock wave back upward before it reaches the ground. On January 28, 2025, the XB-1 completed three supersonic passes without any audible boom registering at the surface. The Supersonic Aviation Modernization Act, introduced in Congress in May 2025, would repeal the overland ban for aircraft meeting a no-audible-boom-at-ground-level standard.

If you understand the Mach cone, you understand why all of this engineering effort is focused on how shocks merge on the way down rather than on reducing how loud the aircraft is overall. The boom is geometry. Change the geometry of the shocks, and you change what the ground hears.

Chuck Yeager broke the sound barrier on October 14, 1947, in a Bell X-1 called Glamorous Glennis, reaching Mach 1.06 over California. The engineers on the ground heard a boom sweep past them. What they were hearing was not a wall coming down. It was a cone passing through.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
