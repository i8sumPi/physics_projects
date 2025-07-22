# Many Mini Physics Projects

Recently I realized that trying out physics projects is a really great and gratifying way to learn programming--and sometimes a lot more simple than it seems! Here are a few of my favorite projects
from recent moments, roughly in chronological order, with potentially more to come (I'll try to keep this website and its links updated). Note: I'll also try to add images and/or video
demos for all the projects soon. 

## Wave Pools

All three of these work using the [wave equation](https://www.feynmanlectures.caltech.edu/I_47.html), which says that the second derivative of the wave height with respect to time is proportional to the second derivative of wave height with respect to position--or, in other words, the acceleration of the wave at a particular point is proportional to the waveform's concavity at that point. In this example, the concavity at a given point is calculated using finite differences, i.e. $(x_{n+1} - x_n) - (x_n - x_{n-1})$, and the program then adjusts the velocity at each point accordingly. One interesting consequence of these programs is they show how this wave equation implies a constant wave speed (in air, this is the speed of sound, and in electromagnetism, this is the speed of light). 

- [Scratch Version](https://scratch.mit.edu/projects/1190895952/)

- [JavaScript Version](https://output.jsbin.com/vopeyir/2)

- [2D Ripple Simulator](https://output.jsbin.com/lahemox)

## Smoke Simulator

This is just a fun project that uses a set of cloned blur images with randomized velocities to generate smoke. Different versions can be made to make this look more like a flame. For a more advanced version of this, future steps could be to replace this simpler simulation with a Navier Stokes equation version. 

- [Using WoofJS (JavaScript Library)](https://woofjs.com/full.html#drawkira) ([source](https://woofjs.com/create.html#drawkira))

## A Few Super Mini Math Projects: 

This Markov Chain generator uses a brute force algorithm where, after any set of two words, the program looks for any other instance of those two words, picks one at random, and then takes the next word after that. Then, the program repeats this process with the new next set of two words. The RSA encryption example just demonstrates how two exponentiations can invert each other if they multiply to something $\equiv 1$ mod the euler totient function ($\phi$) of the original base. The process of calculating these keys was more labor intensive (and on paper), but involved finding the inverses of the base with respect to each factor of $\phi$.  

- [Markov Chain Text Generation](https://trinket.io/library/trinkets/ca8aed434407)
- [RSA Encryption Example](https://trinket.io/library/trinkets/2f7ee49b860c)

## Chain of Springs (Soft Body)

This program is much simpler than it looks, and all it does is apply a force proportional to $(\text{length}-20)$ to each end of each segment shown here. Next steps would be to extend this simulation to a soft body physics simulator using the same algorithm. 

- [Using WoofJS](https://woofjs.com/full.html#soft-body) ([source](https://woofjs.com/create.html#soft-body))

# Additional Resources

Here are a few websites with additional projects I really liked: 
- [The Science Playground](https://thescienceplayground.com/)
