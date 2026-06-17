---
title: 'Why Every Commercial Jet Has Bent Wingtips'
description: 'Winglets add surface area and friction — and still reduce drag overall. The reason is a penalty every wing pays for generating lift in three dimensions.'
pubDate: 'Jun 17 2026'
---

The bent wingtips on virtually every commercial jet aren't aesthetic. They're solving a physics problem baked into how wings work — a penalty every finite wing pays for generating lift. Once you see what's happening at the wingtip, the bent tip stops looking like a design flourish and starts looking like the only reasonable answer.

Most people assume winglets reduce drag the same way a smooth fuselage reduces drag — by streamlining the airflow. The real story is almost the opposite. Winglets add surface area, and surface area creates friction drag. By that measure, they're making things worse. But they eliminate a specific type of drag that costs far more than the friction they introduce. Understanding the tradeoff starts with understanding where that drag comes from.

## The pressure difference that creates the problem

Wings generate lift by creating a pressure difference: high pressure on the lower surface, low pressure on the upper surface. If you imagine an infinite wing stretching in both directions — the 2D case you study first in aerodynamics — that's essentially the complete picture. Pressure differential, lift, done.

Real wings have tips. At the tip, the high-pressure air underneath doesn't stay put. It wraps around the edge into the low-pressure region above, rolling up into a tight corkscrew spiral that trails behind the aircraft. On humid days you can see this as a white tendril curling off the wingtip. Aerodynamicists call it a **wingtip vortex** — a rotating mass of air that every wing with a finite span produces, always, as an unavoidable consequence of generating lift in three dimensions.

## The vortex's hidden cost: induced drag

That vortex doesn't just trail harmlessly behind. It actively pulls the airflow over the wing slightly downward — a phenomenon called **downwash**. And downwash has a direct consequence: it tilts the lift vector backward.

Lift acts perpendicular to the incoming airflow. When downwash tilts that airflow slightly rearward, the lift vector tilts with it. The component of that tilted lift vector pointing in the direction of flight is a drag force. Because it's induced by the process of generating lift, it's called **induced drag**.

In my Aerodynamics course at Rutgers, we derived the equation that quantifies this:

**CDi = CL² / (π · e · AR)**

Unpacked: **CDi** is the induced drag coefficient; **CL** is the lift coefficient (how hard the wing is working to generate lift); **e** is the Oswald efficiency factor (how close the lift distribution is to the theoretical optimum ellipse); and **AR** is the **aspect ratio** — wingspan squared divided by wing area, a measure of how long and narrow the wing is.

Two things jump out. First, induced drag scales with the square of CL — it gets dramatically worse at low speeds and high angles of attack, exactly when you need maximum lift (takeoff and landing). Second, a higher aspect ratio directly reduces induced drag. Longer, narrower wings are always more efficient. Gliders exploit this: a sailplane's aspect ratio can be 40 or higher because there's no gate width to worry about. A 737's is around 10.

The problem is infrastructure. Airport gate widths are fixed. You can't lengthen a 737's wings past a certain point without losing compatibility with existing gates — Boeing already had to work around this for the 737 MAX. So engineers needed a way to capture the efficiency of a longer wing without increasing the physical span.

## What winglets actually do

Winglets don't eliminate the wingtip vortex — nothing can. If you're generating lift on a finite wing, you're generating a vortex. What winglets do is redirect and weaken that vortex, reducing how much downwash it deposits over the wing surface. The aerodynamic effect is equivalent to increasing the wingspan: the **effective aspect ratio** rises, induced drag falls, and the wing performs as if it were physically longer than it is.

The designs have evolved significantly. The original **blended winglet** — the upturned tip that became widespread on the 737 Classic and Next Generation in the 1990s and 2000s — curves smoothly upward, creating a gradual transition that avoids the structural stress of a sharp joint. The **split scimitar winglet**, introduced by Aviation Partners Boeing and first flown by United Airlines in 2014, adds a downward-pointing ventral fin alongside the upward blade. The dual-surface geometry manages the vortex more aggressively on both sides of the wingtip. Airbus took a different approach with the **sharklet** on the A320neo — a taller, more swept design integrated into the wing from the start rather than retrofitted, allowing deeper structural optimization.

Each reflects a slightly different tradeoff: split scimitars add weight at the wingtip (increasing bending load on the wing spar), while sharklets are designed in from scratch, so they integrate more cleanly but require a new wing rather than a retrofit.

## The numbers that make airlines pay for this

The fuel savings are modest in percentage terms and enormous in aggregate. Split scimitar winglets reduce fuel burn by 1.6% on a 1,000 nautical mile sector, rising to 2.2% on a 3,000 nautical mile sector — the longer the flight, the more induced drag accumulates, and the more the winglet recovers. Sharklets on the A320neo deliver up to 4% fuel savings.

For United Airlines, those percentages across a fleet of 737s, 757s, and 767s add up to more than 65 million gallons of fuel saved per year — roughly $200 million annually and 645,000 metric tons of CO₂ avoided. Aviation Partners Boeing has installed winglets on over 10,000 aircraft worldwide.

The underlying physics is nearly a century old. Ludwig Prandtl's lifting-line theory, developed in the 1920s, is what first quantified the relationship between aspect ratio and induced drag, and predicted that an elliptical spanwise lift distribution minimizes it. What changed wasn't the theory — it was the ability to manufacture precisely shaped composite winglet structures light enough that the added friction drag is smaller than the induced drag eliminated.

That equation I derived in aerodynamics class — CDi = CL²/(π·e·AR) — describes exactly why the bent tip is there. The winglet increases the effective AR. The rest follows from the math.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
