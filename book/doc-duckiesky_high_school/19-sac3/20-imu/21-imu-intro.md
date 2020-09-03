# Intro to the IMU {#sac3-imu-intro status=ready}

<div class='requirements' markdown='1'>

Requires:

**Hardware** -

- Basestation with Cleanflight 

- Build Parts 1, 2, and 3 completed

**Previous Lesson** - [Drone Operation - Sensors and Actuators](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/introduction_operation_sensors.html)

Result:

**Knowledge** -

- Learn the definition and purpose of the IMU

- Be able to point out the location of the IMU on the drone

- Be able to explain how the IMU works

</div>

## Introduction to IMU


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)



### Assessments and Evidence of Understanding

By the end of this lesson, students should be able to explain the basic functioning of the IMU and the laws of physics that go behind it.


### AGENDA (Brief Summary of Activities)

- 10 min: Watch a short video.

- 20 min: Give a lecture on the physics of the IMU.

- 10 min: See the effects in Cleanflight


### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Teacher Materials**

Place to play a video, basestation with Cleanflight, and drone.

**Classroom Setup**

Teachers can write a DO NOW on the board for students to set up their basestations and Cleanflight


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 10 minutes

[Watch this video](https://youtu.be/DSypZP3R0sQ)

While watching, pause to emphasize the following:

1. Where the IMU is located

2. The two sensors in the IMU: Gyroscope and Accelerometer, that measure angular velocity and acceleration respectively.

3. Optional: How the Micro-Electro-Mechanical (MEM) System works -

    _Gyroscope_: gyros rotate -> vibration -> voltage -> ADCs

    _Accelerometer_: measure displacement, and then differentiate to get acceleration

4. Note: They measure without interacting with the rest of the world! E.g. what a spacecraft would have to use. The downside of this is that it does not have long-term accuracy.


### Main Lesson

Recommended: 20 minutes

#### **A Smidgeon of Physics: Newton's Two Laws of Motion:**

1. _Newton’s First Law of Motion_: “**The vis insita, or innate force of matter**, is a power of resisting by which every body, as much as in it lies, endeavours to preserve its present state, whether it be of rest or of moving uniformly forward in a straight line.”

First Law describes **Inertia**: Object’s tendency to resist the change of motion.

If we want the object to move, we have to exert eternal forces, and the second law tells us the effect of this.

2. _Newton’s Second Law of Motion_: F = ma (The force on an object produces acceleration)

    - F: Force on object

    - m: Mass of the object

    - a: the acceleration of the object, which is explained [here](https://www.grc.nasa.gov/WWW/K-12/airplane/disvelac.html)

    - In short: Displacement is the change in position. Velocity is the rate of change of displacement. Acceleration is the rate of change of velocity.

**The accelerometer measures the position changes and calculates all the way down to acceleration (accumulating errors along the way).**

#### **Physics Continues: Circular Motion**

Q: What causes an object to have a circular motion? Newton’s Second Law tells us there must be a force exerted on the object. What is the direction of the force?

A: Centripetal Force! Pointing to the center of the circular path.

<figure>
    <figcaption>Centripetal Force Diagram</figcaption>
    <img style='width:16em' src="https://celestialobject.files.wordpress.com/2012/01/ascentri3.jpg"/>
</figure>

See: Example: The gravitational pull from the earth to the moon is the centripetal force causing the moon to move around the earth.

Q: For circular motion, we also care about how fast the object’s orientation is changing.

A: Angular velocity, which measures the rate of change of the object’s orientation

Teacher might refer to the first few paragraphs of [this page](https://xaktly.com/AngularVelocity.html
)

Similarly, angular acceleration is the rate of change of angular velocity.

**The gyroscope measures rotation and calculates all the way down to angular acceleration (accumulating errors along the way).**

See also: Note: The analogy between [displacement, velocity, acceleration] and [Orientation, angular velocity, angular acceleration].

Better: One student sits in a chair with eyes closed and another student spins the chair. The student in the chair guesses their orientation based on the feeling of the spin. Note that the student’s accuracy declines over time, which is similar to the accelerometer and gyroscope accumulates errors.


### Ending The Lesson

Recommended: 10 minutes

Q: How do we account for the errors in the long term?

Pause for group discussion and presentation.

A: We need sensors that interact with the outside world, such as GPS, to know the location.

TODO: show these values and drone visualization in cleanflight


**Useful Resources and References**

Between times 0:21 and 5:00 of [this video](https://www.youtube.com/watch?v=whSw42XddsU).
