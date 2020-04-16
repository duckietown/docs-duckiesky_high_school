# Introduction to the Infrared Sensor {#infrared-lesson-plan status=ready}

#### Module X, Lesson Y

## Introduction to the Infrared Range Finder


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)


### Learning Objectives: By the end of this lesson, students will be able to...

1. Explain what an infrared sensor measures and how it makes those measurements.
2. Explain how the infrared sensor is used by their drones.
3. Explain what an Analogue to Digital Converter (ADC) is, and why it is needed.
4. Explain how to calibrate the infrared range sensor, and how  this calibration
converts raw voltage values into distance measurements in meters.
5. Understand the limitations of the infrared sensor


### Assessments and Evidence of Understanding

Students will incrementally write a python program that reads raw voltage values
from the ADC, converts these values to distance measurements, and publishes
the distance measurements to a ROS topic.

### AGENDA (Brief Summary of Activities)

5 min: Hook - review importance of sensors

5 min: Introduction to the Infrared Sensor

5 min: Introduction to ADC converter

10 min: Walk through python program to read values from the IR sensor

10 min: Student practice: write program to read values from the IR sensor

10 min: Introduction to sensor calibration

10 min: Student practice: students calibrate their sensors

10 min: Demonstrate how to create a ROS publisher to publish the calibrated
measurements and a ROS subscriber to read the measurements

10 min: Student practice: students create ROS publisher and subscriber

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

Requires:

- Each student should have their drone built completed to the point that
they have confirmed that they are receiving measurements from the infrared sensor.

- Each student should have completed the following modules:
introduction to sensors, programming in python, connecting to your drone over ssh,
and introduction to ROS

**Materials needed**

For Students: Drone build with functioning infrared sensor, computer with ssh
capabilities, battery to power their drone.

For Teachers: Teachers should have the same materials as students. A projector
may be useful to walk through the code with students, or the code can be
handwritten on the board.


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 5 min

Hook: Remind students why robots need sensors. Ask what types of sensors the
students know. Ask what students thing the drone needs to know. Introduce the
infrared sensor by explain what it measures and how it is used by the drone.

### Main Lesson

Recommended: X minutes/hours

identify hardware and wires, explain what each one does  


### Ending The Lesson

Recommended: X minutes/hours


**Useful Resources and References**
