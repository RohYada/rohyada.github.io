---
title: 'Why Airliners Keep Fuel in Their Wings, Not the Fuselage'
description: 'Fuel in the wings does more than fill space. It fights the exact force trying to snap the wing off, which is why hydrogen aircraft are struggling to replace it.'
pubDate: 'Jul 14 2026'
---

A fully loaded 777 wing holds around 45,000 gallons of jet fuel. That's not because the fuselage ran out of room. The fuel is up there doing structural work, quietly canceling out one of the biggest loads a wing ever sees.

Most people assume fuel goes in the wings because that's just where the empty space is. The wings are big, hollow, and otherwise unused, so why not. That's true, but it misses the actual engineering reason. Fuel in the wings isn't just stored there. It's positioned there, deliberately, to fight the bending force that lift creates every time the plane flies.

## The wing is a beam, and every beam bends

Picture a wing as a diving board bolted to the fuselage at one end. In flight, lift pushes up along the entire span while the wing's own mass and whatever it's carrying pull down. That combination creates a **bending moment** (a measure of how hard something is trying to bend a structure at a given point, in units like pound-feet or newton-meters), and it's worst right where the wing meets the fuselage. That's the wing root, and it's the point every wing spar has to be built strongest to survive.

In my Aerospace Structures class, we built shear-and-moment diagrams for a wing by hand. Lift gets modeled as a distributed load spread across the span, pushing up. If you stop there, the bending moment at the root is huge. Then you add a second distributed load: the weight of the fuel sitting inside the wingbox, pulling down along that same span. I remember pulling that fuel term out of my diagram just to see what happened to the root moment, and watching it jump. That's the entire argument for wing tanks in one sketch. Fuel isn't dead weight riding along for the trip. It's actively working against the lift trying to bend the spar in half.

This is called **wing bending relief**, and the mechanics are straightforward once you see the diagram. Lift acts as an upward distributed load along the wing's span. Fuselage weight, seats, cargo, passengers, all of that sits near the centerline and effectively hangs off the root like a weight on the end of that diving board, adding to the bending moment. But weight positioned out along the span, like fuel in the wings, acts locally. It's held up by the lift generated right above it instead of transmitting all the way back to the root. The further out along the span you put mass, the more it cancels the bending moment created by lift at that same station. An airplane that carries the same total weight but keeps all of it in the fuselage needs a noticeably beefier wing spar to survive the same flight loads. That's not a small design choice. Spar material is some of the heaviest, most expensive structure on the airframe, and reducing how much of it you need pays off on every single flight for the life of the aircraft, not just once at the factory.

The effect scales with how far out on the wing the mass sits. A gallon of fuel stored near the wing root barely helps, because it's close to the point the moment is measured at anyway. The same gallon out near mid-span or the outboard tanks cancels a lot more bending moment, because it's fighting lift generated far from the root, right where the leverage is largest. That's part of why wings taper and carry tanks running most of their length instead of one lump tank near the fuselage. Spreading the mass out is the whole point.

Engineers manage the fuel burn sequence around this too. Airlines don't drain wing tanks first. Center tank and fuselage fuel typically gets used before the outboard wing tanks, specifically so the wings keep providing bending relief for as much of the flight as possible, especially during the heaviest part of the trip right after takeoff when the wing is working hardest and the aircraft is at its heaviest overall weight.

## Why hydrogen aircraft can't just copy this

This is where the current push toward hydrogen-powered flight runs into a real structural problem. Liquid hydrogen carries more energy per pound than jet fuel, but it needs about four times the volume for the same energy, and it has to be stored at -253°C (close to absolute zero) in pressurized, insulated, cylindrical tanks. A thin wing simply doesn't have the internal geometry to hold tanks shaped like that.

Airbus's response, under its ZEROe program, has been to move toward a blended wing body design, where the fuselage and wings merge into one continuous lifting shape with enough internal volume to fit large cryogenic tanks. That solves the space problem, but it pulls the fuel mass back in toward the centerline instead of spreading it along the span. The wing bending relief that conventional aircraft get essentially for free has to be earned back some other way, whether through a different structural layout, added spar material, or the blended body's own aerodynamic shape doing double duty as a structural member. Airbus has a cryogenic tank prototype targeted for flight testing in 2026, with a version meant for an A380 demonstrator by 2027 or 2028, and a lot of that timeline is really a structures problem wearing a propulsion costume.

It's a reminder that switching fuels isn't just a matter of swapping what burns in the engine. It rewrites the structural loading of the entire aircraft, and a benefit that conventional jets have enjoyed since the earliest swept-wing airliners has to be re-earned from scratch.

Next time you're on a flight and look out at the wing, that fuel sitting a few feet from you isn't just there for range. It's the reason the spar under your feet doesn't need to be twice as thick.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
