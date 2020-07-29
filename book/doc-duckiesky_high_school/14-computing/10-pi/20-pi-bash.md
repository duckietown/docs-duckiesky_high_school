# Bash {#computing-pi-bash status=ready}

<div class='requirements' markdown='1'>

Requires: 

**Hardware** - 

- Basestation 

- Drone (Build Part 1 completed)

**Previous lesson** - [Networking](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/pi_networking.html) 


Result: 

**Knowledge** - 

- Computer file structure

- Essential bash commands


**Skills** - 

- Navigating computer directories in the terminal

- Editing files through the command line

</div>

## Bash


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)

_NGSS: HS - ETS1 - 2_: Design a solution to a complex real-world problem by breaking it down into smaller, more manageable problems that can be solved through engineering.

_ISTE: 1. d._: Understand the fundamental concepts of technology
operations, demonstrate the ability to choose, use and troubleshoot current technologies and are able to transfer their knowledge to explore emerging technologies.



### Assessments and Evidence of Understanding

By the end of this lesson, students should be able to complete the below Bash terminal task.

### AGENDA (Brief Summary of Activities)

5 min: Basestation Setup

40 min: Bash Lesson

15 min: Bash Terminal Task

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

-  This will be a lesson for the student on Bash scripting and the Shell. It is important to learn how to utilize a shell as it is the introduction to the inner processes of the operating system.
- Conceptually connect Bash to Markdown in the sense that the computer is being affected via text: the purpose of Bash is to “control” the computer vs whereas Markdown is utilized for the purpose of "visual layout"

### Main Lesson

Recommended: 40 minutes

Teachers can either use a live demonstration via a projector using the Pi over ssh or utilize an online Bash tutorial (see _Useful Resources and References_ below) that the students can work through. 

By the end of the Main Lesson, students should be able to:

-  See basic information in the terminal and navigate the file system (pwd, ls, cd)
-  Creating, moving, and removing files and directories (touch, mv, cp, rm, mkdir, rmdir)
-  Using a carat to output to a file (e.g. "echo 'foo' >bar.txt")
- Printing output in the terminal (echo, cat)
-  Clearing terminal output and exiting (clear, exit)

TODO: Using a CLI Text Editor

### Ending The Lesson

Recommended: 15 minutes

Better: Exercise: Students should do the following steps with Bash commands to test out their knowledge of the terminal. They can do this through the Pi over ssh:

-  Print the directory they are currently working in 

See also: "pwd"

-  Create a directory named "Hello"

See also: "mkdir 'Hello'"

-  Check that the directory has been created by listing the current files/directories

See also: "ls"

-  Enter into the directory 

See also: "cd Hello"

-  Create a text file called "World.txt" within the "Hello" directory with the contents "Hello World" within it

See also: "echo 'Hello World' >World.txt"

-  Print the contents of the "World.txt" file

See also: "cat World.txt"

-  (Optional) Have the teacher check off that the "Hello" directory has a "World.txt" file with the contents of "Hello World" in it
-  Delete the "World.txt" file

See also: "rm 'World.txt'"

-  Leave the directory

See also: "cd .."

-  Delete the directory along with its contents

See also: "rmdir 'Hello'"

-  Check that the directory has been deleted by listing the current files/directories

See also: "ls"

-  (Optional) Have the teacher check off the outputs of the terminal

**Useful Resources and References**

1. [Shell Tutorial 1](https://www.youtube.com/watch?v=cBokz0LTizk)
2. [Shell Tutorial 2](http://linuxcommand.org/lc3_learning_the_shell.php)
3. [Bash Command Overview](https://www.educative.io/blog/bash-shell-command-cheat-sheet)
4. [Bash Shell Script Tutorial](https://www.youtube.com/watch?v=F-gskSl4pwQ)

