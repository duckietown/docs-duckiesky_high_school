# Intro to ROS {#sac2-ros-intro status=ready}

<div class='requirements' markdown='1'>

Requires: 

**Hardware** - basestation 

**Previous Lesson** - Beginning of [Unit - Sensors, Actuators, and Control Part 2](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy/duckiesky_high_school/out/sac2.html)


Result: 

**Knowledge** - 

- Definition and purpose of robot middleware

- Basic ROS components and vocabulary: topic, message, publisher, subscriber, node, workspace


**Skills** -

- List and echo ROS topics

- Create a catkin workspace

</div>

## Introduction to ROS 


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)

_NGSS: HS - ETS1 - 2_: Design a solution to a complex real-world problem by breaking it down into smaller, more manageable problems that can be solved through engineering.

_ISTE: 1. d._: Understand the fundamental concepts of technology
operations, demonstrate the ability to choose, use and troubleshoot current technologies and are able to transfer their knowledge to explore emerging technologies.


### Assessments and Evidence of Understanding

Students will be able to undertand what ROS is and make a catkin workspace by the end of the lesson. 


### AGENDA (Brief Summary of Activities)

5 mins: Introducing ROS 

45 mins: Reviewing important ROS concepts and commands 

10 mins: Making a catkin workspace 

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Teacher Materials**

Basestation, a projector (if needed)

**Classroom Set Up**

Teachers can write a DO NOW on the board for students to set up their basestations.

## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 5 minutes

See: **Hook**

Teachers use this [link](https://docs.duckietown.org/daffy/opmanual_sky/out/software_architecture_intro.html) to:

1. Give students a sense of the structure of a software diagram. 

2. Illustrate the challenges of software engineering in robotics 

    - Lots of sensors and actuators, and they need to communicate with each other (even in this diagram, not many sensors and actuators but the connections are still fairly complicated)
    
    - Processes might live on different computers to spread the computing load
    
    - Many software modules need to work together (Need to manage their dependencies)


### Main Lesson

Recommended: 45 minutes

Present our solution to the challenges above: ROS (Robot Operating System).

**Official Introduction of ROS**

"ROS is an open-source, meta-operating system for your robot. It provides the services you would expect from an operating system, including hardware abstraction, low-level device control, implementation of commonly-used functionality, message-passing between processes, and package management. It also provides tools and libraries for obtaining, building, writing, and running code across multiple computers." (http://wiki.ros.org/ROS/Introduction)

**In Short**: ROS aims to support **code reuse** in robotics research and development.

Q: What are the benefits of reusing codes?

A:

    - **Wikipedia Verision** "Modular programming is a software design technique that emphasizes separating the functionality of a program into independent, interchangeable modules, such that each contains everything necessary to execute only one aspect of the desired functionality." (https://en.wikipedia.org/wiki/Modular_programming)
 
    - **In Short**: Easy to read, easy to test, easy to reuse, easy to maintain, etc.

    To help students understand this, teachers might draw a comparison to reading and writing a book like [this](https://www.durhampriory.ac.uk/colour-your-own-medieval-manuscript-part-5/) versus a book like [this](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/index.html)

#### **Overview of important ROS concepts** 

**ROS master:** A node that every other node register in order to communicate with each other. It is created by running roscore command (Detailed: [http://wiki.ros.org/Master](http://wiki.ros.org/Master))

**ROS nodes:** ROS nodes are programs that communicate with other programs via publishing and/or subscribing to ROS topics. (Detailed: [http://wiki.ros.org/Nodes](http://wiki.ros.org/Nodes))

**Messages:** The information that is communicated between nodes. Messages are standardized, which means that certain message types have certain fields. For example, “ROS pose message” has two parameters: position and orientation. They are message types themselves, which contain their own parameters. ([http://docs.ros.org/melodic/api/geometry_msgs/html/msg/Pose.html](http://docs.ros.org/melodic/api/geometry_msgs/html/msg/Pose.html)) This makes communication between programs a lot easier (link to the modular programming above). You can even create your own message types!

**ROS Topics:** Topics are what ROS messages are published and subscribed to. (Detailed: [http://wiki.ros.org/Topics](http://wiki.ros.org/Topics))

**Publishers:** Publishers are used to publish specific message types to specific topics.

**Subscribers:** Subscribers are used to read the messages being published to a ROS topic.

Better: Print out all of the topics running by entering “rostopic list” into a free window after running ‘screen -c pi.screenrc’ on your drone. Have messages that are being published to a topic printed out by navigating to an empty window in the screen and entering “rostopic echo [topic_name]”. For example, if you wanted to see the data coming from the infrared sensor, you could enter “rostopic echo /pidrone/infrared”

<div class='requirements' markdown='1'>

**Important ROS Commands:**

_roslaunch_: roslaunch is a tool for easily launching multiple ROS nodes locally and remotely via SSH, as well as setting parameters on the Parameter Server. (Detailed: [http://wiki.ros.org/roslaunch](http://wiki.ros.org/roslaunch))

_roscd_: roscd allows you to change directories using a package name, stack name, or special location. (Detailed: [http://wiki.ros.org/rosbash#roscd](http://wiki.ros.org/rosbash#roscd))

_rostopic_: rostopic contains the rostopic command-line tool for displaying debug information about ROS Topics, including publishers, subscribers, publishing rate, and ROS Messages. (Detailed: [http://wiki.ros.org/rostopic](http://wiki.ros.org/rostopic))

</div>


TODO: a flow chart of controlling a LED with IR sensor 


### Ending The Lesson

Recommended: 10 minutes

Better: make a catkin workspace following this [link](http://wiki.ros.org/ROS/Tutorials/InstallingandConfiguringROSEnvironment).


**Useful Resources and References**

[ROS overview](https://docs.duckietown.org/daffy/opmanual_sky/out/software_architecture_assignment.html)

[ROS Wiki](http://wiki.ros.org)
