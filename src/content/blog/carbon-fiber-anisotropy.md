---
title: 'Carbon Fiber Is Not Strong in All Directions — And That Is the Whole Point'
description: 'Carbon fiber composites are 14x stiffer along the fiber than across it. In my Aerospace Materials homework at Rutgers, that gap produced a result I did not expect.'
pubDate: 'Jun 15 2026'
---

Carbon fiber is famous for being light and strong. What most people don't realize is that it is strong in one direction and relatively weak in the other — by a factor of 14.

That asymmetry is not a flaw. It is the whole design opportunity.

## Not a Material, a System

When engineers say "carbon fiber," they usually mean a carbon fiber reinforced polymer composite — CFRP. Millions of individual carbon fibers are embedded in a resin matrix and oriented in specific directions. Think of it like rebar in concrete: the fibers carry the load, and the resin holds everything in place and protects it from the environment.

The key word is *oriented*. The fibers run in a specific direction, and that direction determines almost everything about how the material behaves.

Along their length — the fiber direction, which engineers call the 1-direction — the fibers are extraordinarily stiff. Perpendicular to the fibers — the 2-direction — you are mostly loading the soft resin instead. The difference in stiffness between those two directions is what makes carbon fiber composites **anisotropic**: the material responds differently depending on which way you load it.

Steel and aluminum don't work this way. They are isotropic — push them from any direction and the response is the same. Carbon fiber is not. That changes everything about how you design with it.

## A Quick Note on the Units

Before the numbers: two units come up constantly in structural analysis.

**Stress** (measured in MPa — megapascals) is force per unit area. It tells you how hard the material is being pushed or pulled at any given point. One MPa is roughly the pressure of a 100 kg weight balanced on a 1 cm² surface. Aerospace structures routinely operate at hundreds or thousands of MPa.

**Strain** is dimensionless — it is a ratio of how much a material deforms relative to its original length. A strain of 0.01 means the material stretched by 1% of its original size. Small numbers, big consequences.

**Stiffness** (measured in GPa — gigapascals, or billions of pascals) tells you how much stress it takes to produce a given strain. A stiffer material deforms less under the same load. Steel has a stiffness of about 200 GPa. Carbon fiber along the fibers beats that at 145 GPa — at about one-fifth the weight.

## What the Numbers Actually Look Like

In my Aerospace Materials homework at Rutgers, I calculated stresses and strains in an SM Carbon (PAN) fiber composite under a realistic loading condition — 2074 MPa pulling in one direction, 1176 MPa in the other, and 729 MPa of shear (a twisting force acting along the surface).

The material's stiffness properties were E11 = 145 GPa along the fibers and E22 = 10 GPa across them. That 14.5x gap is the entire story.

The result I didn't expect: the peak strain in the 2-direction (across the fibers) came out to 0.2054. The peak strain in the 1-direction (along the fibers) was 0.0158. Same material. Same load. The cross-fiber direction stretched thirteen times more.

Now here is the counterintuitive part. When I looked at the stresses, the gap nearly disappeared. Maximum σ11 (stress along the fibers) was 2481 MPa and maximum σ22 (stress across the fibers) was 2074 MPa — only about 20% apart.

Stress barely changed between the two directions. Strain changed by a factor of 13.

That is what anisotropy actually looks like in numbers. The material distributes internal force similarly in both directions, but it deforms at completely different rates depending on which direction you're loading. That distinction doesn't show up until you run the calculation, and missing it in a design is how structures fail.

![Strains and stresses on SM Carbon vs fiber angle under X-Y loads — showing how ε22 and σ22 diverge sharply from ε11 and σ11 as orientation changes](/images/AMHW1Graph.png)

![Results table: maxima and minima for strains and stresses across all orientations](/images/AMHW1Result.png)

The analysis also found something practical. At a fiber orientation of 29° relative to the applied load, σ11 peaks while cross-fiber stress, cross-fiber strain, and shear stress all hit near-minimums — shear dropped to just 5.5 MPa. That makes 29° a near-optimal fiber angle for this particular loading condition.

Rotate the fibers to the wrong angle and you are channeling the load directly into the weak direction. At the wrong orientation, the same structure under the same load fails — not because the material is weak, but because it was placed wrong.

## Why This Shows Up in Every Modern Aircraft

The F-35 airframe is roughly 35% carbon fiber composite by weight. The Boeing 787 is 50%. In both cases, engineers had to solve exactly this problem: figure out the actual load paths through the structure, then orient the fibers so those loads run in the strong direction.

Modern composite laminates don't use a single fiber angle. They stack multiple plies at different orientations — typically 0°, ±45°, and 90° — so the structure has load-carrying capacity in multiple directions at once. The engineering challenge is choosing the stack sequence that covers all real load cases without adding mass you don't need.

The optimization problem is directional. Every ply angle is a choice about where to put strength. Get it right and you have a structure stronger than steel at a fraction of the weight. Get it wrong and you get a failure mode no one designed for.

## The Actual Advantage

Aluminum is strong everywhere, equally. Carbon fiber lets you put strength exactly where the load is — and skip the directions where it isn't. That is the real reason it replaced aluminum in so many aerospace applications. Not just because it is lighter, but because you can engineer the strength in.

The 14x stiffness ratio is not a limitation. It is the lever.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. [Connect on LinkedIn.](https://www.linkedin.com/in/rohan-yadalla/)*
