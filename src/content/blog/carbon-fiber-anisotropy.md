---
title: 'Carbon Fiber Is Not Strong in All Directions — And That Is the Whole Point'
description: 'Carbon fiber composites are 14x stiffer along the fiber than across it. In my Aerospace Materials homework at Rutgers, that gap produced a result I did not expect.'
pubDate: 'Jun 15 2026'
---

Carbon fiber is famous for being light and strong. What most people don't realize is that it is strong in one direction and relatively weak in the other — by a factor of 14.

That asymmetry is not a flaw. It is the whole design opportunity.

## Not a Material, a System

When engineers say "carbon fiber," they usually mean a carbon fiber reinforced polymer composite — CFRP. Millions of individual carbon fibers are embedded in a resin matrix and oriented in specific directions. The fibers carry the load. The resin holds everything together and protects it.

The fibers are what matter here. Along their length (the fiber direction, called the 1-direction), they are extraordinarily stiff. Perpendicular to the fibers (the 2-direction), you are mostly loading the resin — which is far less stiff. This is what makes carbon fiber composites anisotropic: the material behaves differently depending on which direction you load it.

Steel and aluminum are isotropic. Push them from any direction and you get the same response. Carbon fiber composites are not. That changes everything about how you design with them.

## What the Numbers Actually Look Like

In my Aerospace Materials homework at Rutgers, I calculated the stresses and strains in a SM Carbon (PAN) fiber composite under a realistic loading condition — 2074 MPa in one direction, 1176 MPa in the other, with 729 MPa of shear. The material properties were E11 = 145 GPa along the fibers and E22 = 10 GPa across them.

That 14.5x stiffness difference produced a result I didn't expect. The peak strain in the 22 direction came out to 0.2054 — thirteen times higher than the peak strain in the 11 direction at 0.0158. The material was stretching thirteen times more across the fibers than along them, under the same applied load.

But on the stress side, the picture was different. Maximum σ11 was 2481 MPa and maximum σ22 was 2074 MPa — only about 20% apart. Same material, same loading. Strains vary by a factor of 13, stresses by only 1.2. That gap is what anisotropy looks like in numbers, and it is not obvious until you run the calculation.

The analysis also found something practical. At a fiber orientation of 29°, σ11 peaks while the cross-fiber stress and strain both hit their minimums, and shear stress drops to nearly zero — 5.5 MPa. That makes 29° a near-optimal fiber angle for this particular loading condition. Rotate the fibers to the wrong angle and you are running the load straight into the weak direction.

## Why This Shows Up in Every Modern Aircraft

The F-35 airframe is roughly 35% carbon fiber composite by weight. The Boeing 787 is 50%. In both cases, engineers had to solve exactly this problem: figure out what loads the structure will actually see, then orient the fibers to carry those loads in the strong direction.

Modern composite laminates use multiple plies at different angles — 0°, 45°, 90°, and combinations — to distribute load capacity across directions. The optimization problem is choosing the stack sequence that handles all the real load cases without adding weight you don't need.

Get the fiber orientation wrong and the structure fails where you didn't design for it. Get it right and you have a material that is stronger than steel at a fraction of the weight, with the stiffness placed exactly where the loads are.

## The Actual Advantage

Aluminum is strong everywhere equally. Carbon fiber lets you put strength exactly where the load is, and skip the directions where it isn't needed. That is why it replaced aluminum in so many aerospace applications — not just because it is lighter, but because you can design the strength in.

The 14x stiffness ratio is not a limitation. It is the lever.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. [Connect on LinkedIn.](https://www.linkedin.com/in/rohan-yadalla/)*
