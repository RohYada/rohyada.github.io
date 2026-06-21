---
title: 'Why Every Modern Jet Engine Has a Giant Fan Out Front'
description: 'The giant fan you see on a commercial jet isn''t just for show. It''s the reason turbofans burn half as much fuel as the engines that came before them. Understanding why comes down to one equation.'
pubDate: 'Jun 21 2026'
---

Look at the engine on any commercial jet and the first thing you notice is the fan. Not the combustion chamber, not the turbine. The massive spinning disk at the front, wider than a person is tall. That fan is doing most of the work, and it's the reason modern jets are twice as fuel-efficient as the engines from the 1950s.

The intuition most people have is wrong. They assume the thrust comes from the hot exhaust blasting out the back. It does, partly. But on a modern turbofan, roughly 80% of the thrust comes from the cold air the fan pushes around the outside of the engine, air that never touches the combustion chamber at all. The hot core is almost a supporting player.

## The Equation That Explains Everything

The physics comes from a principle called Froude momentum theory. Thrust is just mass flow times velocity change: push more air, or push it faster, and you get more thrust. Simple enough. But fuel efficiency is where it gets interesting.

Propulsive efficiency (call it η) measures how much of the engine's power actually moves the aircraft forward versus how much gets wasted as heat in the exhaust. The formula is:

**η = 2 / (1 + Ve/V0)**

Ve is the exhaust velocity, V0 is the aircraft's speed. The closer those two numbers are, the more efficient the engine.

In propulsion class we plugged in real numbers. At cruise, a commercial jet flies at roughly 250 meters per second. A turbojet (the kind that powered early jets) exhausts at around 900 m/s. Plug that in: η = 2 / (1 + 900/250) = 43%. Less than half the engine's shaft power is actually moving the plane. The rest leaves with the exhaust and warms the atmosphere.

Now take a modern turbofan. It splits that same shaft power differently: a big fan pushes a huge volume of air backward at around 350 m/s. η = 2 / (1 + 350/250) = 83%. Same fuel burned, almost double the useful thrust.

That's not incremental improvement. It's a different approach to the same problem, and it took engineers a few decades to fully commit to it.

The ratio of bypass air to core air is called, logically, the bypass ratio. Early turbofans in the 1960s had bypass ratios around 1.4, barely more air going around the core than through it. The Rolls-Royce RB211 and Pratt & Whitney JT9D, which powered the original 747, pushed that to 4 or 5 in the 1970s and cut fuel burn significantly. The CFM56, the engine that powered 737s and A320s for 30 years, landed around 5 or 6. The LEAP engines on the A320neo hit 11. The GE9X on the 777X has a 134-inch fan, nearly as wide as a 737 fuselage, and runs at bypass ratio 10.

Each jump in bypass ratio was a jump in fuel efficiency. The overall improvement from pure turbojet to a modern high-bypass turbofan is about 50% less fuel burned per unit of thrust. The bypass air also wraps around the hot core exhaust, which reduces jet noise — so airports got quieter as a side effect of the same design trend. That's the single biggest efficiency gain in commercial aviation history, and it came from rethinking where the thrust actually comes from.

## Why There's a Ceiling, and What CFM Is Doing About It

Keep raising the bypass ratio and at some point you hit a wall. The fan needs a nacelle (the cowling around it that shapes the airflow and keeps the bypass air organized). Make the fan bigger and the nacelle gets bigger. At some point the nacelle itself creates so much drag that you're giving back the efficiency gains you just earned. Ground clearance makes it worse. The 737 MAX's engines have a smaller fan than the A320neo's not because of aerodynamics, but because Boeing's lower ground clearance couldn't fit a wider nacelle under the wing. That constraint cost them bypass ratio points and required landing gear redesign. The theoretical ceiling for a ducted turbofan is somewhere around 12:1 to 15:1.

CFM, the joint venture between GE Aerospace and Safran, decided to cut the nacelle out entirely. Their RISE program (Revolutionary Innovation for Sustainable Engines) is an open-fan design: exposed counter-rotating fan blades, no duct, no cowling. Without a nacelle, the bypass ratio equivalent climbs above 70:1. Component tests completed in 2023 already exceeded their 20% fuel savings target compared to the LEAP. An Airbus A380 is the designated flight testbed.

There's a reason open-fan designs were tried and abandoned in the 1980s: they're loud. The exposed blades generate noise at the blade-passing frequency, a high-pitched tone that travels straight into the cabin with nothing to absorb it. Early open-rotor prototypes were effective but miserable to sit near. CFM is betting that 40 years of advances in blade geometry, composite materials, and acoustic modeling can solve the noise problem that killed the concept last time. The fuel math is too good to walk away from.

Once you understand bypass ratio, every commercial jet engine looks different. The big fan isn't cosmetic. It's the whole point. The combustion happening in the core is really just there to spin that fan. CFM RISE is the argument that the nacelle was always the constraint, and that removing it is the next logical step.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
