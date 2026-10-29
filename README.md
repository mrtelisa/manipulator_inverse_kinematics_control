# Manipulator Inverse Kinematics Control

Inverse kinematics control of a 7-DoF industrial manipulator in MATLAB: the tool frame is driven to a goal pose with a Cartesian control loop, and the motion is simulated in 3D.

> Third assignment of the Modelling and Control of Manipulators course (1st year, 1st semester), MSc Robotics Engineering, University of Genoa.

## Content

- **Tool frame:** a tool rigidly attached to the end-effector, and its transformation with respect to the base (`getToolTransformWrtBase`).
- **Cartesian control (`cartesianControl.m`):** orientation (angle-axis) and position error between the tool and the goal frame, turned into a reference velocity with proportional gains.
- **Inverse kinematics:** joint velocities from the Jacobian pseudoinverse.
- **Simulation (`KinematicSimulation.m`):** integration of the joint velocities over time, with joint limits, and a 3D plot of the robot motion.

It builds on the geometric and kinematic models of the [previous assignment](https://github.com/mrtelisa/manipulator_direct_kinematics). `MCM_lab3_24_25.pdf` contains the assignment text.

## Usage

In MATLAB, from the `src/` folder:

```matlab
main
```
