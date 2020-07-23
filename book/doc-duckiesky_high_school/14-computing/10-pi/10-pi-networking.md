# Networking {#pi-networking status=ready}

<div class='requirements' markdown='1'>

Requires: Hardware: Basestation, Build Part 1 completed

Result: Knowledge: 7 layers of network abstraction, IP and MAC addresses, Definition of the computer terminal/shell, Definition and use of SSH; Skills: SSH into a remote computer

</div>

## Networking


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)

_ISTE: 1. d._: Understand the fundamental concepts of technology
operations, demonstrate the ability to choose, use and troubleshoot current technologies and are able to transfer their knowledge to explore emerging technologies.


### Assessments and Evidence of Understanding

Students will be able to connect to the Pi over ssh and verify its the right one by running an existing bash script to blink the built-in LED.

### AGENDA (Brief Summary of Activities)

5 min: Basestation Setup

35 min: Networking Lesson

25 min: Pi SSH and Led Blinking Script

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

For Students: Basestation, Current Drone Build

For Teachers: Basestation


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 5 minutes

Pre Class:

Do Now: Teacher writes on the board for students to prepare their basestations

Hook: Teachers can talk about the following or their own.

-  This will be a lesson for the student on the basics of Networking and Computer Terminals. It is important to comprehend networking to understand the basis of how computers connect with each other and to know computer terminal details to understand how computers can be controlled.


### Main Lesson

Recommended: 35 minutes

- Teachers should cover the basics of the 7 layers of network abstraction and IP/MAC addresses

TODO: Input a video/details based on the updated teacher training material on Networking. [Here](https://edge.edx.org/courses/course-v1:BrownX+CS195R+2018_T1/courseware/0e3596880ec446d8ab63df427e02e9c4/56017f6d3048461b90466ad229ac8df6/?activate_block_id=block-v1%3ABrownX%2BCS195R%2B2018_T1%2Btype%40sequential%2Bblock%4056017f6d3048461b90466ad229ac8df6) is the college course video on Networking.

- Teachers define what a computer terminal and shell is

See also: A shell is a programming language that takes input and gives the input to the computer and operating system to analyze and perform the task that the input asks for. 

See also: A terminal is a program that allows the user to interact with the shell.

- Teachers define SSH and what it is used for 

See also: SSH (Secure Shell) is a method that allows a user to remotely log in from one computer/device to another. We will be utilizing SSH to connect to our Pi. 

### Pi SSH and Led Blinking Script

Recommended: 20 minutes

Exercise: Connect to the Pi over ssh, verify its the right one by running an existing bash script to blink the built-in LED, change the SSID. 

TODO: Commands should be very explicit and minimal, they don’t have experience with bash or editors yet (may want to automate setting the WiFi SSID even, e.g. guided setup process)

TODO: Make step by step 

**Useful Resources and References**

1. [Shell and Terminal Details](http://linuxcommand.org/lc3_lts0010.php)
2. [SSH Details](https://www.ssh.com/ssh/protocol/)