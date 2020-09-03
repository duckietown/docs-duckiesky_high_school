# The Three PID Terms {#loop-pid-terms status=ready}

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
Introduction: 5 min
Main lesson: 40 min
Conclusion: 5 min

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

For Students:

For Teachers: Teachers can look over the EdX lectures that are linked under Userful Links and Resources regarding PID control and implementation. 


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

- Teachers will explain that they will use the vocabulary and concepts that they learned in the last lesson to be able to understand how PID works and they will be able to tune a PID loop. 

### Main Lesson

Recommended: 40 minutes/hours

- Show students [video](https://www.youtube.com/watch?v=wkfEZmsQqiA) explaining PID controllers

##### The Proportional Term

Better: Exercise: Students try different extreme values for the P term in the simulation

- Explain the P term and try tuning in simulation. 
    - The proportional term produces an output that is proportional to the calculated error:
    - $$ P = K_pe(t)$$
    - the discretized form: $$P = K_pe(t_k)$$

See also: The magnitude of the proportional response is dependent upon $K_p$ which is the proportional gain constant. A higher proportional gain constant indicates a greater change in the controller’s output in response to the system’s error.

See also: The propellers will spin faster the farther away the drone is. Or can also be imagined as a spring pulling harder the further away you are. 

See also: Oscillations, get damped to some extent by drag. 

##### The Derivative Term

Better: Exercise: Students try different extreme values for the D term in the simulation

- Explain the D term and try tuning in simulation
    - determined by the rate of change of the system’s error over time multiplied by the derivative gain constant $K_d$. 
    - $$D = K_d \frac{de(t)}{dt}$$
    - If students do not yet know calculus, the discretized form of the term: $$D = K_d\frac{e(t_k)-e(t_{k-1})}{\Delta t}$$

See also: Propellors will spin slower the faster you are moving. Can be also like drag pulling harder the faster you are moving.

See also: Teahers should show graphs of different levels of damping: over, under, critical. 

See also: Will not be able to get to setpoint if there are constant effects like gravity. 

##### The Integral Term

Better: Exercise: Students try different extreme values for the I term in the simulation

- Teachers will explain the I term
    - accounts for the accumulated error of the system over time. The output produced is comprised of the sum of the instantaneous error over time multiplied by the integral gain constant $K_i$.

$$I = K_i \int_{0} ^ {t} e (\tau) d \tau$$

- If students do not yet know calculus, the discretized form of the term: $$I = K_i\sum_{i=0}^k e(t_i)\Delta t$$

-  Propellers were spin faster the longer you are away from the set point

Note: Teachers should explain that while we are looking at the terms from the context of 1D altitute control, they are also used for others such as angle, velocity, position, etc of the drone.

##### The overall control function

The overall control function consists as the sum of proportional, integral, and derivative terms. 

$$u(t) = K_pe(t) + K_d \frac{de(t)}{dt} + K_i \int_{0} ^ {t} e (\tau) d \tau$$

In practice, the discretized form of the control function may be more suitable for implementation:

$$u(t) = K_pe(t_k) + K_i\sum_{i=0}^k e(t_i)\Delta t + K_d\frac{e(t_k)-e(t_{k-1})}{\Delta t}$$

#### Show diagram of PID controller Block Diagram

The figure below summarizes the inclusion of a PID controller within a basic control loop.

<figure>
    <figcaption>PID Controller Block Diagram</figcaption>
    <img style='width:35em' src="https://docs.duckietown.org/DT19/doc-sky/out/assets/data-from-img-pid_controller_block_diagram-a2353f10.png"/>
</figure>

##### Tuning: 

See also: Tuning a PID controller is done by setting the control parameters $K_p, K_i, K_d$ to values that fit to be able to get an ideal control response. The three control terms may be correlated and so changing one parameter may impact the influence of another. 

#### Effects of $K_p$:

- Teachers will describe the effects of $K_p$ 

#### Effects of $K_i$

- Teachers will describe the effects of $K_i$ 

#### Effects of $K_d$

- Teachers will describe the effects of $K_d$ 

### Ending The Lesson

- Summarize the effects and what each term is 
<figure>
    <figcaption>General Effects of Control Terms</figcaption>
    <img style='width:35em' src="https://docs.duckietown.org/DT19/doc-sky/out/assets/data-from-img-control_term_effects_table-e300370c.png"/>
</figure>


**Useful Resources and References**

- Teachers can see [EdX lectures on PID Control](https://edge.edx.org/courses/course-v1:BrownX+CS195R+2018_T1/course/#block-v1:BrownX+CS195R+2018_T1+type@chapter+block@0c4aafccbe244af093e640e6e81d9e26)