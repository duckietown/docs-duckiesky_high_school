# The Three PID Terms {#loop-pid-terms status=ready}

[Student version](+duckiesky_high_school_student#loop-pid-terms)

<div class='requirements' markdown='1'>

Requires: 

**Hardware** 

- Basestation
- Part 1 of drone

**Previous lesson** - [Intro to PID](#loop-pid-intro)


**Knowledge** - 

- What each term of a PID controller does
- Why each term is important
- Rough mathematical understanding of how each term works

**Skills** - Tuning a PID loop

</div>

## The Three PID Terms


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)
_ISTE: 1. d.:_ Understand the fundamental concepts of technology operations, demonstrate the ability to choose, use and troubleshoot current technologies and are able to transfer their knowledge to explore emerging technologies.


### Assessments and Evidence of Understanding
By the end of this lesson, students will understand the different terms used in PID systems.

### AGENDA (Brief Summary of Activities)
5 min: Introduction to lesson  

40 min: Go over definitions of PID terms and their effects  

5 min: Conclusion

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

**Teacher Materials**
 
- Projector for displaying videos or slides
- Reference the student textbook, EdX and Youtube videos (both linked in the useful resources section below) for more detailed explanations of concept snad examples
 


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

- Hook: They will use the vocabulary and concepts that they learned in the last lesson to be able to understand how PID works, the terms associated with PID, and its effects in the 1D Hovering Drone Problem. 

### Main Lesson

- Show students [video](https://www.youtube.com/watch?v=wkfEZmsQqiA) explaining PID controllers

##### The Proportional Term

Better: Exercise: Students try different extreme values for the P term in the simulation

- Explain the P term and try tuning in simulation. 

- Explain the effects of having a higher or lower proportional gain constant.

- Explain affects of the proportional term regarding the altitude problem.

##### The Derivative Term

Better: Exercise: Students try different extreme values for the D term in the simulation.

- Explain the D term and try tuning in simulation.

- Explain affects of the derivative term regarding the altitude problem and its limitations.

See also: Teachers can show graphs of different levels of damping: over, under, critical. 


##### The Integral Term

Better: Exercise: Students try different extreme values for the I term in the simulation

- Teachers will explain the I term

- Explain affects of the integral term regarding the altitude problem and its limitations.



##### The overall control function

- Explain the overall control function

#### Show diagram of PID controller Block Diagram

The figure below summarizes the inclusion of a PID controller within a basic control loop.

<figure>
    <figcaption>PID Controller Block Diagram</figcaption>
    <img style='width:35em' src="https://docs.duckietown.org/DT19/doc-sky/out/assets/data-from-img-pid_controller_block_diagram-a2353f10.png"/>
</figure>

##### Tuning: 

- Explain why tuning a PID controller is necessary

#### Effects of $K_p$:

- Describe the effects of $K_p$ 

#### Effects of $K_i$

- Describe the effects of $K_i$ 

#### Effects of $K_d$

- Describe the effects of $K_d$ 

### Ending The Lesson

- Explain that while we are looking at the terms from the context of 1D altitute control, they are also used for others such as angle, velocity, position, etc of the drone.

- Summarize the effects and what each term is 
<figure>
    <figcaption>General Effects of Control Terms</figcaption>
    <img style='width:35em' src="https://docs.duckietown.org/DT19/doc-sky/out/assets/data-from-img-control_term_effects_table-e300370c.png"/>
</figure>


**Useful Resources and References**

- Teachers can see [EdX lectures on PID Control](https://edge.edx.org/courses/course-v1:BrownX+CS195R+2018_T1/course/#block-v1:BrownX+CS195R+2018_T1+type@chapter+block@0c4aafccbe244af093e640e6e81d9e26)