---
title: 'Why a Spinning Object Flips Itself Over in Orbit'
description: 'A rigid body spinning about its middle axis will flip 180 degrees on its own, with nothing pushing on it. The math says it has to.'
pubDate: 'Aug 23 2026'
---

In 1985, a Soviet cosmonaut named Vladimir Dzhanibekov unscrewed a wing nut off a threaded rod on the Salyut 7 station. The nut floated away, spinning. Then it flipped over. Then it flipped back. It kept doing that, on a steady beat, with nothing touching it.

Most people watch that video and assume something is pushing the nut. Air currents, a magnetic field, leftover force from the cosmonaut's thumb. Nothing is acting on it at all. A freely spinning object keeps spinning the same way forever, and this one obeys that rule exactly. Its angular momentum never changes. What changes is which way the object points while that momentum stays fixed.

That difference is the whole story, and it is not a quirk of wing nuts. Every rigid object in the universe does this, if you spin it the right way.

## The middle axis is the one that betrays you

Any solid object has three special axes it can spin around cleanly, called principal axes. Each one has a **moment of inertia**, which is just a measure of how hard it is to get that object spinning about that particular line. Spin a pencil about its long axis and it barely resists you. Spin it end over end and it resists a lot more. Those are two different moments of inertia for the same pencil.

For most real objects, the three numbers are all different. Call them smallest, middle, and largest. Here is the part that surprises people: spinning about the smallest axis is stable, spinning about the largest axis is stable, and spinning about the middle one is not. There is no in-between. The middle axis is unstable, always, for every object where the three numbers differ.

I did not believe this until I ran it. In dynamics I integrated Euler's rigid-body equations in MATLAB, the three coupled equations that tell you how an object's spin rate changes when you leave it alone. I gave my body moments of inertia of 1, 2, and 3 kg·m² (kilogram meters squared, the units of rotational stubbornness) and spun it about one axis with a deliberate 0.01 rad/s error on the other two. Radians per second is just a spin rate, and 0.01 rad/s is about half a degree per second. A rounding error.

Spinning about the 1 axis, the error stayed at 0.01 forever. Small wobble, never grew. Same story about the 3 axis. Then I ran the 2 axis, the middle one, with the identical setup. The error doubled, doubled again, and inside twelve seconds the object had swapped ends. Then it swapped back. Same equations, same tiny nudge, completely different behavior.

I assumed I had a sign error somewhere and spent an hour hunting for it. The bug was in my expectations. When I linearized the equations around each spin state and looked at the eigenvalues (the numbers that tell you whether a small disturbance grows or shrinks), the smallest and largest axes gave me purely imaginary roots, which means the wobble just oscillates and stays bounded. The middle axis gave me a real positive root. A real positive root means exponential growth. The flip is not a glitch in the simulation. It is the only thing the equations allow.

The reason comes down to two things being conserved at once. Angular momentum is fixed in magnitude and direction. Rotational energy is also fixed for a truly rigid body. Draw both as surfaces in the space of possible spin states and you get a sphere and an ellipsoid crossing. Their intersections are the paths the object can follow. Near the smallest and largest axes those paths are tight closed loops, so the object circles near where it started. Near the middle axis the paths are two curves that cross, and an object on one runs its full length before coming back. That long trip is the flip. The nut is not being pushed. It is sliding along the only track available.

## Explorer 1 learned this the expensive way

America's first satellite, launched in February 1958, was a pencil-shaped tube designed to spin about its long axis, the smallest moment of inertia. Textbook stable. Within hours it was tumbling in a flat spin about the axis it was never supposed to use.

The design assumed a rigid body. Explorer 1 had four flexible whip antennas, and flexible things flex, and flexing burns energy as heat. Angular momentum is still conserved because nothing external is pushing, but energy is not. Once you drain energy, the object slides toward the lowest-energy spin state available at that fixed momentum, and that state is always a flat spin about the largest axis. This is the major axis rule: any object that can flex, vibrate, or slosh will eventually end up spinning about its axis of maximum inertia, no matter what you started it doing. JPL replaced the whips with rigid fiberglass slot antennas on later Explorers.

That same rule now governs the mess in orbit. Dead satellites lose energy through fuel slosh, thermal flexing, and eddy currents in Earth's magnetic field, and they drift into tumbles. Observed rotation rates for defunct satellites run into the tens of degrees per second, with some low-orbit debris measured above 70 deg/s. Space robotic arms proposed for debris removal can currently grab a target rotating at roughly 4 to 5 deg/s. Everything above that has to be slowed down first, contact-free, using magnetic or electrostatic drag, before anything touches it. A large chunk of active debris removal is not the capture. It is the detumbling you have to do to earn the capture.

The next time you see a wing nut flipping in a space station video, the interesting question is not what pushed it. Nothing did. The object is following the only path that conserves both its momentum and its energy, and that path happens to send it end over end. Stability in rotation is not about balance or symmetry. It is about which of three numbers you chose to spin around.

---

*Rohan Yadalla is an aerospace engineering student at Rutgers University finishing his final semester in December 2026. He's interning at AlphaWave, a healthcare AI startup, where he's building AI-powered tools for physician practices. He's actively exploring roles at the intersection of aerospace and AI systems. Connect on [LinkedIn](https://www.linkedin.com/in/rohan-yadalla/) or see his work on [GitHub](https://github.com/RohYada).*
