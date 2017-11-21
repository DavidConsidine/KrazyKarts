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
