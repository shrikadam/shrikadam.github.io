---
layout: post
title: "My Second Post: Hardware Integration"
subtitle: "Wiring the new robotic arm and debugging the servos."
---
It took a few tries, but the new robotic arm is finally wired up and responding to the controller.

Here is a look at the final hardware setup:

![A custom 3D printed robotic arm](/assets/images/posts/my-second-post/robot-arm.jpg)

The next step will be writing the Python script to control the kinematics. Here is a sneak peek:

```python
def move_to_target(x, y, z):
    # Kinematics logic goes here
    pass
```