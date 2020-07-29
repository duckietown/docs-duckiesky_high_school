# Intro to the Motors {#sac3-motors-intro status=ready}

<div class='requirements' markdown='1'>

Requires: 

- Hardware: basestation with Cleanflight, Build Parts 1, 2, and 3 completed

Result: 

- Knowledge: How our motors work, what systems are in place to check them 

- Skills: The ability to utilize Cleanflight and a corresponding Python script interacting with Cleanflight 

</div>

## Introduction to Motors 


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)



### Assessments and Evidence of Understanding

By the end of this lesson, students should be able to demonstrate their knowledge of the innerworkings of their motors, and should be able to run a Python script to navigate Cleanflight and operate their motors. 


### AGENDA (Brief Summary of Activities)

- 5 min: Brainstorming discussion about motors

- 10 min: Brief lecture

- 45 min: Activity with Python and Cleanflight 


### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

You may want to have the Python script that is already written ready to distribute to students, and to make sure all of the students have their Cleanflight flashed and working. 

**Materials needed**

For Students: Basestation with Cleanflight and drone with Build Parts 1, 2, and 3 completed

For Teachers: Basestation with Cleanflight, drone with propellors detatched, and Python script 


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 5 minutes 

**Class discussion**: 

- Have the students spin their motor’s manually and trace the wires back on their drone to see everything the motors are connected to

- Have them brainstorm about what each component of the FC -> ESC -> Motor chain could do 

- Think back to the ethics and safety lessons...Why is smooth motor control so important? 



### Main Lesson

Recommended: 10 minutes

**Motor Lecture**: 

_Motor Explanation_-

There is a coil of metal within each of the 3 wires connected to the motor that allow electrons to flow through and create currents that combine to make a magnetic field that pushes and pulls on the motor to make it speed up and slow down. 

_ESC Explanation_-

The ESCs take the input of power from the battery and digital signals from the flight controller, and then sends volts of electricity to the motor through the 3 wires. 

It is the interface between the digital signal of the FC and the raw voltage going to the motors. 

_Accuracy Explanation_=

Actuators aren’t completely accurate, just like sensors aren’t always completely accurate, so there is a small sensor inside the ESC that gets feedback from the motor by measuring it’s back current (the voltage that comes back into the 3 wires while it’s spinning). This sensor allows our drone to monitor it's motor activity mid-flight. 

<div class='requirements' markdown='1'>

**Vocabulary**: 

- _3-Phase AC_: Stands for **3-Phase Alternating Current** and describes how none of the currents from each of the 3 wires leading to the motor align at the same point, which creates the dissonance and the magnetic field. 

_Back EMF_: **Back electromotive force**, aka counter electromotive force, is the voltage that is emitted in opposition to the change in current of the motors. Each ESC has a small sensor that measures the back EMF and sends that information to the FC in order to monitor the motors as they are spinning. 

</div>

<figure>
    <figcaption>3-Phase AC Diagram</figcaption>
    <img style='width:16em' src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.kebamerica.com%2Fblog%2Fhow-a-3-phase-ac-induction-motor-works%2F&psig=AOvVaw1Wd9OWE6QrvhF6rVpx8tFU&ust=1596125891413000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCLDK2r708uoCFQAAAAAdAAAAABAD"/>
</figure> 

<!-- These explanations can probably all be transfered to the student book-->

TODO: Have them point out different things in Cleanflight that go with this lesson, so they can have things that are hands on to look at.  


### Ending The Lesson

Recommended: 45 minutes 

**Showing motors in action with Cleanflight!** 

Note: This is the most exciting part of this lesson, so it might be best to leave extra time for it. 

See also: Exercise: Use a Python script that sends a constant throttle command that spins the motors at a slow speed. Student tilts the drone to observe the FC corrections. Script prompts the student to input a roll or pitch angle. Students will observe adjacent drone motors spinning up faster. Students will move the drone to the desired angles until the motors return to equal speeds.  

See: This exercise is trying to build intuition for how the motors actuate the drone and how controllers get layered. It also gives an initial hands-on experience with a closed loop controller which they’ll understand better later. 

TODO: Put that script or a tutorial to make that script in here? 

TODO: Might be best to give another option of an activity that doesn't involve Python, but just involves Cleanflight, so classes with less coding confidence can still have a hands-on activity. 


**Useful Resources and References**

The Actuators video of [this edX lecture](https://studio.edge.edx.org/container/block-v1:Brown+CSCI1951-R+2020_summer+type@vertical+block@bdea8a9b9fa0429b943bc371afaf185e). 