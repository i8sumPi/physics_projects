# Many Coding Project Recommendations

Recently I realized that trying out physics and math projects is a really great and gratifying way to learn programming--and sometimes a lot more simple than it seems! Here are a few of my favorite projectsfrom recent moments, roughly in chronological order, with potentially more to come (I'll try to keep this website and its links updated). Note: I might also try to add images and/or video
demos for all the projects at some point. 

## Wave Pools

All three of these work using the [wave equation](https://www.feynmanlectures.caltech.edu/I_47.html), which says that the second derivative of the wave height with respect to time is proportional to the second derivative of wave height with respect to position--or, in other words, the acceleration of the wave at a particular point is proportional to the waveform's concavity at that point. In this example, the concavity at a given point is calculated using finite differences, i.e. $(x_{n+1} - x_n) - (x_n - x_{n-1})$. Then, the program then adjusts the velocity at each point accordingly. 

One interesting these programs show is that the wave equation implies a constant wave speed (in air, this is the speed of sound, and in electromagnetism, this is the speed of light). 

- [Scratch Version](https://scratch.mit.edu/projects/1190895952/)

- [JavaScript Version](https://output.jsbin.com/vopeyir/2)

- [2D Ripple Simulator](https://output.jsbin.com/lahemox)

## Smoke Simulator

This is just a fun project that uses a set of cloned blur images with randomized velocities to generate smoke. Different versions can be made to make this look more like a flame. 

- [Using WoofJS (JavaScript Library)](https://woofjs.com/full.html#drawkira) ([source](https://woofjs.com/create.html#drawkira))

## A Few Super Mini Math Projects: 

This Markov Chain generator uses a brute force algorithm where, after any set of two words, the program looks for any other instance of those two words, picks one at random, and then takes the next word after that particular instance. Then, the program repeats this process with the new next set of two words. 

- [Markov Chain Text Generation](https://trinket.io/library/trinkets/ca8aed434407)

The RSA encryption example just demonstrates how two exponentiations can invert each other if they multiply to something $\equiv 1$ mod the Euler totient function ($\phi$) of the original base. The process of calculating these keys was more labor intensive (and on paper), but involved finding the inverses of the base with respect to each factor of $\phi$.

- [RSA Encryption Example](https://trinket.io/library/trinkets/2f7ee49b860c)

The code below shows a basic implementation for importing the Word2Vec library into WoofJS for use in any kinds of games. Note that the cosine similarity can be calculated by dotting two word vectors and then dividing by the product of their magnitudes. More information in the code. [Library used](https://github.com/turbomaze/word2vecjson). 

- [Word2Vec](https://woofjs.com/create.html#word2vec) 

## Chain of Springs (Soft Body)

This program applies force proportional to $(\text{length}-20)$ to each end of each segment shown here, so each segment acts as an ideal Hooke's Law spring. It can make really beautiful results, and show all the wave phenomena discussed above.

Note: A non-linear version of these chains of springs, i.e. where the force is not linearly defined on length, seems to be a topic of [modern research](http://www.scholarpedia.org/article/Fermi-Pasta-Ulam_nonlinear_lattice_oscillations). A fun project could be to simulate a spring with a non-linear force function yourself! 

- [Using WoofJS](https://woofjs.com/full.html#soft-body) ([source](https://woofjs.com/create.html#soft-body))

- [Another version as a piece of fabric](https://woofjs.com/create.html#soft-square)

- [Another version as a square](https://woofjs.com/create.html#soft-body-fabric)

## Satellite Orbits Simulator

This program simulates the orbits of satellites, given the Earth and the Sun as gravitational sources. A few potential observations: (1) The nature is generally chaotic, and orbits with similar starting positions can end up far away from each other, (2) You can sometimes see parabolic orbits around the sun, especially when the Earth is far away, and (3) you can that the oldest orbits sometimes get caught around [Lagrange Points](https://science.nasa.gov/solar-system/resources/faq/what-are-lagrange-points/) ([demo](https://upload.wikimedia.org/wikipedia/commons/d/d0/Lagrangian_points_equipotential.gif)), especially L4 and L5. 

- [Satellite Orbits Simulator](https://woofjs.com/full.html#satellite-simulator)

# Additional Resources

Here are a few websites with additional projects I really liked: 
- [The Science Playground](https://thescienceplayground.com/)
