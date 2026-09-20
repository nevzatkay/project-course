My interpretation of the brief

My interpretation of this project is to design and implement a small custom 2D physics engine that can simulate rigid bodies and handle their interactions through collision detection and collision response.

The main goal, in my understanding, is not to create a full commercial-level physics engine, but to understand how the different parts of a physics simulation work together. This includes updating the physical state of objects, detecting collisions, generating contacts and calculating appropriate responses.

I am particularly interested in the numerical side of the project. Different integration methods, time steps and collision response approaches can produce noticeably different results, so I think measuring these differences would be an important part of the project rather than only making the simulation visually work.

Why I am a good fit for this project

This project is relevant to me because I am interested in software development, game development and understanding how systems work at a lower level.

I would like to work on a project where the result is not only an application, but also something where I can investigate the algorithms behind it. Physics engines are especially interesting to me because relatively small mathematical or implementation decisions can have a significant effect on stability and performance.

I also like the experimental aspect of the project. Being able to create controlled scenarios, change parameters such as the time step or number of bodies and then compare the results would make it possible to understand the strengths and limitations of the implemented methods.

Relevant experience and background

I have worked with Java, C#, Python, C, web programming, databases, software design and computer networks. My experience with C and C# would be particularly relevant to implementing the core parts of the physics engine and handling the simulation loop.

I have also worked on software projects where I had to structure a system into separate components. In my ColonyWatch project, for example, I developed a modular Java/SpringBoot backend with persistence, services, controllers and automated tests using Maven and JUnit.

Although this was not a physics project, the experience of breaking a larger system into independent components and testing individual parts would be useful when implementing and validating the different stages of the physics pipeline.

Proposed approach

I would first define the scope of the physics engine and select a manageable set of geometric primitives, most likely circles and axis-aligned boxes or convex polygons.

The first stage would be implementing the simulation loop and rigid-body state update. I would then separate collision detection into broad-phase and narrow-phase stages so that potential collisions can be filtered before performing more detailed geometric tests.

For the broad phase, I would investigate a simple spatial or bounding-volume based approach. The narrow phase would then perform the actual collision tests for the supported shapes and generate the required contact information.

After that, I would implement collision response and investigate parameters such as restitution and friction. If the selected scope allows it, I would also include rotational motion and examine how it affects the simulation.

I would create controlled test scenes for validating the engine. These could include objects falling under gravity, objects colliding with static surfaces, multiple-body collisions and different arrangements with varying collision densities.

The same scenarios would then be tested with different simulation time steps and numbers of bodies. I would measure things such as penetration error, computational time and, where appropriate, changes in energy or momentum.

Finally, I would analyse the results and document where the chosen numerical and collision methods work reliably and where they begin to produce unstable or inaccurate behaviour.

Initial plan

* Define the supported body types, physical properties and simulation assumptions.
* Design the rigid-body data structures and simulation loop.
* Implement state integration and configurable simulation time steps.
* Implement broad-phase collision detection.
* Implement narrow-phase collision tests for the selected geometric shapes.
* Implement contact generation and collision response.
* Add physical properties such as restitution and, if included in the selected scope, friction and rotation.
* Create controlled test scenes for validating individual parts of the engine.
* Measure numerical stability under different time steps.
* Investigate penetration and collision-response errors.
* Measure energy or momentum behaviour where appropriate.
* Test the performance of the engine with different numbers of bodies and collision densities.
* Compare the computational cost of different implementation approaches where applicable.
* Document inaccurate or unstable cases and analyse their causes.
* Keep the implementation and all test scenarios version-controlled and reproducible.
* If the results are suitable, prepare the work for TDK.

Additional information

I plan to maintain the project in a Git repository from the beginning and use issues to organise the implementation, experiments and testing tasks.

For visualization and interaction, I would use a suitable game or graphics framework, while keeping the actual physics calculations independent from any built-in physics subsystem.

I would also keep the experimental scenarios reproducible so that the same parameters can be used when comparing different integration, collision detection or response approaches.

My main goal would be to build a compact but complete physics pipeline and use controlled experiments to understand the relationship between numerical methods, simulation stability, collision accuracy and computational performance.
