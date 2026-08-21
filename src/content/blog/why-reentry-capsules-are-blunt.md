---
title: 'Why Reentry Capsules Are Blunt Instead of Pointed'
description: 'A sharp nose is the worst possible shape for coming home from orbit, and the reason is a shock wave that refuses to touch the vehicle.'
pubDate: 'Aug 21 2026'
---

Every spacecraft that has ever brought people back from orbit came home backwards. Mercury, Gemini, Apollo, Soyuz, Dragon. All of them turn around and fly a wide, rounded face into the atmosphere at thousands of miles per hour. The sleek pointed nose you would sketch if someone asked you to draw something fast is the shape that gets you killed.

I spent a long time assuming this was a packaging decision. You need somewhere to bolt the heat shield, capsules are cone-shaped, so the flat end goes first. That is not it. The bluntness is the heat shield. Change the shape and you change how much heat reaches the structure by a factor of four, before you have picked a single material.

## The heat is not friction

The first thing to unlearn is that reentry heating comes from air rubbing against the skin. Almost none of it does. The vehicle is coming in at something like 7.8 kilometers per second from low orbit, and Apollo came back from the Moon at about 11 km/s, roughly 25,000 mph. Sound in air travels at about 0.34 km/s. The vehicle is outrunning its own pressure signal by a factor of thirty, so the air ahead of it gets no warning that anything is coming.

Air that cannot move out of the way gets crushed instead. That violent compression happens across a shock wave, a paper-thin sheet where pressure, density, and temperature all jump almost instantly. The air behind that sheet reaches several thousand kelvin (kelvin is just degrees Celsius shifted so that zero is absolute zero, so 5,000 K is around 4,700 C). At those temperatures air stops behaving like air. Electrons get knocked loose from the molecules and the gas turns into plasma, which is what blacks out radio contact during entry.

Here is the part that reframes the whole problem. The total energy is not up for negotiation. A capsule in orbit carries a fixed amount of kinetic energy, and it all has to go somewhere before touchdown. You cannot make the number smaller. The only thing you get to design is where it ends up: in the air, or in your spacecraft.

## The shock that refuses to touch

Put a sharp point on the front and the shock wave attaches to the tip. It sits right on the surface, and the superheated gas behind it is in direct contact with your structure. All that compressed, glowing air is now dumping heat straight into the nose, at the exact spot with the least material to absorb it.

Make the front blunt and the shock cannot stay attached. It detaches and stands off ahead of the vehicle as a curved bow shock, with a cushion of gas in the gap between the shock and the surface. The air still gets crushed and still gets thousands of degrees hot, but most of that hot gas slides around the shoulder and trails away behind you instead of soaking into the shield. H. Julian Allen and Alfred Eggers worked this out at NACA Ames in 1952, and their result was the opposite of everything aerodynamics had taught up to that point: the heat a vehicle absorbs goes *down* as its drag goes *up*. Roughly 90 percent of the energy gets dumped into the air rather than the vehicle. The shape that looks worst is the one that works.

There is a clean way to see the size of the effect. The standard engineering estimate for heating at the stagnation point (the spot dead center on the nose where the incoming air is brought completely to rest, and the hottest point on the vehicle) is the Sutton-Graves relation. Heat flux there, meaning power per unit area in watts per square centimeter, scales with velocity cubed and with one over the square root of the nose radius. Velocity cubed is why entry speed dominates everything. The square root is the design lever.

I ran the numbers by hand for two shapes at the same speed and altitude. Apollo's heat shield had a radius of curvature of 4.69 meters. Give a pointed vehicle a nose radius of 0.3 meters, which is still not a needle. The ratio of heat fluxes is the square root of 4.69 divided by 0.3, which is about 4. Same speed, same air, same material. The blunt shape takes a quarter of the peak heat flux. That square root is the entire argument for the shape of every crew capsule ever flown, and I find it slightly absurd that it fits on one line.

Bluntness buys a second thing too. High drag means the vehicle sheds speed high up, where the air is thin and there is less of it to heat. A low-drag body keeps its speed longer and does its decelerating deep in dense air, which is the worst place to be doing it.

## Why it still matters

None of this is settled history. The hard part was never the shape, it was surviving the heat that still gets through, and that is an active materials problem right now. Varda Space Industries brought its W-5 capsule down at Koonibba, South Australia on January 29, 2026. It was the first capsule to come home behind a heat shield built entirely of company-made C-PICA, a NASA ablative material. Ablative means the shield is supposed to burn. It chars and flakes away in a controlled way, and the heat leaves with the material that carries it off. Varda had already flown the stuff on W-4 in June 2025 next to shoulder tiles made by NASA Ames, so both production methods rode the same entry and could be compared afterward. SpaceX is solving the same problem in a much harder configuration. Starship reenters belly-first rather than as a capsule, which is the same trick of presenting the widest possible face, and its heat shield survived its most demanding entry yet on Flight 13 in July 2026 with revised tile attachment pins and adhesive. Tiles falling off has been the recurring failure, not the aerodynamics.

Next time you see a reentry capsule, notice that the wide end is not a compromise around the parachutes or the crew seats. It is the primary thermal protection system, and the actual heat shield material is just insurance for the fraction that gets past it. The blunt shape is doing the heavy lifting, and it works because of a shock wave that stands a few centimeters away and never touches anything.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
