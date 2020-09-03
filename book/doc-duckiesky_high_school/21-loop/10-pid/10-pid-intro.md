# Intro to PID {#loop-pid-intro status=ready}

<div class='requirements' markdown='1'>

Requires: 
Previous lesson: Intro to the Motors 

Result: 

Students will be able to understand feedback control systems and be able to use control system vocabulary terms such as: setpoint, control variable, error. 

</div>

## Lesson Title


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)



### Assessments and Evidence of Understanding


### AGENDA (Brief Summary of Activities)
Introduction: 5 min
Main lesson: 40 min
Conclusion: 5 min

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

For Students:

For Teachers: Teachers can look over the EdX lectures that are linked under Useful Links and Resources regarding PID control and implementation. 


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

- Students will learn about the terms of PID and the concept of feedback loops and their applications. 

- Explain that students can control LEDs and can directly control it to get the ideal result. 

Hook: explain that that they cannot do this for all systems such as the 1D hovering problem of a drone. Sending one speed to the motors is not enough for the drone to fly it to a desired altitude or hover it at the current altitude because of actuators and world error or noise. 

- Introduce the idea of feedback loops. 


### Main Lesson

Recommended: 40 minutes/hours


- Teachers define open loop vs closed loop systems

<!-- https://www.electronics-tutorials.ws/systems/open-loop-system.html --> 


Better: Exercise: Do this in two stages, "open-loop" and "closed-loop". First, a student looks at a target they’re supposed to go to, gets blindfolded, and tries to walk there. Then the same thing without being blindfolded.

Better: Exercise: Teachers draw a block diagram of an closed-loop controller. Show the single input into the controller: the setpoint. Then draw the feedback loop and explain that there are now two inputs to the controller: the setpoint and the error (how far the robot is from the setpoint). Let students label or identify each part of the diagram. 

- Teachers should make it clear that the loop works in iterations, based on the current setpoint and measurements it determines an output, then does the same process over again after some delay.

- Explain important terms and definitions involved with the PID (proportional, integral, derivative) controller. 

#### Example relating to biological system: 

Better: Exercise: Students can identify some of their examples of feedback loops. 

- Teachers can give an example here is body thermoregulation, but other examples may be used such as reflexes, hormone feedback loops, heart and blood pressure in the body, etc, and describe what each term represents. 


- Explain what the error of the system is comprised of:  
    $$ e(t) = r(t) - y(t)$$

- Explain the reason for the PID controller: 
    - minimize the rise and settling times, eliminate error, increasing stability by changing the control variable based on three control terms.



### Ending The Lesson

Recommended: 5 minutes/hours

- Teachers will summarize that feedback loops will be used and these terms will be implemented in the next lesson.

**Useful Resources and References**

- Teachers can see [EdX lectures](https://edge.edx.org/courses/course-v1:BrownX+CS195R+2018_T1/course/#block-v1:BrownX+CS195R+2018_T1+type@chapter+block@0c4aafccbe244af093e640e6e81d9e26) on PID Control

Here is a helpful [video](https://www.youtube.com/watch?v=wkfEZmsQqiA) explaining PID controllers