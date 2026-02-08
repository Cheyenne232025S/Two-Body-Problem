# Two Body Problem
In this notebook I attempted to model a two body problem between the Sun and Earth. It tried this first with a 5th order Runge-Kutta method (Dorman-Prince 5) and an 8th order Runge-Kutta method. Additionally I took time to document and understand most of the physics behind this problem. I found disrepencies in some of the plots outputted depending on how many years I was modeling for and what power ODE I was using. This revealed to me that it was not incorrect physics rather small compuational instabilities such as sign flips when moving between methods and very small computational errors. Some day I would like to do this with a 3 body problem. 

The assumptions under this model are:
- only two bodies exist
- Newtonian Gravity is Exact
- Perfect point masses
- isolated system
- no Non-Gravitational forces
- Perfectly known inital conditions

Credit: 
Wikipeida 
[Youtube](https://www.google.com/search?q=modeling+the+two+body+problem&rlz=1C1RXQR_enUS1090US1090&oq=modeling+the+two+body+problem&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIHCAEQIRigATIHCAIQIRifBTIHCAMQIRifBTIHCAQQIRifBTIHCAUQIRifBTIHCAYQIRifBTIHCAcQIRifBTIHCAgQIRifBTIHCAkQIRifBdIBCDQwMzFqMGo3qAIIsAIB8QXs-PktfPJhGQ&sourceid=chrome&ie=UTF-8#fpstate=ive&vld=cid:74588417,vid:nJ_f1h49jfM,st:0)
ChatGPT (coding and mentor to understand the physics)

This was a weekend project, and I would like to move onto other projects, however with more time I would like to compare different solver method's output side by side and make the model closer to reality. 
