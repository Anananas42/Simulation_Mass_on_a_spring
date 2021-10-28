# Simulation_Mass_on_a_spring (2019)
Analytical and numerical simulation of a mass on a spring with adjustable parameters and nice visualization. Numerical simulation uses highly reliable Runge-Kutta method of 4th degree.

## How to use
Start the Unity application using "Zavazi na pruzine - fyzika.exe"

- The movement of the mass is described by the differential equation above.
- x(t) is the position of the object in terms of time
- m is the mass of the object
- x0 is the initial relative position to rest position
- v0 is the initial velocity relative to the spring
- b is the drag coefficient
- k is the spring's stiffness
- A is the amplitude of a periodic external force
- f is the frequency of a periodic external force
- With analytically solved cases, time can be reversed

- 'RESET' Resets the simulation by setting time to 0s.
- Resonance tick box changes current frequency of the external force to the own frequency of the object on the spring
- 'START' is used to start or stop the simulation.

The simulation must be reset in order to apply given values!

- Simulation uses automatically analytical method when no external force is applied (that is when A=0). Otherwise numerical method is used. The analytical method is incorrect in overdamped case - see Disclaimer. Everything else works correctly.

![screenshot_mass_spring_sim](https://user-images.githubusercontent.com/43809508/139278711-18033059-6ba9-409e-9c20-4a469eca380f.png)

### Disclaimer
The application isn't perfect, it was my second project in highschool, but it can still serve as a very useful experimentation and visualization tool.
* Overdamped analytical solution is incorrect - better to use numerical solving. The application uses analytical solution unless an external force is applied. So you can set the mass to some large value and external force to the smallest and it will be negligible.
