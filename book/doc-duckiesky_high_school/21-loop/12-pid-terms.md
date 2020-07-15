# Lesson 2: The Three PID Terms {#loop-pid-terms status=ready}

<div class='requirements' markdown='1'>

Requires: 

Result: 

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

Recommended: 10 minutes/hours


### Main Lesson

Recommended: X minutes/hours

Here is a helpful video explaining PID controllers: https://www.youtube.com/watch?v=wkfEZmsQqiA

#### The Proportional Term

The proportional term produces an output that is proportional to the calculated error:

$$ P = K_pe(t)$$

The magnitude of the proportional response is dependent upon $K_p$ which is the proportional gain constant. A higher proportional gain constant indicates a greater change in the controller’s output in response to the system’s error.

The propellers will spin faster the farther away the drone is. 

#### The Derivative Term

The derivative term is determined by the rate of change of the system’s error over time multiplied by the derivative gain constant $K_d$. 

$$D = K_d \frac{de(t)}{dt}$$

#### The Integral Term

The integral term accounts for the accumulated error of the system over time. The output produced is comprised of the sum of the instantaneous error over time multiplied by the integral gain constant $K_i$.

$$I = K_i \int_{0} ^ {t} e (\tau) d \tau$$

#### The overall control function

The overal control function consists as the sum of proportional, integral, and derivative terms. 

$$u(t) = K_pe(t) + K_d \frac{de(t)}{dt} + K_i \int_{0} ^ {t} e (\tau) d \tau$$

#### Show diagram

#### Tuning: 

Tuning a PID controller is done by setting the conotrl parameters $K_p, K_i, K_d$ to values that fit to be able to get an ideal control response. The three control terms may be correlated and so changing one parameter may impact the influence of another. The general effects of each term are therefore useful as reference, but the actual effects will vary depending on the specific control system.

##### Effects of $K_p$:
Increasing $K_p$ will proportionally increase the control output. This causes the system to react more quickly (thereby decreasing the rise time and the settling time by a small amount). Even so, setting the proportional gain too high could cause massive overshoot, which in turn could destabilize the system. Increasing $K_p$ also has the effect of decreasing the steady-state error. However, as the value of the process variable approaches the setpoint and the error decreases, the proportional term will also decrease. As a result, with a P-controller (a controller with only the proportional term), the process variable will asymptotically approach the setpoint, but will never quite reach it. Thus, a P-controller cannot be used to completely eliminate steady-state error.

##### Effects of $K_i$

The integral term takes into account past error, as well as the duration of the error. If error persists for a long time, the integral term will continue to accumulate and will eventually drive the error down. This has the effect of reducing and eliminating steady-state error. However, the build-up of error can cause the value of the process variable to overshoot, which can increase the settling time of the system, though it decreases the rise time.

##### Effects of $K_d$

By calculating the instantaneous rate of change of the system’s error and using this slope for linear extrapolation, the derivative term anticipates future error. While the proportional and integral terms both act to move the process variable to the setpoint, the derivative term seeks to dampen their efforts and decrease the amount the system overshoots in response to a large change in error (which would greatly affect the magnitude of the proportional and integral contributions to the overall control output). If set at an appropriate level, the derivative term reduces oscillations, which decreases the settling time and improves the stability of the system. The derivative term has negligible effects on steady-state error and only decreases the rise time by a minor amount.



### Ending The Lesson

Recommended: X minutes/hours

While we are looking at them from the context in helping control the altitude of the drone in 1D, these terms are also used for angle, velocity, position of the drone. 

**Useful Resources and References**
