# Intro to PID {#loop-pid-intro status=ready}

<div class='requirements' markdown='1'>

Requires: 
Previous lesson: Intro to the Motors 

Result: 

Students will be able to understand feedback control systems and be ablet o use control system vocabulary terms such as: setpoint, control variable, error. 

</div>

## Lesson Title


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)



### Assessments and Evidence of Understanding


### AGENDA (Brief Summary of Activities)


### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

For Students:

For Teachers: Teachers can look over the EdX lectures that are linked under Userful Links and Resources regarding PID control and implementation. 


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 5 minutes/hours

- Teachers will introduce that today, students will learn about the terms of PID and the concept of feedback loops and their applications. 

- Teachers can bring up that students can control LEDs and can directly control it to get the ideal result. 

- Teachers should explain that they cannot do this for all systems

See also: 1D hovering problem of a drone. Sending one speed to the motors is not enough for the drone to fly it to a desired altitude or hover it at the current altitude because of actuators and world error or noise. 

- Introduce the idea of feedback loops. 


### Main Lesson

Recommended: 40 minutes/hours


- Teachers define open loop vs closed loop systems

See also: Open loop system, also known as a non-feedback system, is a continuous system where output does not affect the control action of the input (Electronics Tutorials). Ex: Toaster

See also: A closed loop system, also known as a feedback system, is a system where the control action is based on the output (Electronics Tutorials). Ex: Body thermoregulation

<!-- https://www.electronics-tutorials.ws/systems/open-loop-system.html --> 


TODO: Exercise: Do this in two stages, "open-loop" and "closed-loop". First, a student looks at a target they’re supposed to go to, gets blindfolded, and tries to walk there. Then the same thing without being blindfolded.

- Teachers draw a block diagram of an closed-loop controller. Show the single input into the controller: the setpoint. Then draw the feedback loop and explain that there are now two inputs to the controller: the setpoint and the error (how far the robot is from the setpoint). 

- Teachers should make it clear that the loop works in iterations, based on the current setpoint and measurements it determines an output, then does the same process over again after some delay.


- Teachers go over important terms and definitions involved with the PID (proportional, integral, derivative) controller. 

See also: **Process Variable**, represented by $y(t)$: The parameter of the system that is being monitored and controlled. 

See also: **Setpoint**, $r(t)$: The desired value of the process variable.

See also: **Control Variable**, $u(t)$: The output of the controller that serves as input to the system in order to minimize error between the setpoint and the process variable. 

See also: **Steady-State Value**: The final value of the process variable as time goes to infinity. 

See also: **Steady-State Error**: The difference between the setpoint and the steady-state value. 

See also: **Rise Time**: The time required for the process variable to rise from 10% to 90% of the steady-state value. 

See also: **Settling Time**: The time required for the process variable to settle within a certain percentage of the steady-state value. 

See also: **Overshoot**: The amount the process variable exceeds the setpoint, and it is expressed as a percentage.


#### Example relating to biological system: 

- Teachers can introduce these terms and the application of feedback systems in the body. An example here is body thermoregulation, but other examples may be used such as reflexes, hormone feedback loops, heart and blood pressure in the body, etc. 

See also: These terms are applicable to a biological system that we rely in. Thermoregulation relies on a negative feedback system. 

See: The process variable: your body temperature.

See: Setpoint: Regular body temperature is 98.6 degrees F(or 37 degrees C). 

See: Control Variable: If you are cold, and you have a lower body temperature than usual, your body will generate more heat to restore back to regular body temperature. If you are warm, and you have a higher body temperature than usual, your body will reduce heat in your body to restore back to regular body temperature. 


- Here the teacher will go over the error of the system: 

See also: The error of the system $e(t)$, is calculated as the difference between setpoint and proces variable. 

$$ e(t) = r(t) - y(t)$$

See also: The controller aims to minimize the rise time and settling time of the system, while eliminating steady-state error and maximizing stability (no unbounded oscillations in the process variable). It does so by changing the control variable $u(t)$ based on three control terms.



### Ending The Lesson

Recommended: 5 minutes/hours

- Teachers will summarize that feedback loops will be used and these terms will be implemented in the next lesson.

**Useful Resources and References**

- Teachers can see EdX lectures on PID Control: https://edge.edx.org/courses/course-v1:BrownX+CS195R+2018_T1/course/#block-v1:BrownX+CS195R+2018_T1+type@chapter+block@0c4aafccbe244af093e640e6e81d9e26