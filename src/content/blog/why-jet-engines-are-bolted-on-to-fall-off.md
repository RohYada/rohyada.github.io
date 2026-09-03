---
title: 'Why Jet Engines Are Bolted On to Fall Off'
description: 'The hardware holding a jet engine to the wing is deliberately the weakest link in the chain, and that choice decides whether a bad day ends with a wing or a fire.'
pubDate: 'Sep 03 2026'
---

A large turbofan weighs around 9,000 pounds and pushes about 60,000 pounds of thrust into the wing it hangs from. On a Boeing 747, the hardware that carries all of that is four steel pins, and they are designed to snap.

Most people assume an engine mount is built the way you build anything holding something heavy: as strong as possible, then a little stronger. The engine hangs from a pylon, the aerodynamic post that sticks forward and down from the wing, and the pylon bolts to the wing structure at a small number of fittings. Those fittings are not the strongest part of the assembly. On the 747 they are the weakest, on purpose. Boeing called them fuse pins, and the name is exact. A household fuse is the cheapest thing in the circuit so when something goes wrong, the fuse dies and not your wiring.

The reason sits directly above the engine. That part of the wing is a fuel tank. If an engine is going to leave the airplane, the question is not whether you can stop it. At those loads you cannot. The question is what it takes with it.

## A joint does not have one strength

In Aerospace Structures I spent a homework set on a pin-loaded lug: a flat metal tab with a hole in it and a bolt pulling on it. It is everywhere, including engine pylons.

What surprised me is that you do not calculate its strength. You calculate four, because a lug fails four different ways and they are different events. **Bearing** is the hole getting crushed oval by the pin pressing on it. **Net-section tension** is the material either side of the hole pulling apart, the way paper tears at the punched holes first. **Shear-out** is the pin plowing a channel through the short end of the tab and popping out the edge. And the pin can shear off, cut in two like a bolt in cable cutters.

The load that matters is the lowest of the four. That is the one that happens. And what decides which is lowest is not the material. It is a shape ratio called e/D, the distance from the hole center to the end of the tab divided by the hole diameter. Keep e/D around two and the tab pulls apart in tension near its full material strength. Trim it below about 1.5 and shear-out takes over, and the joint gives up earlier and in a completely different way. Same alloy, same bolt, same load. You moved a hole a quarter inch and changed which failure the part is capable of.

That was the moment the fuse pin idea stopped sounding reckless to me. If failure mode is a design variable, you are choosing one whether you think about it or not. A pylon fitting is that choice made out loud. Engineers set the geometry so that at overload the pin lets go at a known place and a known load, before anything upstream of it in the load path (the chain of parts handing the force along, from engine to pylon to wing spar) can tear. A clean break at the fitting drops the engine. A messy break farther inboard opens the tank.

## What the rule actually asks for

This is not a Boeing preference. It is written into certification. 14 CFR 25.963(d) requires that fuel tanks not rupture when an engine pylon, engine mount, or landing gear tears away. 25.721 asks the same of a pylon dragging on the ground: when it fails from overload, the failure mode must not spill enough fuel to start a fire. Notice what they do not say. They do not say the mount must survive. They say the way it breaks has to be survivable. The rule is written in failure modes because the people who wrote it knew you do not get to pick whether a part fails, only how.

Airbus read the same rules and went the other direction. When they designed their first jetliners in the early 1970s they left fuse pins out and attached the strut to the wing permanently, betting that a mount that never releases beats one that might release when you did not want it to. The FAA approved both. Two of the biggest engineering organizations on earth read the same rules and landed on opposite answers.

Airbus had a point, and El Al 1862 in 1992 is the proof. A 747 freighter lost the No. 3 engine and pylon after takeoff from Amsterdam, and the Dutch investigation traced it to a fatigue crack in a midspar fuse pin. Fatigue is cracking that grows a little with every load cycle, every takeoff and landing, at stresses far below what would break the part in one go. A pin sized to be the weak link is also the part with the least margin left over when a crack starts eating it. The design worked exactly as intended, and it worked on a day nobody wanted it to.

That tension has not gone away. The NTSB is still working the crash of UPS Flight 2976, the MD-11 freighter whose No. 1 engine and pylon came off during rotation at Louisville in November 2025, killing 14 people. Investigators found both lugs of the left pylon's aft mount fractured, with fatigue cracking on multiple surfaces. Progressive damage, not one bad moment. The 2026 hearings put mount design and inspection intervals back at the center of it, thirty-three years after Amsterdam.

The next time you look out at an engine, the interesting hardware is not the engine. It is the handful of fittings at the top of the pylon, sized so the worst day ends with a wing instead of a fire. The catch is that a part built to be the weakest thing in the chain has the least room to hide a crack, so the design rests on finding those cracks before the airplane does.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
