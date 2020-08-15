# Reading Sensors {#sac2-sensing-reading status=ready}

<div class='requirements' markdown='1'>

Requires:

**Hardware**
- basestation
- Build Part 1 and 2 completed
- battery

**Previous lessons**
- [Computing and Networking](#part:computing)

- [Calibration](#sac2-sensing-calibration)

Result:

**Knowledge** - Introduction to Python syntax and concepts including global variables, libraries, classes, methods, functions, and while loops

**Skills**
- Write a Python script to read and calibrate measurements from their IR sensor

- Function composition to reuse their calibration function from the previous lesson

- Dimensional analysis to verify that a function produce the desired units

</div>

## Reading Sensors with Software


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)



### Assessments and Evidence of Understanding

By the end of this lesson, students will be able to measure distances on their Pi using the IR sensor.


### AGENDA (Brief Summary of Activities)
5 min: classroom setup
10 min: introduction to the lesson




### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

**Teacher Materials:** base station, drone build completed to build part 2, meter stick

**Classroom Setup:** Teachers can write a DO NOW on the board for students to set up their basestations and open a web browser. Have them complete the creation of a GitHub account process (step 1 in the student book) while you introduce the lesson.


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 25 minutes

**Activity 1:** Reading and Calibrating the Sensor without Programming

This is an interactive activity used to motivate the need for programming.

Divide the class into groups of three. In each group, designate one student to read the voltage value from the multimeter. This student will need to setup their multimeter to read up to 20V. Designate another student to convert the voltage value to a distance in meters. This student will need to a calculator and the calibration formula from the previous lesson. Designate a third student to hold the IR sensor facing down at a surface. This student will need to plug the battery into their drone so the IR sensor has power.

The goal of the activity is to get the IR sensor as close to 0.3 meters as possible. It will require the group to work together to read the IR sensor, convert the reading, and then move the sensor up or down to get the 0.3 meters. While the students are working, write the debrief questions below on the board. After 5 minutes (or more/less depending on the class), the teacher will walk around and check the height of the IR sensor using a meter stick to see which group was closest. If students finish early, they can go on to the debrief questions below:

Have the students debrief by answering the following questions:

Q: What step took the longest? (reading, converting, moving the sensor)

Q: How could you speed up this process?

Q: How did it feel to do the same thing over and over again?

**Background:**

Explain how sensors need to be read and interpreted quickly in robotics, especially on a drone. The slower we process the sensors' information on the drone, the more time it takes for us (or our computer) to react and control the flight.

Bad: Problem: We need an **automated** way of doing the conversion to units. We need measurements many times each second. Automated means that the measurements and conversions happen without the user needing to do anything.

Better: Solution: Write a computer program to read and convert the measurements!

So far, we've seen two coding languages: text editors which format text, and bash which is used for interacting with the computer. We need a coding language whose purpose is “doing computing” (making mathematical computations or calculations quickly). We need Python!


Note: This is explained clearly in !


### Main Lesson

Recommended: 60 minutes

Explain that the first challenge with automating the sensor reading is to get the hardware devices to "talk" to eachother. Recall that the IR sensor produces a voltage, which is an *analog* signal. However, many computers, including the Pi, can only read *digital* signals (1's and 0's only). Explain that the ADC takes in the analog signal and converts it to a digital signal that the Pi can read.

Lead the students through Activity 1 in the Student Book. This can be done either by having the students read through the activity, or by following the teacher through the activity on a projector.

Explain that it is inconvenient to keep running the script every time we want to take a measurement. Introduce the concept of while loops in Python. Lead the students through Activity 2 in the Student Book , and stop before the "Slow Down" section. Explain that the while loop is running as fast as the computer can go, but this slows down other computer processes. Additionally, it makes it hard for the students to read the values. Introduce the concept of waiting between measurements. Finish Activity 2.

For advanced students who are asking the question: *How did they know how to read from the ADC?*. Let them go or lead them through Activity 3 in the Student Book.

Depending on how advanced the students are, explain that although we have a calibration function from Volts to meters, the Python script can only read the ADC value. Therefore, we need a way to convert from the ADC value to meters. Lead the students through Activity 4 in the Student Book.

For all students, explain that the ADC value needs to be converted to a distance measurement, just like the students had to do in the introduction activity. Lead the students through Activity 5 in the Student Book to convert the ADC values to distance.


### Ending The Lesson

Review what was accomplished today, and how it relates to the overall goal of flying the drone:

In the previous lesson, we:

1. created a function that converted Volts to meters

In this lesson, we:

1. learned that the drone needs to read and convert the measurements *fast*, and so we needed to *automate* this process.

1. learned that the Pi cannot read the analog voltage from the IR sensor, so the value needed to be converted to a digital value using the ADC

1. learned how to read and print the ADC value on the Pi.

1. learned how to convert the ADC value to meters.


If students want more practice with Python, they can go through [this online Python activity](https://cscircles.cemc.uwaterloo.ca) on their own time.


**Useful Resources and References**

**Python vocab**:

_Scripts_:

This is code written in a text file and saved with ".py" at the end in order to run a lot of code at once that you can work on remotely. This is used when you want Python to preform a long chunk of code at a time or if the code spans multiple files.  

_Function calls_:

The most simple callable object in Python (just means you put in an argument and Python retuns an object/objects). A function call specifically takes in the argument (or parameters) of a mathematic function and return values or "answers"

_Printing_:

<div class='example-usage' markdown="1">

By typingin `print()` and putting what you want the screen to show in the parentheses, Python will then print out the specified message.

</div>


[Function calls definition](https://en.wikibooks.org/wiki/Python_Programming/Functions#:~:text=6%20External%20Links-,Function%20Calls,classes%20or%20certain%20class%20instances.)
