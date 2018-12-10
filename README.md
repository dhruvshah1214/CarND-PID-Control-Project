# CarND-Controls-PID
Self-Driving Car Engineer Nanodegree Program

---

## Reflection

### Describe the effect each of the P, I, D components had in your implementation.

- The proportional portion of the controller uses the cross-track error and multiplies it by a constant to try to steer the car toward the center line. However, with just this, the car overshoots the central line and results in back-and-forth, unstable driving.

- The integral portion tries to eliminate a possible bias on the control system that could prevent the error to be eliminated (usually steering drift).

- The differential portion helps to counteract the proportional tendency to overshoot the center line by smoothing the approach to it.

### Describe how the final hyperparameters were chosen.

I used the Twiddle algorithm (taken out of source code) to tune the hyperparameters to the PID controller.

## Simulation

### The vehicle must successfully drive a lap around the track.

A short video is included in the videos/ folder of this repository.
