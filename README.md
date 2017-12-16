# KrazyKarts

### KK01: Creating A Go-Kart Pawn ###

+ Create the project.
+ Create a pawn.
+ Add the mesh.
+ Setup Camera.
+ Attach throttle controls.

### KK02: Understanding Forces and Movement ###

+ Revision of forces in physics.
+ Calculating movement from force.
+ Providing the driving force.

### KK03: Blocking Movement Without Physics ###

+ Setting up the collision volumes.
+ Sweeping with 'AddActorWorldOffset'.
+ Resetting velocity on collision.
+ Refactoring the 'Tick' function.

### KK04: Rotations With Quaternions ###

+ Angle axis rotations with FQuat.
+ adding rotations actors.
+ Rotating our velocity.

### KK05: Simulating Air Resistance ###

+ Understanding air resistance.
+ Getting the "speed".
+ Calculating force due to air resistance.

### KK06: Simulating Rolling Resistance ###

+ What is rolling resistance?
+ Finding the gravity in Unreal.
+ Implementing rolling resistance.

### KK07: Steering And Turning Circles ###

+ Why we get turning circles.
+ Calculating our rotation geometry.

### KK08: Server Functions And Cheat Protection ###

+ How to change state from the client.
+ Introduction to RPC server functions.
+ What is validation?
+ Implementing validation for input.

### KK09: Autonomous Proxy vs SimulatedProxy ###

+ What are Actor roles?
+ Investigating the network roles.
+ Updating the 'AutonomousProxy'.

### KK10: Sources of Simulation Error ###

+ How simulation error effect out game.
+ Overview the different sources of error.
+ Investigate approaches to eliminating them.

### KK11: Replicating Variables From The Server ###

+ Overview of property replication.
+ Replicating the actor position.
+ Setting and reading the property.
+ Replicating the actor rotation.

### KK12: Triggering Code On Replication ###

+ Deep dive on property replication.
+ Setting the network update interval.
+ Notify on replicate.
+ Simulate between updates.

### KK13: Smooth Simulated Proxies ###

+ Replicating velocity.
+ Why is movement jerky?
+ Replicating control input SimulatedProxy.

### KK14: Simulating Lag And Packet Loss ###

+ What is lag?
+ Why does lag cause glitching?

### KK15: Replay Autonomous Moves ###

### KK16: Planning Clinet-Side Prediction ###

+ Pseudocode for client prodiction.
+ Adding structs for synchronisation.

### KK17: Replicating Structs ###

+ What do we have already?
+ Replicating state via a struct.
+ Sending the 'Move' struct via RPC.

### KK18: Simulating A Move ###

+ The 'SimulateMove' signature.
+ Updateing the canonical state.
+ Implement 'SimulateMove'.

### KK19: Unacknowledged Move Queue ###

+ 'TArray' for the Move queue.
+ Tidying the move creation code.
+ Printing the queue length.
+ Removing acknowledged moves.

### KK20: Simulating Unacknowledged Moves ###

+ Simulate all moves.
+ Testing for smoothness.
+ How can we still make it glitch?

### KK21: Fixing SimulatedProxy Prediction ###

+ Ensuring the Server simulates once.
+ Local prediction on the client.
+ Making smoother predictions.

### KK22: Refactoring Into Components ###

+ Red-Green-Refactor process.
+ How to spot your "code smells".
+ Identifying a suitable refactor.
+ Planning our refactor.

### KK23: Extracting A Movement Component ###

+ Create and name the component.
+ Move member declarations across.
+ Move function implementations.
+ Fix build errors.

### KK24: Extracting A Replication Component ###

+ Creating the component.
+ Enable replication.
+ Move member declarations across.
+ Move function implementations.
+ Fix build errors.

### KK25: Decoupling Movement And Replication ###

+ What happens if we disable the replicator?
+ Allow the Movement Component to tick.
+ Getting the information to replicate.

### KK26: Linear Interpolation For Postion ###

+ How does linear interpolation work?
+ Overview of client interpolation.
+ Pseudocode of client interpolation.

### KK27: FMath::Lerp For Client Interpolation ###

+ Ensure movement replication is off.
+ Updating the time variables.
+ 'FMath::Lerp' vs 'FMath::LerpStable'.
+ Implementing the pseudocode.

### KK28: FQuat::Slerp For Rotation ###

+ 'Slerp' vs 'Lerp'.
+ Store transform instead of location.
+ Implemeting 'Slerp'ed location.

### KK29: Hermite Cubic Spline Interpolation ###

+ Understanding jarring movement.
+ How velocity can help or hinder.
+ A brief overrview of polynomials.
+ Introducing the Hermite Cubic Spline.

### KK30: FMath::CubicInterp For Velocity ###

+ Slopes, derivatives and velocity.
+ Using 'CubicInterp' for location.
+ Using 'CubicInterpDerivative' for Velocity.

### KK31: Refactoring With Structs ###

+ Assessing the existing code.
+ Creating a plain C++ struct.
+ Pulling out methods.

### KK32: Client Interpolation Mesh Offset ###

+ Understanding mesh offsetting.
+ Set up the mesh offset root component.
+ Manipulating the offset instead.


### KK33: Advanced Cheat Protection ###

+ Bounding the inputs.
+ Stressing our DeltaTime.
+ Tracking simulation time.
