# Lesson 1: Intro to PID {#loop-pid-intro status=ready}

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

Recommended: X minutes/hours

### Main Lesson

Recommended: X minutes/hours

Teachers go over important terms and definitions inovled with the PID (proportional, integral, derivative) controller. 


Process Variable, represented by $y(t)$: The parameter of the system that is being monitored and controlled. 


Setpoint, represented by $r(t)$: The desired value of the process variable.


Control Variable, represented by $u(t)$: The output of the controller that serves as input to the system in order to minimize error between the setpoint and the process variable. 


Steady-State Value: The final value of the process variable as time goes to infinity. 


Steady-State Error: The difference between the setpoint and the steady-state value. 


Rise Time: The time required for the process variable to rise from 10% to 90% of the steady-state value. 


Settling Time: The time required for the process variable to settle within a certain percentage of the steady-state value. 


Overshoot: The amount the process variable exceeds the setpoint, and it is expressed as a percentage.


##### Example relating to biological system: 

These terms are applicable to a biological system that we rely in. Thermoregulation relies on a negative feedback system. 

The process variable: your body temperature.

Setpoint: Regular body temperature is 98.6 degrees F (or 37 degrees C). 

Control Variable: 

If you are cold, and you have a lower body temperature than usual, your body will generate more heat to restore back to regular body temperature. 

If you are warm, and you have a higher body temperature than usual, your body will reduce heat in your body to restore back to regular body temperature. 

### Main Lesson

Recommended: X minutes/hours

Here the teacher will go over the general algorithm: 

The error of the system $e(t)$, is calculated as the difference between setpoint and proces variable. 

$$ e(t) = r(t) - y(t)$$

The controller aims to minimize the rise time and settling time of the system, while eliminating steady-state error and maximizing stability (no unbounded oscillations in the process variable). It does so by changing the control variable $u(t)$ based on three control terms.

Open loop system, also known as a non-feedback system, is a continuous system where output does not affect the control action of the input (Electronics Tutorials). 

A closed loop system, also known as a feedback system, is a system where the control action is based on the output (Electronics Tutorials). 

<!-- https://www.electronics-tutorials.ws/systems/open-loop-system.html --> 

Exercise: Do this in two stages, "open-loop" and "closed-loop". First, a student looks at a target they’re supposed to go to, gets blindfolded, and tries to walk there. Then the same thing without being blindfolded.

### Ending The Lesson

Recommended: X minutes/hours


**Useful Resources and References**
