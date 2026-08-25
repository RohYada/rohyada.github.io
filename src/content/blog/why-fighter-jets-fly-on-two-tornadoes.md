---
title: 'Why Fighter Jets Fly on Two Tornadoes'
description: 'On most wings, air separating from the surface means you are about to stall. On a delta wing, it is the whole design. Here is how deliberately broken airflow produces a third of the lift.'
pubDate: 'Aug 25 2026'
---

On a normal wing, separated airflow is the thing you spend your entire career trying to prevent. On a delta wing, it is the point. Fighter jets fly around with two tornadoes pinned to the top of the wing, on purpose, and past about 25 degrees of nose-up those vortices are doing roughly a third of the lifting.

Almost every explanation of lift assumes the air stays glued to the wing. It curves over the top, it stays attached, and when it stops you stall. That story works for a long skinny wing, which is what airliners have. It falls apart for the short, sharply swept triangles bolted to fighters and to Concorde.

The number that separates the two families is aspect ratio, which is span squared divided by wing area. It is just a measure of how long and skinny a wing is. A 737 wing is around 9. Concorde's was about 1.7. Classical wing theory says a wing that stubby should be a terrible lifter that quits early. Yet Concorde came over the fence with its nose 14 degrees up, and delta fighters routinely pull past 30 degrees of angle of attack (the angle between the wing and the oncoming air) without drama. The lift is not coming from the air that stayed attached. It is coming from the air that got away.

## Two cones of spinning air, anchored to the wing

Start at the leading edge. Higher pressure underneath, lower on top, so air tries to sneak around the front edge from below. On a fat rounded airliner edge it makes that turn cleanly. On a delta the edge is sharp and swept way back, and the air cannot make the corner. It separates right there, at almost any angle of attack above zero.

Here is the part that makes deltas work. Because the edge is swept, the flow coming off it runs sideways, out toward the tip. That sideways march rolls the separated sheet into a tight spiral instead of letting it flap around and die. You get a cone of spinning air that starts as a pencil point at the apex and fattens as it runs back, sitting right on the upper surface. One per side.

A vortex is fast-spinning air, and fast-spinning air has low pressure at its core, same reason the center of a tornado is a pressure low. So the wing now has two low-pressure tubes clamped to its upper surface. Low pressure on top is lift, and unlike a stall bubble these things are stable. Crank the nose up and they do not collapse, they get stronger. That is the trick: the delta gave up on keeping the flow attached and built a structure out of the separation.

Edward Polhamus at NASA Langley worked out how to compute this in 1966, and his reasoning is one of the cleaner arguments I have run into. On a rounded leading edge with attached flow, the air whipping around the front produces a suction force that points forward, acting like a small thrust. Sharpen the edge and you lose it. Polhamus argued the force does not vanish, it rotates: same magnitude, now perpendicular to the wing instead of forward. Extra lift, from the flow's failure to attach. The result is two terms:

**C_L = K_p · sin(α) · cos²(α) + K_v · sin²(α) · cos(α)**

C_L is the lift coefficient (lift divided out by air density, speed, and wing area, so wings of different sizes compare directly). First term: ordinary attached-flow lift. Second term: the vortices. K_p and K_v depend on the wing's shape.

I plotted this in MATLAB during Aerodynamics for a slender delta of aspect ratio 2, using K_p = πAR/2 = 3.14 per radian and K_v around 3.2. At 25 degrees the vortex term was about a third of total lift. By 35 degrees it was over 40 percent, and the curve was still climbing. The week before I had plotted a lifting-line curve for a conventional finite wing, and that one rolled over and broke around 15 degrees. Seeing both on the same axes changed how I think about separation. It stopped being a failure mode and became something you design around.

## Where it stops working, and why that is the real engineering problem

Vortices do eventually quit, and the way they quit is nastier than a normal stall. Past some angle the tight core abruptly swells and goes turbulent, a transition called vortex breakdown. The breakdown point starts near the trailing edge and marches forward as you keep pulling. Lift falls off, but the bigger problem is that what used to be a smooth spinning tube is now a firehose of turbulent air aimed straight at whatever is behind the wing. The F/A-18 learned this expensively: vortices shed off its leading-edge extensions battered the vertical tails hard enough to cause fatigue cracking, and the fix was a wedge-shaped fence on top of each extension to steer the vortices clear.

That constraint is live. The Boeing F-47, in development with first flight targeted for 2028, is a tailless modified delta, and so is China's J-36. Deleting the vertical tails buys a smaller radar signature, but it also deletes the surfaces that normally keep an aircraft pointed straight. What is left at high angle of attack is largely the vortex system itself, which means where those vortices form, how strong they are, and exactly when they break down are no longer side effects. They are the flight control system. The physics NASA characterized on the F-106B and the F-16XL in the 1960s and 70s is now load-bearing for aircraft that have not flown yet.

So when you see a delta fighter hold a nose-up attitude that looks like it should be falling, the airflow over that wing separated a long time ago. It separated on schedule, at the edge the designers chose, and rolled into something useful. Separated flow is not automatically a stall. Sometimes it is the plan.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
