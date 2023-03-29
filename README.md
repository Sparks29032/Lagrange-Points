### What are Lagrange Points
Consider the Sun-Earth system and a small asteroid orbiting with the system. Lagrange points points in the center of mass frame where the centrifugal force of the asteroid balances with the gravitational forces from the Sun and Earth. These five colored points are plotted below on an effective potential plot.

![image](https://user-images.githubusercontent.com/59151395/228440467-eae91677-03a1-447a-b696-ab587a4d1c35.png)

### Simulating Earth-Sun Orbits
To simulate Lagrange points in orbit, we should first simulate the Earth-Sun system. We can do this using a simple Euler-Cromer algorithm. Alongside the orbit of the Earth we have also plotted the how the gravitational potential of the Earth changes as it orbits.

![download](https://user-images.githubusercontent.com/59151395/228442433-ad029dff-eaec-4e8b-9d80-dfb8e77be68c.gif)

It may also be fun to look at how Earth would revolve around the Sun if the eccentricity of orbit was larger...

![download](https://user-images.githubusercontent.com/59151395/228442478-6f97820e-cf30-4ba4-911e-8c943fff340e.gif)

...or if the mass of the sun was closer to that of the Earth. Notice with this orbit that the Sun has noticible and not insignificant motion relative to the center of mass located at the origin.

![download](https://user-images.githubusercontent.com/59151395/228442515-af9defff-3966-4697-9182-422ec8e26309.gif)

### Simulating a Third Body
From here, we can easily add a third body to our simulated orbit of the Earth and Sun...

![download](https://user-images.githubusercontent.com/59151395/228442553-92d5b0e5-126d-4abc-90ae-4075a7147e34.gif)

...and even a fourth body!

![download](https://user-images.githubusercontent.com/59151395/228442587-51bacc66-4fd1-4099-b3e7-0862ab0db846.gif)

### Simulating Lagrange Points
Now, let us compute the five Lagrange points. In a system where the mass of the largest body is 25 times larger than the second-largest body, two of the Lagrange points are stable (in green) and three are unstable (in red). The stable are L4, L5 while the unstable are L1, L2, L3.

![download](https://user-images.githubusercontent.com/59151395/228442611-d5369430-7357-4166-b11c-cf414e8aa6f3.gif)

When the mass of the largest body is less than 24.96 larger than the second largest (in the below example, it is only 2.4 times larger), then all five Lagrange points are unstable, demonstrated below.

![download](https://user-images.githubusercontent.com/59151395/228442645-dd408256-8a7c-4d54-b411-50354d8ad789.gif)

### Future Ideas
* Including the effective potentials on the orbit diagrams
* Using more accurate simulation methods
* Creating a toggle between the center of mass and coordinate systems
