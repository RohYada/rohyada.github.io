---
title: 'Why Aircraft Skin Is Designed to Wrinkle'
description: 'Run the buckling numbers on a jet fuselage panel and it should give up at a tenth of the load it actually carries. It does buckle. Then it keeps working, and the wrinkles are the reason.'
pubDate: 'Aug 26 2026'
---

Catch the rear fuselage of a 757 in low sun and you can see the skin wrinkle between the rivet lines, like a bedsheet pulled diagonally. Nothing is wrong with that airplane. The wrinkles are the structure doing its job.

Almost everyone learns buckling as the end of the story. Push on a slender column, it holds, it holds, and then at some critical load it bows sideways and you are done. That model is right for a column. It is wrong for the thin sheet metal that covers an airplane, and the difference is worth real weight.

A wing spar is the beam running out along the span, and it looks like a capital I lying on its side: thick flanges top and bottom, a thin vertical sheet joining them called the web. The flanges take the bending. The web takes shear, which is the sliding force that tries to slice the beam along its depth, like pushing the top of a deck of cards sideways while the bottom stays put. Fuselage skin does the same job in a different shape, and both are backed by stiffeners: stringers running lengthwise, frames or ribs running crosswise, dividing the sheet into rectangular panels a few inches across.

## The panel quits, and a truss shows up in its place

Here is the number that stopped me. In Aerospace Structures I ran the classic flat-plate buckling equation on a normal panel: 0.040 inch aluminum, about a millimeter thick, sides roughly 150 mm apart, simply supported, loaded in shear.

**τ_cr = k · π²E / [12(1 − ν²)] · (t/b)²**

τ_cr is the critical shear stress, meaning the shear force per unit area at which the panel first buckles, measured in MPa (megapascals, one newton of force spread over one square millimeter). E is the stiffness of aluminum, ν is Poisson's ratio (how much metal squeezes sideways when you stretch it), t is thickness, b is the short side, and k is a coefficient set by the panel's shape and edge supports, about 5.35 here.

That comes out around 16 MPa. Aluminum sheet like 2024-T3 does not give up in shear until roughly ten times that. So my first read was that the panel was undersized. It is not. What I had computed was the stress at which the panel wrinkles, which has almost nothing to do with the stress at which it fails.

What happens past 16 MPa is the interesting part. The panel cannot carry any more compression along the diagonal that is being squeezed, so it folds out of the way along that diagonal and stops resisting compression entirely. But the other diagonal, the one being stretched, does not care that the sheet is wavy. Fabric works fine in tension even when it is crumpled. So the buckled panel reorganizes itself into a bundle of narrow tension straps running corner to corner, and it pulls inward on everything around it. The stringers on either side get squeezed and act as compression posts. The flanges take the leftover. The panel that just failed as a plate is now a truss, and a truss made of tension diagonals and compression posts is a perfectly good way to carry shear.

Herbert Wagner worked this out in 1929, against a standard practice that said a shear web was finished the moment it buckled. Wagner said it only changes what kind of structure it is, then carries many times the load that first wrinkled it. Paul Kuhn and James Peterson at NACA Langley spent the next two decades turning that into something you could actually design with, testing around fifty beams to failure and publishing the results in 1952 as NACA TN 2661. That report is still the backbone of how post-buckled fuselage panels get sized today. Seventy-four years old, and I was reading it for a homework problem.

## The bill for it, and why composites reopened the argument

Nothing here is free. Once the panel folds, the diagonal tension yanks inward on the stiffeners and rivet lines, so the stiffeners have to be beefier than a non-buckling design would need, and the fasteners see a steady pull rather than a clean shear. That is a fatigue problem, since fatigue is damage that accumulates from load cycles even when no single cycle is anywhere near strong enough to break anything. Designers handle it by choosing where buckling is allowed. Fuselage side and belly skin, yes. Wing upper surface in cruise, no, because a wrinkled wing costs drag. On the B-52 the wrinkles became permanent, which is why those bombers look the way they do, and the fleet is still flying at seventy.

Composites made this a live fight again. Carbon fiber does not shrug off repeated wrinkling the way aluminum does; the folding works the resin between plies, and delamination is not a thing you want to discover at ultimate load. So the safe move has been to forbid buckling below limit load, which throws away exactly the reserve Wagner found. Published tests on post-buckled composite wing panels put the cost of that caution at about 9 percent of panel mass, and 4 to 13 percent of an entire wing cover depending on aircraft size. Clean Aviation's Multifunctional Fuselage Demonstrator, an 8 meter thermoplastic barrel finished in late 2024, beat its weight target at cost parity with metal, and thermoplastic matrices are tougher against exactly this kind of damage. How much buckling to permit in a composite skin is not settled physics. It is an open certification question with tonnes riding on it.

So the wrinkles in that 757's skin are not wear, and they are not the airplane straining. They are panels that gave up their easy job and took a harder one, which is what the drawings asked them to do. Buckling is a change of behavior, not the end of one, and knowing the difference is worth several percent of the airframe.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
