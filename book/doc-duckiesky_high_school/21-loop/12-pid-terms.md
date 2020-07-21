# Lesson 2: The Three PID Terms {#loop-pid-terms status=ready}

<div class='requirements' markdown='1'>

Requires: 
Hardware: basestation, Build Part 1 completed
Previous lessons: Intro to PID

Result: 
Students will understand what each term of a PID controller does, why each term is important, and rough mathematical understanding o how each term works. Students will be able to tun a PID loop. 

</div>

## Lesson Title


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)



### Assessments and Evidence of Understanding


### AGENDA (Brief Summary of Activities)


### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

For Students:

For Teachers:


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 5 minutes/hours

- Teachers will explain that they will use the vocabulary and concepts that they learned in the last lesson to be able to understand how PID works and they will be able to tune a PID loop. 

### Main Lesson

Recommended: 40 minutes/hours

Here is a helpful video explaining PID controllers: https://www.youtube.com/watch?v=wkfEZmsQqiA

##### The Proportional Term

- Teachers will explain the P term and try tuning in simulation. 

See also: The proportional term produces an output that is proportional to the calculated error:

$$ P = K_pe(t)$$

See also: The magnitude of the proportional response is dependent upon $K_p$ which is the proportional gain constant. A higher proportional gain constant indicates a greater change in the controller’s output in response to the system’s error.

See also: The propellers will spin faster the farther away the drone is. Or can also be imagined as a spring pulling harder the further away you are. 

See also: Oscillations, get damped to some extent by drag. 

##### The Derivative Term

- Teachers will explain the D term

See also: The derivative term is determined by the rate of change of the system’s error over time multiplied by the derivative gain constant $K_d$. 

$$D = K_d \frac{de(t)}{dt}$$

See also: Propellors will spin slower the faster you are moving. Can be also like drag pulling harder the faster you are moving.

See also: Teahers should show graphs of different levels of damping: over, under, critical. 

See also: Will not be able to get to setpoint if there are constant effects like gravity. 

##### The Integral Term

- Teachers will explain the I term

See also: The integral term accounts for the accumulated error of the system over time. The output produced is comprised of the sum of the instantaneous error over time multiplied by the integral gain constant $K_i$.

$$I = K_i \int_{0} ^ {t} e (\tau) d \tau$$

See also: Propellers were spin faster the longer you are away from the set point

TODO: Tune PID loop and play with parameters

- Teachers should explain that while we are looking at the terms from the context of 1D altitute control, they are also used for others such as angle, velocity, position, etc of the drone. 

##### The overall control function

The overal control function consists as the sum of proportional, integral, and derivative terms. 

$$u(t) = K_pe(t) + K_d \frac{de(t)}{dt} + K_i \int_{0} ^ {t} e (\tau) d \tau$$

#### Show diagram of PID controller Block Diagram

##### Tuning: 

See also: Tuning a PID controller is done by setting the control parameters $K_p, K_i, K_d$ to values that fit to be able to get an ideal control response. The three control terms may be correlated and so changing one parameter may impact the influence of another. 

#### Effects of $K_p$:

- Teachers will describe the effects of $K_p$ 

See also: Increasing $K_p$ will proportionally increase the control output. This causes the system to react more quickly (thereby decreasing the rise time and the settling time by a small amount). 

See also: Setting the proportional gain too high could cause massive overshoot, which in turn could destabilize the system. 

See also: Increasing $K_p$ also has the effect of decreasing the steady-state error. 

See also: However, as the value of the process variable approaches the setpoint and the error decreases, the proportional term will also decrease. As a result, with a P-controller (a controller with only the proportional term), the process variable will asymptotically approach the setpoint, but will never quite reach it. 

See also: A P-controller cannot be used to completely eliminate steady-state error.

#### Effects of $K_i$

- Teachers will describe the effects of $K_i$ 

See also: The integral term takes into account past error, as well as the duration of the error. If error persists for a long time, the integral term will continue to accumulate and will eventually drive the error down. 

See also: This has the effect of reducing and eliminating steady-state error. 

See also: The build-up of error can cause the value of the process variable to overshoot, which can increase the settling time of the system, though it decreases the rise time.

#### Effects of $K_d$

- Teachers will describe the effects of $K_d$ 

See also: The derivative term anticipates future error. While the proportional and integral terms both act to move the process variable to the setpoint, the derivative term seeks to dampen their efforts and decrease the amount the system overshoots in response to a large change in error (which would greatly affect the magnitude of the proportional and integral contributions to the overall control output). 

See also: If set at an appropriate level, the derivative term reduces oscillations, which decreases the settling time and improves the stability of the system. The derivative term has negligible effects on steady-state error and only decreases the rise time by a minor amount.



### Ending The Lesson

Recommended: 5 minutes/hours

- Teachers should summarize the effects of each term. 

**Useful Resources and References**
