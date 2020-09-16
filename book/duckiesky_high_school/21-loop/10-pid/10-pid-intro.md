# Intro to PID {#loop-pid-intro status=ready}
 
[Student version](+duckiesky_high_school_student#loop-pid-intro)
 
<div class='requirements' markdown='1'>
 
Requires:
 
**Hardware** -  Their completed drone and their basestation
**Previous lesson** - [Intro to the Motors](#sac3-motors-intro)
 
 
Result:
 
**Knowledge** -
 
- Students will be able to understand feedback control systems and be able to use control system vocabulary terms such as:
   - Setpoint
   - Control variable
   - Error
 
 
**Skills** - N/A
 
</div>
 
## Intro to PID
 
 
### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)
_ISTE: 1. d.:_ Understand the fundamental concepts of technology operations, demonstrate the ability to choose, use and troubleshoot current technologies and are able to transfer their knowledge to explore emerging technologies.
 
### Assessments and Evidence of Understanding
 
By the end of this lesson, students will understand the different between open and closed loop systems, feedback control systems, what the PID controller is used for in the case of their drones, and be able to use vocabulary terms pertaining to feedback loops and systems.
 
 
### AGENDA (Brief Summary of Activities)
5 min: Introduction to the lesson and identify the 1D hovering problem of a drone.
40 min: Main lesson which includes learning about feedback loops, an example of feedback loops, and defining terms associated with feedback loops.
5 min: Conclusion and summary of the lesson.
 
### Differentiation _(strategies for grouping, ELL, and inclusion)_
 
 
### Advanced preparation/Materials/Set Up (Including Misconceptions)
 
**Materials needed**
 
**Teacher Materials**
 
- Projector for displaying videos or slides
- Reference the student textbook, EdX and Youtube videos (both linked in the useful resources section below) for more detailed explanations of concept snad examples
 
**Classroom Set Up**
- Allow space for students to fly their drones
 
 
## SCRIPT OF TEACHING AND LEARNING ACTIVITIES
 
 
### Introducing The Lesson
 
 
Better: Exercise: Students can try manipulating their LEDs on the drone as they have done before in the build.
 
**Hook:**
 
- Students will already have the ability from previous parts of the build to manipulate their LEDs. To manipulate their LEDs, such as turning them on and off, is a relatively simple task: students can give it a command to tell it to turn on or off. However, there are other tasks that are not as simple. The 1D hovering problem of a drone (getting the drone to hover at a specific altitude) cannot be achieved by just sending one speed to the motors due to factors such as the actions of the actuators and noise of the environment.
 
- Introduce the idea of feedback loops.
 
 
### Main Lesson
 
- Define open loop vs closed loop systems
 
<!-- https://www.electronics-tutorials.ws/systems/open-loop-system.html -->
 
 
Better: Exercise: Do this in two stages. First to demonstrate an "open-loop", a student looks at a target they’re supposed to go to, gets blindfolded, and tries to walk there. To demonstrate a "close-loop system", do the same thing with a partner and without being blindfolded, and get the partner to yell directions. 
 
 
- These two exercises would have shown the difference between open and closed loops: closed loop systems would require constant checking of the distance remaining between their current location and the goal location.
 
Better: Exercise: Teachers draw a block diagram of an closed-loop controller. Show the single input into the controller: the setpoint. Then draw the feedback loop and explain that there are now two inputs to the controller: the setpoint and the error (how far the robot is from the setpoint). Let students label or identify each part of the diagram.
 
- Emphasize that closed-loop systems works in iterations, based on the current setpoint and measurements it determines an output, then does the same process over again after some delay.
 
- Explain important terms and definitions involved with the PID (proportional, integral, derivative) controller
 
Better: Exercise: Students can brainstorm some of examples of feedback loops.
 
- Choose an example of a feedback loop and explain what each of the terms would be represented by in the example: 
   - ie: body thermoregulation, reflexes, hormone feedback loops, heart and blood pressure in the body
 
- Define the error term
 
- Explain the general reason for the PID controllers in systems
 
### Ending The Lesson
 
Better: Exercise: Students try flying their drone, and try identifying what the process variable, setpoint, and control variable would be for the 1D drone hovering problem.
 
- Go over what the three terms are representing in the 1D drone hovering problem.
 
- Feedback loops are used in many technological, engineering, system applications.
 
**Useful Resources and References**
 
- Teachers can see [EdX lectures](https://edge.edx.org/courses/course-v1:BrownX+CS195R+2018_T1/course/#block-v1:BrownX+CS195R+2018_T1+type@chapter+block@0c4aafccbe244af093e640e6e81d9e26) on PID Control
 
Here is a helpful [video](https://www.youtube.com/watch?v=wkfEZmsQqiA) explaining PID controllers

