---
title: 'Why Fighter Jets Are Designed to Be Unstable'
description: 'Modern fighters are built to be aerodynamically unstable on purpose — and a computer is the only thing keeping them in the air.'
pubDate: 'Jun 17 2026'
---

An F-16 would not stay in the air for more than a few seconds if you cut power to its flight computer. It isn't a backup-systems problem or a worst-case failure mode. The jet is built that way on purpose. Left to the laws of aerodynamics alone, it doesn't want to fly straight — it wants to tumble. The only reason it doesn't is a computer making tiny corrections thousands of times a second, faster than any human could.

That sounds like a flaw. It's actually the whole point.

## What "stable" actually means for an aircraft

Most people picture a stable airplane as one that flies smoothly. The engineering meaning is narrower and more useful: a stable aircraft is one that returns to level flight on its own after a bump. Hit some turbulence, the nose drops, and a stable plane naturally pulls itself back to where it was without the pilot doing anything. A passenger jet is designed to do exactly this. You want a 737 that shrugs off a gust and settles down.

The amount of "want to return" is measured by something called the **static margin** — the distance between the aircraft's center of gravity (the point it balances around) and its **neutral point** (the spot where aerodynamic forces produce no tendency to pitch up or down). When the center of gravity sits ahead of the neutral point, the static margin is positive, and the plane is stable: it self-corrects. When the center of gravity sits behind the neutral point, the static margin goes negative, and the plane is unstable: a small disturbance grows instead of fading. The nose that drops keeps dropping.

For most of aviation history, negative static margin meant a crash. Modern fighters chase it on purpose.

## The real mechanism: trading stability for agility

Here's the trade buried in that sign. Stability and maneuverability pull in opposite directions. The same nose-forward balance that makes a plane self-correct also makes it sluggish — it resists changing direction, because resisting change is exactly what "stable" means. A jet that desperately wants to fly straight is a jet that fights the pilot every time he wants to turn hard.

So fighter designers do something that sounds reckless. They move the balance point backward, past the neutral point, into negative static margin — what the field politely calls **relaxed static stability**. NASA's research notes that fighters can run static margins as negative as -20 percent. Now the airframe doesn't resist maneuvers. It practically falls into them. Point the nose and it goes, because it was already halfway to departing anyway. That instability is free maneuverability, sitting there for the taking.

The catch is obvious: an aircraft that falls into turns also falls into tumbles. You can't hand that to a human pilot. Our reaction time is something like a quarter of a second — far too slow to catch a divergence that doubles in a fraction of that. This is where **fly-by-wire** comes in: instead of the stick connecting to the control surfaces through cables and pushrods, it feeds a computer, and the computer drives the surfaces. The pilot asks for a maneuver; the flight control system figures out the dozens of tiny surface deflections per second needed to deliver it without letting the unstable airframe run away.

I came at this from the math before I ever thought about the hardware. In my Flight Dynamics course at Rutgers, we worked through **stability derivatives** — coefficients that quantify how strongly an aircraft responds to a disturbance, how hard it tries to come back to level. You assemble them and out pops the static margin. For every textbook airplane, that number is positive. Then we looked at the case where it goes negative, and I remember staring at the sign flip and realizing it wasn't a mistake or a broken design — it was a decision. A whole class of aircraft is engineered to live on the wrong side of that equation, and an entire computer exists to make the wrong side survivable. That's the moment the theory stopped being symbols and turned into an F-16.

## Why a computer can do what a pilot can't

None of this was possible until the control loop got fast and reliable enough to trust with your life. The groundwork is genuinely NASA's. In 1972, a modified F-8 Crusader became the first aircraft flown entirely by a digital computer — pilot Gary Krier took it up on May 25 with no mechanical backup at all, only a triple-redundant electronic system standing by. That program ran 210 flights over 13 years and proved a computer could be the primary, trusted path between stick and surface.

That proof is what unlocked the design freedom. As NASA put it, the need for stability had always "constrained aircraft design," dictating the size and placement of the tail, fuselage, and wings — and every one of those stability features made the plane harder to maneuver. Once a computer could command corrections faster and more often than a pilot, designers could simply delete the stability. The F-16 was an early beneficiary; the same F-8 program even let a YF-16 test pilot evaluate its side-stick controller before his first flight in the real jet.

The redundancy detail matters more than it sounds. If a single computer flies an unstable jet, a single computer failure is fatal — there's no stable airframe to coast on while you reboot. So these systems run multiple independent computers voting on every command, built to keep flying through a failure. The instability that buys the maneuverability is also what makes the computer non-optional.

## Why it matters

This is one of the cleanest examples I've found of engineering turning a liability into a feature. Instability isn't tolerated in a fighter — it's the design goal, deliberately dialed in and then managed by software fast enough to make it safe. The same idea quietly spread to aircraft you've flown on: the Airbus A320 brought digital fly-by-wire to airliners in 1987, the Boeing 777 followed in 1994, and NASA's X-59 supersonic demonstrator runs it today.

What stuck with me is the inversion. The plane fighting to stay level is the easy one to build and the hard one to dogfight in. The plane trying to tumble is the one that wins — as long as something is watching the static margin closely enough to never let it.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
