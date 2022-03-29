# Drone Localization {#localization-camera-localization status=ready}

[Student version](+duckiesky_high_school_student#localization-camera-localization)


<div class='requirements' markdown='1'>


Requires: test 1 to show interns book edits

**Hardware** -    

- Basestation
- Completed Build Part 4 

**Previous lesson** - [Comparing Images](#localization-camera-images)


Result: 

**Knowledge** - Definition and purpose of localization


**Skills**

- Make a map for the drone to localize over
- Move the drone to global positions within the map


</div>

## Drone Localization

### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)



### Assessments and Evidence of Understanding

By the end of this lesson, students should be able to ...

### AGENDA (Brief Summary of Activities)

X min: <!--insert time slot 1 (add or delete these as needed)-->

X min: <!--insert time slot 2 (add or delete these as needed)-->

X min: <!--insert time slot 3 (add or delete these as needed)-->

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Teacher Materials:**

**Classroom Setup:**

Teachers can write a DO NOW on the board for students to ...

## SCRIPT OF TEACHING AND LEARNING ACTIVITIES


### Introducing The Lesson

Recommended: 10 -15 minutes

**Hook:**

In autonomous mobile robotics estimate of position is crucial. If you covered your eyes while standing in a room your other four senses in your body would help you to survey your surroundings. Robots how ever do not pocess senses like humans but we can simulate them with sensors and cameras. For example a self driving car has sensors and mounted cameras as an essential component that collect data to let the computer know a rough estimation of the machines surroundings, like if another car were infront of it. This process is also known as **localization**.

### Main Lesson

Recommended: 45 minutes

In order for the drone to use localization you will be using two algorithms on the PiDrone **Monte Carlo** and **Fast S.L.A.M.**. These two algorithms are desgined to target specific drone flying scanrios; scenario one (Monte Carlo) the drone is provided with a map like the one implemented into this lesson, and scenario two where the drone would use its sensors to simultaniously develope a map of its enviroment (Fast Slam). 

For the purpose of this course we will be using the Monte Carlo localization (M.C.localization) which refers to the priniciple of using random sampling to model a complicated unavoidable process. In a more in depth analysis the M.C. localization is a very popular particle filter algorithm. In every new frame captured by the drones camera the filter will apply a motion prediction to adjust each possible position of the drone. At each movement correction the motion predictions will be resampled until it finds a match.**Do not worry if you still feel uneasy on the concept, we recomend doing the localization activities for better understanding**

Better: Exercise: if a jigsaw puzzle is available, otherwise with pictures of one, give students a few pieces and let them try to figure out where their pieces come from by looking at the finished puzzle picture on the box.

The drones primary sensor is the pi camera facing downward. To complete understanding of how the particle filters allow localization we will take a closer look at the process the camera extracts features and shapes to determine its position. To process information from the camera we will use a open source computer vision library callled OpenVC. From a computers perspective a **feature** is a point of interest. Unlike humans that are able to identify a point of interest on a picture like; texture, patterns, color, or what ever may call our attention, a computer needs a precise definition of the point of interest. Features can also be defined as areas in an image where the pixel intensities change rapidly. Once a feauture is extracted the OpenCV will give us a keypoint and descriptor for each feature with its corresponding (x,y) coordinates.

### Getting Set Up 

1. place your directory in the /ws/src folder on your drone.

2. you should find "package.xml" and "CMakeLists.txt" which you need to modify your package. 

3. On line 3 of "package.xml" you need to replace the default github name with your github name so it matches the nam in your directory. Do the same on line 2 of "CMakeLists.txt".

4. navigate to the /ws folder and run the following line of code.

**catkin --pkg project-localization-slam-2019-yourGithubName**

(this allows your package to be ros-runnable from the pidrone_pkg. This is a one time step) 

### Using the Localization 

**Coming Soon**

### Vocabulary  

Localization: the fact of being or becoming located or fixed in a particular place.

S.L.A.M. (acronym): simultaneous localization and mapping problem



### Ending The Lesson

Recommended: 10 - 15 minutes


Better: Exercise: Have the drone use it to localize and fly to different targets.


**Useful Resources and References**


1. [Oxford Dictionary](https://onlinelibrary.wiley.com/doi/full/10.1002/047134608X.W8318) - Definition of localization
