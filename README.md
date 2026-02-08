# Two Body Problem
In this notebook I modeled the two-body problem for the Sun–Earth system using the relative-motion equation and compared two adaptive Runge–Kutta ODE solvers in SciPy: RK45 (Dormand–Prince 5(4)) and DOP853 (Dormand–Prince 8(5,3)). I also documented the physics behind the vector form of Newton’s law of gravitation and the reduction to a single relative-coordinate ODE.

When I increased the simulation time horizon, I noticed small differences in the diagnostic plots (energy and angular momentum conservation). These differences were not due to incorrect physics, but due to numerical behavior of the solvers (accumulated discretization error and solver-dependent drift direction), even though the drift magnitude remained very small.

In the future I’d like to (1) compare solver outputs side-by-side more systematically, (2) try a symplectic integrator for long-term stability, and (3) extend the model to a three-body problem.

The assumptions under this model are:
- only two bodies exist
- Newtonian Gravity is Exact
- Perfect point masses
- isolated system
- no Non-Gravitational forces
- Perfectly known inital conditions

Credit: 
- Wikipeida 
- [Youtube](https://www.google.com/search?q=modeling+the+two+body+problem&rlz=1C1RXQR_enUS1090US1090&oq=modeling+the+two+body+problem&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIHCAEQIRigATIHCAIQIRifBTIHCAMQIRifBTIHCAQQIRifBTIHCAUQIRifBTIHCAYQIRifBTIHCAcQIRifBTIHCAgQIRifBTIHCAkQIRifBdIBCDQwMzFqMGo3qAIIsAIB8QXs-PktfPJhGQ&sourceid=chrome&ie=UTF-8#fpstate=ive&vld=cid:74588417,vid:nJ_f1h49jfM,st:0)
- ChatGPT (coding + explanations)

 
