# Networking {#computing-pi-networking status=ready}

[Student version](+duckiesky_high_school_student#computing-pi-networking)

<div class='requirements' markdown='1'>


Requires: 

**Hardware** - Basestation   
**Previous lesson** - Build Part 1


Result: 

**Knowledge** - 

- 7 layers of network abstraction
- IP and MAC addresses
- Definition of the computer terminal/shell
- Definition and use of SSH


**Skills** - Basic Text Editor and VSCode skills

</div>


## Networking


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)

_ISTE: 1. d._: Understand the fundamental concepts of technology
operations, demonstrate the ability to choose, use and troubleshoot current technologies and are able to transfer their knowledge to explore emerging technologies.


### Assessments and Evidence of Understanding

By the end of this lesson, students should be able to connect to the Pi and verify its the right one by running an existing bash script to blink the built-in LED.

### AGENDA (Brief Summary of Activities)

10 min: Basestation Setup

30 min: Networking Lesson

25 min: Pi Connection and Led Blinking Script

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Teacher Materials:**

Basestation, a projector (optional) 

**Classroom Setup:**

Teachers can write a DO NOW on the board for students to set up their basestations.


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 10 minutes

**Hook:**

-  This will be a lesson for the student on the basics of Networking and Computer Terminals. It is important to comprehend networking to understand the basis of how computers connect with each other and to know computer terminal details to understand how computers can be controlled.
    - One robot can be made up of one or more computers that need to coordinate with each other, and robots may need to communicate with external systems; for these purposes, networking is essential. 
- (Optional) Networking should be applied to how the drone communicates with the basestation. To do this, teachers can start class with a small discussion instead of or in addition to the above hook. The following questions are potential discussion points:

Q: What are some other robots or devices in your daily life that have to communicate with each other? How do you think they do this? 

Q: How will we control our drone? From what? 

Q: What features of the communication channel between our basestation and the drone could be important? Wireless connectivity, latency (delay between communications), throughput (maximum volume of communications)?

### Main Lesson

Recommended: 40 minutes

- Teachers should cover the basics of the 7 layers of network abstraction and IP/MAC addresses as outlined in the student book.
 <!--   - (Optional) Students should fill out worksheet during process. -->
- Teachers define (and potentially demonstrate) what a computer terminal and shell is as outlined in the student book.
- Teachers define SSH and what it is used for as outlined in the student book.


### Ending The lesson

Recommended: 10 minutes

Better: Exercise: Teachers should have students connect to the Pi via web browser and explain each of the components of the text editor.

<!-- Exercise: Teachers should have students connect to the Pi via web browser, verify its the right one by running an existing bash script to blink the built-in LED.

 (Optional) If students are able to get through this section with additional time remaining, they can work towards connecting to the Pi via SSH.
    - SSH (Secure Shell) is a method that allows a user to remotely log in from one computer/device to another. Typically, we would be utilizing SSH to connect to our Pi, but 
 -->


Better: Optional Exercise: Teachers can attempt to follow our [old build instructions](https://docs.duckietown.org/DT19/opmanual_sky/out/build_phase5.html) to connect to the drone over SSH; if you are able to, you can try to have students follow the similar process. These instructions are not too detailed and are outdated, so it may take additional troubleshooting on your end to figure this out (additionally this may not be compatible on chromebook). 

**Useful Resources and References**

1. [Networking edX Lecture](https://edge.edx.org/courses/course-v1:BrownX+CS195R+2018_T1/courseware/0e3596880ec446d8ab63df427e02e9c4/56017f6d3048461b90466ad229ac8df6/?activate_block_id=block-v1%3ABrownX%2BCS195R%2B2018_T1%2Btype%40sequential%2Bblock%4056017f6d3048461b90466ad229ac8df6)
2. [Shell and Terminal Details](http://linuxcommand.org/lc3_lts0010.php)
3. [SSH Details](https://www.ssh.com/ssh/protocol/)