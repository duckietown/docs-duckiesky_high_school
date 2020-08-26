# Blinking an LED {#computing-pi-led status=ready}

<div class='requirements' markdown='1'>

Requires: 

**Previous lesson** - 

- [Networking](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/pi_networking.html)

- [Bash](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/computing_pi_bash.html)

**Hardware** - 

- Basestation

- Build Part 1 completed

Result: 

**Knowledge** - Definition and purpose of Raspberry Pi GPIO

**Skills** -

- Read the GPIO pin chart for the Raspberry Pi

- Write a bash script to blink their LED

</div>

## Blinking an LED


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)

_NGSS: HS - ETS1 - 2_: Design a solution to a complex real-world problem by breaking it down into smaller, more manageable problems that can be solved through engineering.

_ISTE: 1. d._: Understand the fundamental concepts of technology
operations, demonstrate the ability to choose, use and troubleshoot current technologies and are able to transfer their knowledge to explore emerging technologies.


### Assessments and Evidence of Understanding

Students write a bash script to make the led that they've soldered blink.

### AGENDA (Brief Summary of Activities)

5 min: Basestation Setup

20 min: Scripts and REPLS Lesson

35 min: Writing a Bash Script

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Classroom Set Up**

Teacher can write a DO NOW on the board for students to set up their basestations.


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 5 minutes

See: **Hook**

Teachers can talk about the following or their own.

-  This will be a lesson for the student on creating a bash script that will blink the LED on their drone. It is important to understand scripts as they will come up when continuing with programming.


### Main Lesson

Recommended: 20 minutes

1. Teachers cover what a REPL (Read–eval–print loop) is and what a script is

- Read–eval–print loop: a simple interactive computer programming environment that takes **single** user inputs, executes them, and returns the result to the user

- Script: a programming language for a special run-time environment that automates the execution of tasks; the tasks could alternatively be executed **one-by-one** by a human operator.

See: Difference - script saves the commands to be run sequentially in the future

2. Teachers speak on Pi GPIO numbering

- On the Raspberry Pi, Pin can be defined in two ways, using the **GPIO Board** and **GPIO BCM** methods.

- **GPIO BCM** refers to the default pin of the Broadcom SOC channel chip.

- **GPIO Board** refers to the naming on the Raspberry Pi board. This is the numbering on the Pi Hat


### Writing a Bash Script

Recommended: 35 minutes

Better: Instructors show how to make and run bash scripts, delays, printing, pin setting by leading students write a bash script to make the led that they've soldered blink

[See the student book for details](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school_student/docs-duckiesky_high_school_student/branch/daffy-develop/duckiesky_high_school_student/out/computing_pi_led.html)

**Useful Resources and References**

1. [More information on REPLs](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop#:~:text=A%20read%E2%80%93eval%E2%80%93print%20loop,REPL%20environment%20is%20executed%20piecewise.)
2. [More information on scripts](https://techterms.com/definition/script)
3. [More information on blinking an LED](https://www.teknotut.com/en/first-raspberry-pi-project-blink-led/)
