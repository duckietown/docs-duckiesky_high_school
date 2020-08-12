# Intro to Sensors {#sac1-basics-sensors status=ready}

<div class='requirements' markdown='1'>

Requires: 

**Previous lesson** - [Signals and Connections](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/electronics_circuitry_signals.html)


Result: 

**Knowledge** -

- The ability to differentiate between examples of continuous signals and those discretized in time and/or value 

- Know the purpose of discretizing continuous signals

- Know the general pathway for measuring a physical system 
potential

- Get a sense of the limitations of electrical sensors


</div>

## Introduction to Sensors


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)



### Assessments and Evidence of Understanding

By the end of the lesson, students are able to understand how sensors process signals, as well as how they are subject to errors.

### AGENDA (Brief Summary of Activities)

10 min: Brainstorming the senses of robots based on human experience

25 min: Introduce conecepts about sensors

15 min: Fun exercise to help students experience the concepts introduced

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Classroom Set Up**

Teacher can write a DO NOW on the board for students to think about what can be measured by a robot.


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 10 mintues

See: **Hook**

Students brainstorm and discuss in groups the things that can be measured by a robot, and possibly write their ideas on board.

After this is done, teachers do a review what our drone’s three sensors measure: 

- IR sensor - measures distance

- IMU sensor - measures acceleration 

- The camera - measures planar motion

**Explain the definition of roll, pitch, and yaw.**

<figure>
    <figcaption>Roll, Pitch, and Yaw Diagram</figcaption>
    <img style='width:12em' src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/Flight_dynamics_with_text_ortho.svg/1200px-Flight_dynamics_with_text_ortho.svg.png"/>
</figure>

With the help of this picture, teacher introduces the terms roll pitch and yaw, and then asks the students to identify which of the sensors measure each of them (IMU for roll and pitch, camera for yaw)

Better: **Optional**: Have your students make paper airplanes to physically demonstrate roll, pitch, and yaw. 

### Main Lesson

Recommended: 25 minutes

The main lesson is evolved around introducing 3 questions, possibly let students discuss their solutions, and then providing solutions to questions.

Question 1. **How computers interpret sensors' output.** 

Q: Refer to the [signals lesson](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/electronics_circuitry_signals.html) that computers can only understand a finite set of numbers, so we need to convert sensors' output to a finite set of numbers.

Pause for discussion if necessary

A: Analog-to-Digital Converter (ADC)!

<div class='requirements' markdown="1">

Voltage or Current is produced by the sensors -> amplification (convert to voltage if necessary) -> ADC

</div> 

<figure>
    <figcaption>Analog and Digital Signal Diagram</figcaption>
    <img style='width:12em' src="https://www.allaboutcircuits.com/uploads/articles/An-Introduction-to-Digital-Signal-Processing-(1).png"/>
</figure>

Question 2. **How we acquire data that are not directly measured.**

Q: What if we want the data in between those signals? Or if we want to predict the future values?

Pause for discussion if necessary

A: Interpolation (estimate the data points in between known data) and extrapolation (using the current trend to predict the future data)

<figure>
    <figcaption>Interpolation and Exterpolation Graph</figcaption>
    <img style='width:12em' src="https://storage.ning.com/topology/rest/1.0/file/get/2656751898?profile=original"/>
</figure>

Question 3. **How good are our sensors?**

There are two measures of the “goodness” of a sensor: 

    1. Accuracy: How close are the measurements to the truth

    2. Precision: How close are the measurements of the same item to each other

<figure>
    <figcaption>Accuracy and Precision Graph</figcaption>
    <img style='width:12em' src="https://circuitglobe.com/wp-content/uploads/2016/09/accuracy-and-precision-compressor.jpg"/>
</figure>

See also: We need to pay extra attention to the units used. Here are the industry standards.

    - Meters, NOT inches or feet
    
    - Radians, NOT degrees

Q: Sensors have errors, too! Just like the signal noise from the [electronics unit](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/electronics_circuitry_signals.html). How might we mitigate them?

Pause for discussion if necessary

A: 

    - Filtering Frequencies: cut the frequency measurements that are unreasonably high or low

    - Combining data from multiple sensors

    - Cleverly decide which data are trustworthy


### Ending The Lesson

Recommended: 15 minutes 

Better: Mimicking the second way (combining data from multiple sensors) that make sensors more accurate – students individually measure something (a distance, number of jelly beans in a jar, or any other creative activities) and then averaging the individual guesses.


**Useful Resources and References**
