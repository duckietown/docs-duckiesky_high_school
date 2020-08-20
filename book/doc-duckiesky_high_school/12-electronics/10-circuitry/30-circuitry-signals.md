# Signals and Connections {#electronics-circuitry-signals status=ready}

<div class='requirements' markdown='1'>

Requires: 

**Hardware** - Uncompleted drone kit
**Previous Lesson** - Voltage, Current, and Resistance

Result: 

**Knowledge** - Ability to identify different electrical connections used on the drone and the advantages of each, know the definition of signals and where they are used on the drone, understand the differences between and varying advantages of analog and digital signals, understand that values, properties, and concepts can be encoded into numbers and the purpose thereof, and know advantages of binary as a number system.

</div>

## Lesson Title
Signals and Connections

### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)


### Assessments and Evidence of Understanding

By the end of this lesson, student should be able to understand analog and digital signals and examples of each, as well as be abe to translate numbers into binary.

### AGENDA (Brief Summary of Activities)

- Intro (5 min)

- Main Lesson (60 min)

- Ending the Lesson (15 min)

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

For Students: Uncompleted drone kit

For Teachers: Presentaion medium for lesson (i.e. whiteboard, powerpoint slide)

## SCRIPT OF TEACHING AND LEARNING ACTIVITIES

### Intro

The teacher should open this lesson with an explaining that there are two types of signals on the drone. (Analog and Digital) Have the students guess where these signals could be located on the drone. If no one is able to give an answer, lead into the lesson saying that these signals are important to know and are intigral to the drone's flight.

### Main Lesson

Recommended: 60 minutes

__Electrical connections (30min)__

Briefly explain: crimping, connectors, splicing, soldering, and introduce PCBs as 'home bases' for connections

Exercise: Point out soldered connections, pull out different connectors used in the drone (e.g. from battery sense to Pi GPIO to XT-60), compare the number of pins, current capacity, etc.

Use this section as an opportunity to motivate why students need to learn to solder. This will transition the course to the next module, Soldering!

Besides power, electricity can also be used to convey information...

__Analog signals (10min)__

Information can be transmitted through electricity:

- Encoding in voltage: use an IR sensor as an example

- Encoding in frequency: use WiFi as an example

- Noise, which can come from various sources, can distort or block the information transmittion done by the former

After describing frequency and voltage, have a group brainstorm on what other electronics and sensors could have a voltage or frequency signal. (Use examples from above to lead the discussion)

__Digital signals (20 min)__

Introduce how numbers can represent anything, e.g. letters (a=1, b=2, etc...)

Exercise: devise a way to represent things as one or more numbers! For example, physical properties (distance, colors, volume, etc...), other symbols, music: notes, chords, progressions, pieces, scales/modes,  intervals, etc…, sports plays, games (cards, stats, etc...)

Our number system uses base-10 (10 symbols) to represent numbers, but there are many other ways to convey information!

There’s no reason we have to use 10 symbols, you can get away with just 2 -- binary! (or other numbers, eight: octal, sixteen: hexadecimal) Show ascii table with binary and decimal. [ascii table](https://www.rapidtables.com/code/text/ascii-table.html)

To understand binary, here is a short activity to do: [activity link](https://docs.google.com/document/d/1QnD9khmPUz1az3ZLc5L8vavR6lU0uScspotRhORnHxE/edit) [video explaination](https://www.youtube.com/watch?v=wDWj1a4BZjQ)

Assign the students to convert a few numbers of the teacher's choosing on their flippydo.

The teacher should discuss how digits can be represents as ranges of voltages with an undefined zone in between (used as a break). Also, mention having only two simplifies the circuitry, reduces effects of noise

- Binary can be transmitted in parallel and over time, which are two ways to represent more than one symbol, sacrificing either complexity or time

- Mention electrical vs timing vs content specifications of signals (discussing this will set up for future networking lessons with higher levels of abstraction)

### Ending The Lesson

Recommended: 15 minutes

Give students binary game link, and challenge them to hit the highest level! 

[https://games.penjee.com/binary-bonanza/](https://games.penjee.com/binary-bonanza/)

**Useful Resources and References**

[https://docs.google.com/document/d/1QnD9khmPUz1az3ZLc5L8vavR6lU0uScspotRhORnHxE/edit](https://docs.google.com/document/d/1QnD9khmPUz1az3ZLc5L8vavR6lU0uScspotRhORnHxE/edit)

[https://games.penjee.com/binary-bonanza/](https://games.penjee.com/binary-bonanza/)

[https://www.rapidtables.com/code/text/ascii-table.html](https://www.rapidtables.com/code/text/ascii-table.html)

[Glossary](https://docs.google.com/document/d/1LJzESfH8VnLDAitNTwwa-iDZs-zY-KM2v1EuWFoLz6A/edit?usp=sharing)
