# Creating a ROS Publisher {#sac2-ros-publisher status=ready}

[Student version](+duckiesky_high_school_student#sac2-ros-publisher)

<div class='requirements' markdown='1'>

Requires: 

**Hardware** - 

- basestation

- Build Parts 1 and 2 completed

**Previous Lesson** - [Introduction to ROS](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy/duckiesky_high_school/out/sac2_ros_intro.html)

Result: 

**Knowledge** - Python loops 

**Skills** - 

- Create custom ROS messages

- Create ROS publishers

- Use ROS commands


</div>

## Creating a ROS Publisher


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)

_NGSS: HS - ETS1 - 2_: Design a solution to a complex real-world problem by breaking it down into smaller, more manageable problems that can be solved through engineering.

_NGSS: HS - PS4 - 2_: Evaluate questions about the advantages of using a digital transmission and storage of information.

_ISTE: 5. c._: Break problems into component parts, extract key information, and develop descriptive models to understand complex systems or facilitate problem-solving


### Assessments and Evidence of Understanding


### AGENDA (Brief Summary of Activities)


### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Teacher Materials**

Basestation, drone build

**Classroom Set Up**

Teachers can write a DO NOW on the board for students to open the python file that read and print sensor values written in [the sensor lesson](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy/duckiesky_high_school/out/sac2_sensing_reading.html).


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 5 minutes

Review the code of reading sensor values in the [student book](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school_student/docs-duckiesky_high_school_student/branch/daffy-develop/duckiesky_high_school_student/out/sac2_ros_publisher.html).

See: **Hook**

Q: How should we make this information useful to other parts of the robots?

A: ROS!

### Main Lesson

Recommended: 30 minutes

Teacher uses [this tutorial](https://wiki.ros.org/ROS/Tutorials/CreatingMsgAndSrv) to explain how to creat ROS messages. 

Two types of messages that might need more explaining: 

1. **Header:** The header contains a timestamp and coordinate frame information that is commonly used in ROS

2. **Float:** More precise measurement than integers

Then, students follow the teacher step by step to create a ROS publisher, which is detailed in the [student book](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school_student/docs-duckiesky_high_school_student/branch/daffy-develop/duckiesky_high_school_student/out/sac2_ros_publisher.html).

### Ending The Lesson

Recommended: 15 minutes 

Time to visualize our progress!

Open up a new terminal, start up roscore by typing `roscore` and hit enter in order to get nodes running.

Navigate back to the previous terminal, run the code. We can see it is still printing sensor values.

Q: What about the publisher we just created?

A: Open another terminal, run `rostopic list` and see the `distance` topic we just created. Then we run `rostopic info distance` to see the message type (Float32) and where it is published from (infrared_node). Lastly, run `rostopic echo distance` to show the message we just created in the terminal! (It should be Float32 messages with data label)

**Useful Resources and References**

[Python Loops](https://www.learnpython.org/en/Loops)

[ROS Tutorial on Creating Publisher and Subscriber](https://wiki.ros.org/ROS/Tutorials/WritingPublisherSubscriber%28python%29)
