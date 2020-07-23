# Reading Sensors {#sac2-sensing-reading status=ready}

<div class='requirements' markdown='1'>

Requires: 

- Hardware: basestation, Build Part 1 and 2 completed, battery

- Previous lessons: Unit - [Computing and Networking](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/computing.html), [Calibration](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/sac2_sensing_calibration.html) 

Result: 

- Knowledge: Basic introduction to Python syntax and variables

- Skills: Write a Python script to read and calibrate measurements from their IR sensor

</div>

## Reading Sensors with Software 


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

Recommended: 15 minutes (25 minutes if you do the activity as a class at the bottom)

Explain how sensors need to be read and interpreted quickly in robotics, especially on a drone. The slower we process the sensors' information on the drone, the more time it takes for us (or our computer) to react and control the flight. 

Bad: Problem: We need an automated way of doing the conversion to units. We need measurements many times each second. 

Better: Solution: Python! - a coding language whose purpose is “doing computing” (making mathematical computations or calculations quickly), not formatting text or interacting with the computer


**Python vocab**:

_REPL (Read-eval-print loop)_: 

Also called interactive mode, a REPL is a quick way to interact with Python when trying easy commands. Python reads what you enter, evaluates it on the spot, and prints something out immediately depending on what you wrote. 

_Scripts_: 

This is code written in a text file and saved with ".py" at the end in order to run a lot of code at once that you can work on remotely. This is used when you want Python to preform a long chunk of code at a time or if the code spans multiple files.  

_Function calls_: 

The most simple callable object in Python (just means you put in an argument and Python retuns an object/objects). A function call specifically takes in the argument (or parameters) of a mathematic function and return values or "answers" 

_Printing_: 

<div class='example-usage' markdown="1">

By typingin `print()` and putting what you want the screen to show in the parentheses, Python will then print out the specified message. 

</div>

<!-- I don't know if these definitions are even right? -->

</div>

Note: This is explained clearly in [this online Python activity](https://cscircles.cemc.uwaterloo.ca)! 


### Main Lesson

Recommended: 30 minutes 

Lead through writing a script to print an IR value. 

TODO: Explain how to actually do that 

See also: Exercise: Have your students measure the voltage coming from their IR sensors and have them try to figure out how it relates to the values they’ve been printing. 

TODO: Explain again that the ADC takes in values from the IR sensor that are continuous and then changes it to a format that the Pi can read and how that relates to the values we are computing and measuring. 

See also: Exercise: Every student, for two (or more) known distances, measure the raw ADC value from the Pi
Use them to compute the two constants. 


### Ending The Lesson

Recommended: 15 minutes 

Have your students put all of this information together by writing a script to get a raw ADC value, convert it to a distance, and print. 

TODO: Maybe we should right in how to do that as well. Possibly using [this link](https://github.com/h2r/pidrone_pkg/blob/master/scripts/infrared_pub.py)?

**Useful Resources and References**

[REPL vs. scripts](https://stackabuse.com/python-programming-in-interactive-vs-script-mode/)

[Function calls definition](https://en.wikibooks.org/wiki/Python_Programming/Functions#:~:text=6%20External%20Links-,Function%20Calls,classes%20or%20certain%20class%20instances.) 

