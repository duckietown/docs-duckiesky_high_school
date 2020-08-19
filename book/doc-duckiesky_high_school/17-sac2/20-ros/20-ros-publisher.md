# Creating a ROS Publisher {#sac2-ros-publisher status=ready}

<div class='requirements' markdown='1'>

Requires: 

**Hardware** - 

- basestation

- Build Parts 1 and 2 completed

**Previous Lesson** - [Introduction to ROS](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/sac2_ros_intro.html)

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

Teachers can write a DO NOW on the board for students to open the python file that read and print sensor values written in [the sensor lesson](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/sac2_sensing_reading.html).


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 5 minutes

Review the code of reading sensor values.

See: **Hook**

Q: How should we make this information useful to other parts of the robots?

A: ROS!

### Main Lesson

Recommended: 30 minutes

Teacher uses [this tutorial](https://wiki.ros.org/ROS/Tutorials/CreatingMsgAndSrv) to explain how to creat ROS messages. 

Two types of messages that might need more explaining: 

1. **Header:** The header contains a timestamp and coordinate frame information that is commonly used in ROS

2. **Float:** More precise measurement than integers

Then, students follow the teacher step by step to create a ROS publisher:

1. Import the ROS python library and the needed message types.

See also: Add the line 'import rospy' to the top of the program.

See also: Add the line 'from std_msgs.msg import Float32' to the top of the program.

2. Create a publisher and explain the three message types () involved.

See also: Type 'distance_publisher = rospy.Publisher('distance', Float32, queue_size=1)' right before the calibration function 'adc_to_distance'.

3. Create an infrared sensor node.

See also: Type "rospy.init_node('infrared_node')" in the next line.

4. Publish the message in the previously created while loop.

See also: Type "distance_publisher.publish(Float32(distance))" right after the line 'print(distance)' in the while loop, assuming that name of the local variable that represents the output of the 'adc_to_distance' function is named 'distance'. If not, adjust the code accordingly.

5. Change the structure of the while loop to a ROS manner. (This step is just a change of syntax)

See also: Change the top of the loop from 'while True:' to 'while not rospy.is_shutdown():'

See also: Change the bottom of the loop from 'time.sleep(1)' to 'rospy.sleep(1)'.

### Ending The Lesson

Recommended: 15 minutes 

Time to visualize our progress!

Open up a new terminal, start up roscore by typing 'roscore' and hit enter in order to get nodes running.

Navigate back to the previous terminal, run the code. We can see it is still printing sensor values.

Q: What about the publisher we just created?

A: Open another terminal, run 'rostopic list' and see the 'distance' topic we just created. Then we run 'rostopic info distance' to see the message type (Float32) and where it is published from (infrared_node). Lastly, run 'rostopic echo distance' to show the message we just created in the terminal! (It should be Float32 messages with data label)

TODO: Intro to the web UI. Run their IR publisher and see the results onscreen.

**Useful Resources and References**

[Python Loops](https://www.learnpython.org/en/Loops)

[ROS Tutorial on Creating Publisher and Subscriber](https://wiki.ros.org/ROS/Tutorials/WritingPublisherSubscriber%28python%29)
