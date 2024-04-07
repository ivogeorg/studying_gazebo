### studying_gazebo

Exercises with Gazebo worlds, models, etc.

### ROS Services

1. The `/gazebo/pause_physics` and `/gazebo/unpause_physics` can be very useful to simulate the behavior of objects that have to be translated in more than one direction. The translate mode only works one axis at a time, so first translating up the `z` axis and then along the `y` or `x` axis doesn't work, because the object will experience the gravity and fall. To work around this:
   1. Spawn the object.
   2. `rosservice call /gazebo/pause_physics` on the command line.
   3. Translate the object as needed.
   4. `rosservice call /gazebo/upause_physics` on the command line.
   5. To see available services, `rosservice list` on the command line.

### References

1. [Gazebo models (Github)](https://github.com/osrf/gazebo_models).
2. [SDF format](http://sdformat.org/spec?elem=geometry).

