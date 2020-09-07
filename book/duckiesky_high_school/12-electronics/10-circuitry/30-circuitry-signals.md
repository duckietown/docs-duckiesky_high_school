# Signals and Connections {#electronics-circuitry-signals status=ready}

[Student version](+duckiesky_high_school_student#electronics-circuitry-signals)

<div class='requirements' markdown='1'>

Requires: 

**Hardware** - 

- Uncompleted drone kit

**Previous Lesson** - [Voltage, Current, and Resistance](https://docs.duckietown.org/daffy/downloads/duckiesky_high_school/docs-duckiesky_high_school/branch/daffy-develop/doc-duckiesky_high_school/out/electronics_circuitry_voltage.html)

Result: 

**Knowledge** - 

- Ability to identify different electrical connections used on the drone and the advantages of each

- Know the definition of signals and where they are used on the drone

- Understand the differences between and varying advantages of analog and digital signals

- Understand that values, properties, and concepts can be encoded into numbers and the purpose thereof, and know advantages of binary as a number system.

</div>

## Signals and Connections

### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)

_ISTE: 1. d._: Understand the fundamental concepts of technology
operations, demonstrate the ability to choose, use and troubleshoot current technologies and are able to transfer their knowledge to explore emerging technologies.

### Assessments and Evidence of Understanding

By the end of this lesson, student should be able to understand analog and digital signals and examples of each, as well as be abe to translate numbers into binary.

### AGENDA (Brief Summary of Activities)

- 5 min: Introduction 

- 20 min: Electrical Signals

- 10 min: Analog signals

- 20 min: Digital signals 

- 15 min: Short online game  

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Teacher Materials**

Optional presentaion medium for lesson (i.e. whiteboard, powerpoint slide). 

## SCRIPT OF TEACHING AND LEARNING ACTIVITIES

### Introducing the Lesson 

Recommended: 5 minutes 

**Hook:** 

- The teacher should open this lesson with an explanation that there are two types of signals on the drone (Analog and Digital).  

Better: Exercise: Have the students guess where these signals could be located on the drone. If no one is able to give an answer, lead into the lesson saying that these signals are not only intigral to the drone's flight, but also integral to know in the field of robotics. 

### Main Lesson

Recommended: 50 minutes

__Electrical connections (20min)__

Briefly explain: crimping, connectors, splicing, and soldering. Introduce PCBs as _'home bases'_ for connections in the drone. 

Better: Exercise: Point out soldered connections and pull out different connectors used in the drone (e.g. from battery sense to Pi GPIO to XT-60), compare the number of pins, current capacity, etc.

See also: Use this section as an opportunity to motivate why students need to learn to solder. This will transition the course to the next module, Soldering!


__Analog signals (10min)__

Besides power, electricity can also be used to convey information...Information can be transmitted through electricity:

1. Encoding in _voltage_: use an IR sensor as an example. 

2. Encoding in _frequency_: use WiFi as an example. 

Note: _Noise_, which can come from various sources, can distort or block the information transmittion done by the former.

Better: Exercise: After describing frequency and voltage, have a **group brainstorm** on what other electronics and sensors could have a voltage or frequency signal. (Use examples from above to lead the discussion). 

__Digital signals (20 min)__

Introduce how numbers can represent anything, e.g. letters (a=1, b=2, etc...)

Better: Exercise: Devise a way to represent things as one or more numbers! For example, physical properties (distance, colors, volume, etc...), other symbols, music (notes, chords, progressions, pieces, scales/modes,  intervals, etc.), sports plays, games (cards, stats, etc.). 

Our number system uses base-10 (10 symbols) to represent numbers, but there are many other ways to convey information!

There’s no reason we have to use 10 symbols, you can get away with just 2 -- binary! (or other numbers, eight: octal, sixteen: hexadecimal) Show [ascii table](https://www.rapidtables.com/code/text/ascii-table.html) with binary and decimal. 

Better: Exercise: To understand binary, here is a [short activity](https://docs.google.com/document/d/1QnD9khmPUz1az3ZLc5L8vavR6lU0uScspotRhORnHxE/edit) to do with this [video explaination](https://www.youtube.com/watch?v=wDWj1a4BZjQ). Assign the students to convert a few numbers of the teacher's choosing on their flippydo.

Using the resources below and in the student book, teachers should discuss: 

- How digits can be represented as ranges of voltages with an undefined zone in between (used as a break). Also, mention having only two symbols (binary) simplifies the circuitry and reduces effects of noise. 

- Binary can be transmitted in parallel and over time, which are two ways to represent more than one symbol, sacrificing either complexity or time. 

- Mention electrical vs timing vs content specifications of signals (discussing this will set up for future networking lessons with higher levels of abstraction). 

### Ending The Lesson

Recommended: 15 minutes

Better: Give students this [binary game link]((https://games.penjee.com/binary-bonanza/)), and challenge them to hit the highest level! 


**Useful Resources and References**

1. [Flippy Do Activity](https://docs.google.com/document/d/1QnD9khmPUz1az3ZLc5L8vavR6lU0uScspotRhORnHxE/edit)

2. [Binary Bonanza Game](https://games.penjee.com/binary-bonanza/)

3. [ASCII Table](https://www.rapidtables.com/code/text/ascii-table.html)

4. [Glossary](https://docs.google.com/document/d/1LJzESfH8VnLDAitNTwwa-iDZs-zY-KM2v1EuWFoLz6A/edit?usp=sharing)
