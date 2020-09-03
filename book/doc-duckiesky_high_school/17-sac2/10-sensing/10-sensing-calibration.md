# Calibration {#sac2-sensing-calibration status=ready}

[Student version](+duckiesky_high_school_student#sac2-sensing-calibration)

<div class='requirements' markdown='1'>

Requires:

**Hardware** -

- Basestation

- IR sensors

- Multimeter

- Graph paper or a computer with Excel

**Previous Lesson** - [Introduction to Sensors](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/sac1_basics_sensors.html)

Result:

**Knowledge** -  

- Understanding that sensors don't provide readings in standardized units or scales

- The the specific nonlinearities of the IR sensor

- Equation of a line and its use for linear approximation

- How to interpolate

**Skills** -  

- Calibrating measurements by linearizing the readings and then interpolating known readings

</div>

## Calibration  


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)

_ISTE: 5.c._: Collect data or identify relevant data sets, use digital tools to analyze them, and represent data in various ways to facilitate problem-solving and decision-making.


### Assessments and Evidence of Understanding

By the end of this lesson, students should have a completed _Voltage vs. 1/distance_ graph.  


### AGENDA (Brief Summary of Activities)

25 min: In depth explanation of the IR sensor

25 min: Activity graphing the inputs and outputs of the IR sensor to linearize it and interpolate values using the equation of the line

5 min: Wrap up and explanation of the bigger purpose of this exercise


### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Teacher Materials**

- Already completed _Voltage vs. Distance_ and _Voltage vs. 1/distance_ graph to compare with students' graphs. Feel free to make your own, or there are links to example graphs below.

- Projector/ slides to show graphs if needed.

**Classroom Set Up:**

- Teachers can write a DO NOW on the board that says "Start thinking about what you already know about Infared Sensors. What does that name make you think of?"

- Each student should have a multimeter either on their desk or ready to be passed out, along with their IR Sensor.


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 25 minutes

**Hook:**

- Discuss what students already believe their IR Sensor is (as stated in the DO NOW) and fascilitate a discussion of the importance of monitoring drone height in the right units and communicating that with different parts of the drone. This lesson is important because not only does it help students understand how their own drones' sensors recieve and send vital information, it also reinforces basic graphing and conversion skills that have many applications in the world of STEM and beyond.

Using the student book material or the links listed below, explain what Infared (IR) Sensors are and how they work.

See also: It might be useful to review what [infared light](https://www.livescience.com/50260-infrared-radiation.html) is and where it can be found. What environmental factors could potentially alter our drone's IR readings?

Possible discussion question:

Q: Will there be a higher voltage emitted when the sensor is closer to the surface or further away?

A: There will be a higher voltage reading when the sensor is closer to the surface, because the infared light bounding back will be stronger the less distance it has to travel.

Better: Exercise: Have your students use the multimeter to measure the voltage from their IR sensors at different distances away from the floor or their desks. [This video](https://youtu.be/KYreVzorAs4) an example of students doing this. Either on a piece of graph paper or in an Excel spreadsheet, have them record and plot this data with "height above ground (cm)" as the x-axis and "IR sensor voltage (V)" as the y-axis to identify a relationship between the two variables (they will come out to be the inverse transform). Then, they can calculate the distance between the surface and the sensor by using only the voltage.


### Main Lesson

Recommended: 25 minutes

**Analyze the Data**

1. Have students analyze their own graphs to try and find a trend in the data. Encourage note taking and group collaboration on this, since they should all have similar data points.

Q: What does the graph show about the uses and limitations of the IR sensor?

2. Pull up your own graph of IR values to show students. Ask your students about various points and see if they compare to yours to show that students’ values may be different.

Note: A particular voltage has _at least_ two potential distances associated with it. Point out that the sensor stops working past a certain distance.

3. Emphasize that we have to make the assumption that the sensor is within the useful range, and that we have to enforce that it stays within that range when flying, so there will be a height limit when flying the actual drone.

5. Present the _voltage vs distance) graphs in the [IR sensor data sheet](https://www.makerguides.com/wp-content/uploads/2019/02/GP2Y0A21YK0F-Datasheet.pdf). The data sheet is like an instruction book for a sensor: it contains information about the sensor written by the designer. By familiarizing students with the data sheet for the IR sensor, the goal is to promote students' self-efficacy to learn about other sensors on the drone and on other robots.

4. Finally, use the linearization shown in the data sheet (voltage vs. inverse distance) to find the actual mathematical relationship between voltage and distance. Highlight that the data takes on the shape of 1/x, and then show a graph of voltage vs 1/distance.

        Voltage = k/distance + p


<figure>
    <figcaption>Voltage vs. Distance and Inverse Distance Graphs (Ignore the key)</figcaption>
    <img style='width:50em' src="https://www.researchgate.net/profile/Eric_Johnson15/publication/48267744/figure/fig1/AS:306095043170310@1449990153544/SHARP-GP2Y0A02YK0F-infrared-range-sensor-response-curves-8.png"/>
</figure>

Better: Exercise: Have your students convert their own plot to be voltage vs 1/distance to see how linear it is. Notice that there’s an offset towards the right side of the graph where 1/x is larger (distance to the sensor is smaller).
<!-- I think I could say that better but idk how-->


### Ending The Lesson

Recommended: 10 minutes

Better: Exercise: Using their linear equations from the above activity, students can now predict Voltage based on a specific Height and vice versa by interpolating within the graph. Put different heights on the board and see who can calculate the Voltage first with the equation, and then have students test it on the actual IR sensor.

- Remind students that even though they used the equation of a line to interpolate and estimate certain voltages and distances, that there are specific nonlinearities of the IR sensor.

- Explain how they calibrated the readings by putting them into a graph so they can estimate data in the middle since sensors don’t provide readings in standardized units or scales. We will add an ADC (Analog-to-Digital Converter) to allow our Rasberry Pi to read distance from our IR sensor.


**Useful Resources and References**

1. [EdX lecture](https://edge.edx.org/courses/course-v1:BrownX+CS195R+2018_T1/courseware/0e3596880ec446d8ab63df427e02e9c4/3bde0261d3b04ccfa06f77eec394f97a/?activate_block_id=block-v1%3ABrownX%2BCS195R%2B2018_T1%2Btype%40sequential%2Bblock%403bde0261d3b04ccfa06f77eec394f97a)  

2. [IR sensor tutorial](https://www.makerguides.com/sharp-gp2y0a21yk0f-ir-distance-sensor-arduino-tutorial/)
