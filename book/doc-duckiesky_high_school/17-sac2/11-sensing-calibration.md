# Calibration {#sac2-sensing-calibration status=ready}

<div class='requirements' markdown='1'>

Requires: 

- Hardware: Basestation, IR sensors, Multimeter 

- Previous Lesson: [Introduction to Sensors](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/sac1_basics_sensors.html) 

Result: 

**Knowledge**: 

- Understanding that sensors don't provide readings in standardized units or scales

- The the specific nonlinearities of the IR sensor

- Equation of a line and its use for linear approximation

- How to interpolate 

**Skills**: 

- Calibrating measurements by linearizing the readings and then interpolating known readings

</div>

## Calibration  


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)


### Assessments and Evidence of Understanding

Each student should have a completed _Voltage vs. 1/distance_ graph by the end of the lesson. 


### AGENDA (Brief Summary of Activities)

- In depth explanation of the IR sensor. 

- Activity graphing the inputs and outputs of the IR sensor to linearize it and interpolate values using the equation of the line. 

- Lesson on the limitations of the sensor and why there is a height limit for the drone. 

- Wrap up and explanation of the bigger purpose of this exercise. 


### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

For Students: IR sensor, multimeter

For Teachers: Already completed _Voltage vs. Distance_ and _Voltage vs. 1/distance_ graph to compare with students' graphs. 


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 25 minutes 

Explain for Infared (IR) Sensors work. 

    The IR sensor emits infared light and also detects infared light, measures the intensity of the light that is returning, and emits a voltage that correlates with the intensity of that light. (V0 = 5V, Ground = 0V). The sensor emits 0-5 volts of electricity depending on how far away it is from a surface, and therefore how strong the infared signals are that are bouncing off that surface. 

Possible discussion question: 

Q: Will there be a higher voltage emitted when the sensor is closer to the surface or further away? 

A: There will be a higher voltage reading when the sensor is closer to the surface, because the infared light bounding back will be stronger the less distance it has to travel. 

See also: Exercise: Have your students use the multimeter to measure the voltage from their IR sensors at different distances away from the floor or their desks. Have them record and plot this data to identify a relationship between the two variables (they are the inverse transform). Then, they can calculate the distance between the surface and the sensor by using only the voltage. 


### Main Lesson

Recommended: 25 minutes

- Pull up the actual reference plot in the datasheet. Ask your students about various points and see if they compare to yours to show that students’ values may be different. A particular voltage has _at least_ two potential distances associated with it. Point out that the sensor stops working past a certain distance. 

- Emphasize that we have to make the assumption that the sensor is within the useful range, and that we have to enforce that it stays within that range when flying, so there will be a height limit when flying the actual drone. 

- Finally, explain (or have them derive) the actual mathematical relationship between voltage and distance. 

    Voltage = k/distance + p 

Highlight that the data takes on the shape of 1/x, and then show a graph of voltage vs 1/distance.

<figure>
    <figcaption>Voltage vs. Distance and Inverse Distance Graphs (Ignore the key)</figcaption>
    <img style='width:20em' src="https://www.researchgate.net/profile/Eric_Johnson15/publication/48267744/figure/fig1/AS:306095043170310@1449990153544/SHARP-GP2Y0A02YK0F-infrared-range-sensor-response-curves-8.png"/>
</figure>

See also: Exercise: Have your students convert their own plot to be voltage vs 1/distance to see how linear it is. Notice that there’s an offset towards the right side of the graph where 1/x is larger (distance to the sensor is smaller). 
<!-- I think I could say that better but idk how-->

### Ending The Lesson

Recommended: 10 minutes

- Remind students that even though they used the equation of a line to interpolate and estimate certain voltages and distances, that there are specific nonlinearities of the IR sensor. 

- Explain how they calibrated the readings by putting them into a graph so they can estimate data in the middle since sensors don’t provide readings in standardized units or scales. We will add an ADC (Analog-to-Digital Converter) to allow our Rasberry Pi to read distance from our IR sensor. 



**Useful Resources and References**
[This edX lecture](https://edge.edx.org/courses/course-v1:BrownX+CS195R+2018_T1/courseware/0e3596880ec446d8ab63df427e02e9c4/3bde0261d3b04ccfa06f77eec394f97a/?activate_block_id=block-v1%3ABrownX%2BCS195R%2B2018_T1%2Btype%40sequential%2Bblock%403bde0261d3b04ccfa06f77eec394f97a) explains IR sensors in more detail and shows a video of students using their multimeter to read the voltage of the IR sensor. 
