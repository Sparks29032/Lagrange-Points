### What are Lagrange Points
Consider the Sun-Earth system and a small asteroid orbiting with the system. Lagrange points points in the center of mass frame where the centrifugal force of the asteroid balances with the gravitational forces from the Sun and Earth. These five colored points are plotted below on an effective potential plot.

![image](https://user-images.githubusercontent.com/59151395/228440467-eae91677-03a1-447a-b696-ab587a4d1c35.png)

### Simulating Earth-Sun Orbits
To simulate Lagrange points in orbit, we should first simulate the Earth-Sun system. We can do this using a simple Euler-Cromer algorithm. Alongside the orbit of the Earth we have also plotted the how the gravitational potential of the Earth changes as it orbits.

![image](https://user-images.githubusercontent.com/59151395/228440316-794dde28-49e4-4c7c-8f2c-aa9156e20da8.png)

It may also be fun to look at how Earth would revolve around the Sun if the eccentricity of orbit was larger...

![image](https://user-images.githubusercontent.com/59151395/228440333-40a47ed9-0ff4-48a3-8269-b704a8f523d4.png)

...or if the mass of the sun was closer to that of the Earth. Notice with this orbit that the Sun has noticible and not insignificant motion relative to the center of mass located at the origin.

![image](https://user-images.githubusercontent.com/59151395/228440346-3abf5822-3d77-4d6a-be69-9a5ce03f9024.png)

### Simulating a Third Body
From here, we can easily add a third body to our simulated orbit of the Earth and Sun...

![image](https://user-images.githubusercontent.com/59151395/228440396-8e171d84-b372-4cc5-9fa1-1e1ae66f2c40.png)

...and even a fourth body!

![image](https://user-images.githubusercontent.com/59151395/228440414-4d9563ba-0ee9-4e20-b964-8902ac8c6deb.png)

### Simulating Lagrange Points
Now, let us compute the five Lagrange points. In a system where the mass of the largest body is 25 times larger than the second-largest body, two of the Lagrange points are stable (in green) and three are unstable (in red). The stable are L4, L5 while the unstable are L1, L2, L3.

![image](https://user-images.githubusercontent.com/59151395/228440444-2ea5d78e-fdce-4845-8812-ea8c43c3dac7.png)

When the mass of the largest body is less than 24.96 larger than the second largest (in the below example, it is only 2.4 times larger), then all five Lagrange points are unstable, demonstrated below.

![image](https://user-images.githubusercontent.com/59151395/228440453-9979ff37-d13e-4a0a-af4a-03ee9ebcb971.png)

### Future Ideas
* Including the effective potentials on the orbit diagrams
* Using more accurate simulation methods
* Creating a toggle between the center of mass and coordinate systems
