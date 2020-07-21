# Sensors and Actuators {#introduction-operation-sensors status=ready}

<div class='requirements' markdown='1'>

Requires: 
**Hardware** - Unassembled drone kit.   
**Previous lesson** - None.

Result: 
**Knowledge** - 

- Basic components of robot hardware and software

- Your specific drone's sensors and actuators

- How the sensors and actuators interact to achieve stable flight

**Skills** - 

- The ability to identify all of the sensors and actuators of your drone 

</div>

## Lesson 1: Anatomy of a Robot 


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)



### Assessments and Evidence of Understanding

Students at the end of this lesson should be able to describe the basic components of a robot and point to what everything in their drone kit is. 
<!-- Potentially could put a link to a "label the parts" kind of assesment if wanted -->


### AGENDA (Brief Summary of Activities)

1. Quick lecture about robot anatomy 

2. Comprehensive disscussion with class 

3. Going through the physical parts of the drone and labeling their use 


### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

For Students: The drone kit 

For Teachers: The  drone kit 

<!-- I don't think we need differentiation, advanced prep, or materials needed because this is a short lesson, but I'll leave them in there for now just in case-->


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 15 minutes 

1. Introduce Important Vocabulary 

<div class='requirements' markdown="1">

**Sensors** - parts on a robot that allow it to _sense_, or estimate, its own conditions or environment 

**Actuators** - parts on a robot that use energy to _interact_ with its environment

**Controller** - connects the input from the sensors to create an output from the actuators in order to accomplish a goal 

</div>

2. Possible Class Discussion Questions: 

Note: This is an optional discussion based on the engagement of your class. If this seems too basic, feel free to skip through the introduction. 
<!-- this might not have to be said idk-->


Q: What _sensors_ to humans have to percieve the world around them? 

A: Eyes, ears, nose, taste buds, sense of touch, etc. 


Q: What types of robots would need the same sensors you have? 

A: _Example_: Self driving cars would need to see the road like your eyes do. (answers will vary)


Q: What _actuators_ do humans have to act on the world around them? 

A: Arms, legs, fingers, muscles, etc. 


Q: How might these actuators and sensors combine (either on a human or robot) to create a more complex movement or action? 

A: _Example_: Our nose might smell something we want to walk towards, but we still have to use our eyes to make sure we aren't bumping into anything on the way. The input from our nose and eyes influence how and where our legs move to walk us towards the smell. (answers will vary)


Q: What are the _controllers_ that humans have to combine input and control action? 

A: The brain, spinal cord, control loops (handle reflexes, homeostasis, blood flow etc. based on outside information without having to conciosly think about it) 



### Main Lesson

Recommended: 35 minutes/hours

Note: These are the simple definitions of the parts to get a basic understanding. Everything will be described in greater detail later in the book. 

- Sensors in your drone: 


1. **Infared Sensor (IR)** - measures the distance to an object (or the ground) using infared beams, then uses the cable to report it 

<figure>
    <figcaption>IR + IR Sensor Cable</figcaption>
    <img style='width:16em' src="https://docs.duckietown.org/daffy/opmanual_sky/out/assets/data-from-img-ir-e874dd15.png"/>
</figure> 


2. **Camera** - observes 2D images of the world to allow the drone to determine its planar position and speed 

<figure>
    <figcaption>Camera (Pi Cam) + Flexible Flat Cable (FFC)</figcaption>
    <img style='width:16em' src="https://docs.duckietown.org/daffy/opmanual_sky/out/assets/data-from-img-cam-6416de2c.png"/>
</figure> 


3. **Inertial Measurement Unit (IMU)** - sensor on your flight controller (FC) that allows the drone to tell how it is accelerating and rotating in all 3 dimensions

<figure>
    <figcaption>Flight Controller (FC) with IMU</figcaption>
    <img style='width:16em' src="https://docs.duckietown.org/daffy/opmanual_sky/out/assets/data-from-img-fc-31280b0a.png"/>
</figure> 

<!-- need to put in the part about roll, pitch, yaw with the paper airplane excercise--> 


- Actuators on your drone: 

1. **Motors** - actuators that spin at a variable RPM (revolutions per minute) depending on how much power it recieves (quantaty = 4)

<figure>
    <figcaption>2 CW and 2 CCW Motors</figcaption>
    <img style='width:16em' src="https://docs.duckietown.org/daffy/opmanual_sky/out/assets/data-from-img-2205_2300kv_brushless_motors_red-5ef15e4a.jpg"/>
</figure> 

2. **Propellers** - device with blades attached to motors to turn rotational motion into thrust (quantity = 4) 

<figure>
    <figcaption>2 Clockwise and 2 Counterclockwise Blade Propellers</figcaption>
    <img style='width:16em' src="https://docs.duckietown.org/daffy/opmanual_sky/out/assets/data-from-img-props-0d9497a1.png"/>
</figure> 

See also: Optional activity - The propellers will attach to the motors, which will attach to the 4 arms of your drone. Ask your students to identify which of their propellers are clockwise and which are counterclockwise using the arrows. A possible excersise is to have them think critically about which propellers would have to be attached to which arm and move when trying to preform different flying tasks (ex. flying up and straight, flying to the right without losing hight, etc.). 

3. **LED** - actuator that lights up that you will be using in some experiments 

- Controllers in your drone: 
<!-- make the distinction between controllers and computers?-->

1. **Electronic Speed Controllers (ESCs)** - small computers that react extremely quickly to accomplish to simply keep the motors spinning at a particular speed by sending it a variable amount of power based on the input it recieves (quantity = 4)

<figure>
    <figcaption>1 ESC for each Motor</figcaption>
    <img style='width:16em' src="https://docs.duckietown.org/daffy/opmanual_sky/out/assets/data-from-img-esc-resized-1024-07963732.jpg"/>
</figure> 

2. **Flight Controller** - computer that connects the IMU sensor to the ESCs and motors to react quickly in order to fly the drone at a particular angle 
<!--this definition is wordy-->

<figure>
    <figcaption>Flight Controller</figcaption>
    <img style='width:16em' src="https://docs.duckietown.org/daffy/opmanual_sky/out/assets/data-from-img-fc_labeled-resized-1024-79c845dc.jpg"/>
</figure> 

3. **Raspberry Pi** - more powerful computer that accomplishes a complicated goal, such as flying at a particular speed or to a particular position (it excecutes specific code loaded via an SD card)

<figure>
    <figcaption>Raspberry Pi Model B</figcaption>
    <img style='width:16em' src="https://docs.duckietown.org/daffy/opmanual_sky/out/assets/data-from-img-pi_on_box-327809ca.png"/>
</figure>

### Ending The Lesson

Recommended: 10 minutes

- Make sure that your students can identify every part of the drone, so they aren't confused on vocabulary during the build. 

See also: Tangible games to enhance learning: Call out a part and see who can grab theirs first. You could also have them sort all of their parts into actuators, sensors, controllers, and other on their desk. 

- Understand that all of these components are just building blocks that can be put together to build a drone, but that can also be used in robotics to accomplish a multitude of tasks. 

See also: Have your students come up with another use for a part or combination of parts that would allow a robot to do something other than fly a drone. Encourage them to use the vocabulary from this lesson in their responses. 


**Useful Resources and References**
 
[Explanation of Drone Flight Dynamics](https://www.mathworks.com/videos/drone-simulation-and-control-part-1-setting-up-the-control-problem-1539323440930.html)
