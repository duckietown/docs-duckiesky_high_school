# Creating a ROS Publisher {#sac2-ros-publisher status=ready}

<div class='requirements' markdown='1'>

Requires: 

- Hardware: basestation, Build Parts 1 and 2 completed

- Previous Lesson: [Introduction to ROS](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/sac2_ros_intro.html)

Result: 

- Knowledge: Python loops 

- Skills: The ability to create custom ROS messages, create ROS publisher, and use ROS commands


</div>

## Creating a ROS Publisher


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)

_NGSS: HS - ETS1 - 2_: Design a solution to a complex real-world problem by breaking it down into smaller, more manageable problems that can be solved through engineering.

_ISTE: 5. c._: Break problems into component parts, extract key information, and develop descriptive models to understand complex systems or facilitate problem-solving


### Assessments and Evidence of Understanding


### AGENDA (Brief Summary of Activities)


### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

For Students:

For Teachers:


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 15 minutes 

[Creat a package](http://wiki.ros.org/ROS/Tutorials/CreatingPackage) and [build a package](http://wiki.ros.org/ROS/Tutorials/BuildingPackages) with the linked instructions.


### Main Lesson

Recommended: 30 minutes

Use [this tutorial](https://wiki.ros.org/ROS/Tutorials/CreatingMsgAndSrv) to explain how to creat ROS messages. 

Two types of messages that might need more explaining: 

1. **Header:** The header contains a timestamp and coordinate frame information that is commonly used in ROS

2. **Float:** More precise measurement than integers

Lead students to create various messages. 

See also: Possible example: Create a ROS message called MyMessage with a field for a string, called name, and a field for an array of float64, called contents. Edit files such as CMakeLists.txt to ensure your message is compiled and available for use.


### Ending The Lesson

Recommended: 15 minutes 

Implement the IR publisher, and then see the results on the screen.

TODO: A high-schooler friendly template that they can go into a loop in which they can put their existing IR sensor code, set the loop rate, and explain the importance of rate consistency, limiting, and minimum. Rostopic echo their newly published messages


**Useful Resources and References**

[Python Loops](https://www.learnpython.org/en/Loops) 