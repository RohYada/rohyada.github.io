---
title: 'Why Swept Wings Give Jets a Tendency to Fishtail'
description: 'Swept wings make jets inherently prone to a coupled yaw-roll oscillation called Dutch roll. A computer on every modern airliner is continuously suppressing it.'
pubDate: 'Jun 23 2026'
---

In May 2024, a Southwest Airlines 737 MAX flying from Phoenix to Oakland started fishtailing at altitude. The wings rocked left and right while the nose swayed in the opposite direction, and the rudder pedals moved on their own. Passengers probably felt sick. The FAA opened an investigation. What they experienced was Dutch roll, a flight dynamic oscillation that swept-wing aircraft are inherently prone to. A computer normally suppresses it before anyone on board notices.

Dutch roll is not just rolling. It is a coupled oscillation where yaw (the nose swinging left or right) and roll happen together but slightly out of phase. When the nose swings right, the aircraft also rolls right, but the roll lags behind the yaw. A few seconds later the nose swings left and the aircraft rolls left. The motion looks like a ship corkscrewing through a gentle swell, or, as the name suggests, like a Dutch speed skater swaying side to side on ice.

The coupling between yaw and roll is not a defect. It comes directly from the geometry of swept wings.

## How Swept Wings Set Up the Oscillation

Think about what happens when a swept-wing aircraft yaws a few degrees to the right. The right wing, advancing into the airstream, presents a shallower **sweep angle** (the angle between the wing's leading edge and a line perpendicular to the fuselage) to the oncoming flow. A less-swept wing generates more lift. The left wing, rotating away, faces a steeper sweep angle and generates less. In the span of a few degrees of yaw, the two wings have different lift outputs, and the aircraft rolls right to match the yaw.

This tendency for sideslip (the angle between the aircraft's actual velocity and the direction its nose points) to produce a rolling moment is called the **dihedral effect**. Some dihedral effect is stabilizing. It rolls the aircraft back toward level after a gust. The problem is that swept wings produce an extremely strong dihedral effect, much larger than what you get from the physical upward tilt of the wings.

Here is where the oscillation comes from. The aircraft yaws right. Swept-wing dihedral effect immediately rolls it right. But the roll restoring force is much stronger than the yaw restoring force from the vertical tail. The aircraft rolls back through level and overshoots before the yaw has corrected. Now it is rolling left while still yawing right. That mismatch sets up the next half-cycle. Yaw and roll chase each other, neither one damping the other out fast enough.

In Flight Dynamics at Rutgers, we solve for these modes by building the linearized lateral-directional equations of motion around a trimmed cruise condition. The state vector has sideslip angle, roll rate, yaw rate, and bank angle. You build the 4x4 system matrix from stability derivatives and compute eigenvalues in MATLAB. Dutch roll shows up as a complex conjugate pair. The real part tells you how fast it damps; the imaginary part gives the oscillation frequency. When I ran this for a simplified swept-wing transport in class, the real part came back barely negative. The **damping ratio** (a dimensionless number where 1.0 is critically damped and 0 means it never decays) was around 0.04. I double-checked the matrix. It was not wrong.

A damping ratio of 0.04 means something specific. The oscillation takes about 35 seconds to drop to half its initial amplitude. FAA regulations (FAR 25.181) require transport aircraft to have Dutch roll damping of at least 0.08, with the product of damping ratio and **natural frequency** (in rad/s, the oscillation rate without damping) of at least 0.15. Most unaugmented swept-wing jets fail this. The airframe alone will not keep the oscillation in bounds.

## Why a Computer Has to Fix It

The engineering solution is the **yaw damper**, a feedback control system that reads yaw rate from a rate gyroscope and deflects the rudder to oppose any yaw motion it detects. The yaw damper acts in tens of milliseconds, far faster than a pilot can feel a disturbance and move the controls. In normal cruise, it makes continuous small rudder inputs several times per minute in turbulent air. Passengers never notice. The oscillation is suppressed before it builds to anything.

The 2024 Southwest incident showed what happens when this system fails. Before the flight, maintenance crews reset the stall management yaw damper computer codes to address a logged discrepancy. Anomalous rudder behavior started on the very first subsequent flight. When Dutch roll set in during light turbulence, the yaw damper was not suppressing it. The oscillations were visible and uncomfortable. Post-flight inspection found structural damage to the vertical stabilizer's trailing edge ribs, the internal structure that supports the rudder attachments.

Dutch roll is usually treated as a comfort problem. An uncommanded oscillation at altitude is unsettling, but most of the time a pilot counteracts it manually and the aircraft stays intact. The Southwest incident showed something more: an uncontrolled Dutch roll can load the **empennage** (the tail assembly, including the horizontal and vertical stabilizers and all their control surfaces) in ways that cause real structural damage. The oscillation is not just uncomfortable. It is a fatigue and loads problem.

The stakes are high enough that yaw damper certification is currently holding up new aircraft programs. The Boeing 737 MAX 7 and MAX 10 are awaiting FAA approval partly because Boeing requested a time-limited exemption for its **stall management yaw damper** (SMYD), a combined system handling both Dutch roll suppression and stall warning, to reach a higher software design assurance level. The SMYD is not a comfort feature. It is one of the last certification items standing between those aircraft and revenue service.

Swept-wing efficiency and Dutch roll tendency have been inseparable since the first swept-wing jet transports in the 1950s. A design choice made to reduce cruise drag requires a control system to remain safe at all airspeeds. Every modern airliner carries a yaw damper because of it. When that system is working, you feel nothing. That nothing is doing a lot of work.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
