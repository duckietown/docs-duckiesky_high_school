# Lesson 1: Intro to Sensors {#sac1-basics-sensors status=ready}

<div class='requirements' markdown='1'>

Requires: Previous Lesson - [Signals and Connections](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/electronics_circuitry_signals.html)


Results: 

- The ability to differentiate between examples of continuous signals and those discretized in time and/or value 

- Know the purpose of discretizing continuous signals

- Know the general pathway for measuring a physical system 

- Get a sense of the potential limitations of electrical sensors


</div>

## Introduction to Sensors


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)



### Assessments and Evidence of Understanding


### AGENDA (Brief Summary of Activities)


### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

For Students:

For Teachers:


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 5 mintues 

Let students brainstorm the things that can be measured and lead a review what our drone’s three sensors measure: 

- IR sensor - measures distance

- IMU sensor - measures acceleration 

- The camera - measures planar motion


### Main Lesson

Recommended: 30 minutes 

1. Explain the definition of roll, pitch, and yaw. 

<figure>
    <figcaption>Roll, Pitch, and Yaw Diagram</figcaption>
    <img style='width:12em' src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/Flight_dynamics_with_text_ortho.svg/1200px-Flight_dynamics_with_text_ortho.svg.png"/>
</figure>

See also: **Optional Excercise: Have your students make paper airplanes to physically demonstrate roll, pitch, and yaw. 


Ask the students to identify which of the sensors measure each of them: 

    - IMU for roll and pitch 
    
    - Camera for yaw 

2. How computers interpret sensors' output. 

Bad: Refer to the [signals lesson](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/electronics_circuitry_signals.html) that computers can only understand a finite set of numbers, so we need to convert sensors' output to a finite set of numbers. 

Better: Analog-to-Digital Converter (ADC)!

Voltage or Current is produced by the sensors -> amplification (convert to voltage if necessary) -> ADC

<figure>
    <figcaption>Analog and Digital Signal Diagram</figcaption>
    <img style='width:12em' src="https://www.allaboutcircuits.com/uploads/articles/An-Introduction-to-Digital-Signal-Processing-(1).png"/>
</figure>

3. Introduce a new question. 

Q: What if we want the data in between those signals? Or if we want to predict the future values?

A: Interpolation (estimate the data points in between known data) and extrapolation (using the current trend to predict the future data)

<figure>
    <figcaption>Interpolation and Exterpolation Graph</figcaption>
    <img style='width:12em' src="https://storage.ning.com/topology/rest/1.0/file/get/2656751898?profile=original"/>
</figure>

TODO: Need to think of ways to build intuitions for sensor calibration

4. Sensors are not always correct. 

- First, we need to calibrate it with equations that were proven to be pretty good. (Be careful with units!)

- There are two measures of the “goodness” of a sensor: 

    1. Accuracy: How close are the measurements to the truth

    2. Precision: How close are the measurements of the same item to each other 

<figure>
<figcaption>Accuracy and Precision Graph</figcaption>
<img style='width:12em' src="https://i0.wp.com/wp.stolaf.edu/it/files/2017/06/precsionvsaccuracy_crashcourse.png?resize=579%2C600&ssl=1"/>
</figure>

- Problems: sensors have errors, too! Just like the signal noise from the [electronics unit](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/electronics_circuitry_signals.html).

Solution: 

    - Filtering Frequencies: cut the frequency measurements that are unreasonably high or low

    - Combining data from multiple sensors

    - Cleverly decide which data are trustworthy


### Ending The Lesson

Recommended: 15 minutes 

See also: **Exercise**: Mimicking the second way (combining data from multiple sensors) that make sensors more accurate – students individually measure something (a distance, number of jelly beans in a jar, or any other creative activities) and then averaging the individual guesses.  


**Useful Resources and References**
