# Lesson 3: Intro to Ethics {#introduction-relevance-ethics status=ready}

<div class='requirements' markdown='1'>

Requires: No previous lessons are required.

Result: Students will be able to learn about what ethics is and why it is important. They will also be introduced to ethical challenges in computer science and engineering including algorithmic bias, accessibility concerns, and human job security. 

</div>

## Ethics


### STANDARDS: Next Generation Science Standards (NGSS) and International Society for Technology in Education (ISTE)



### Assessments and Evidence of Understanding


### AGENDA (Brief Summary of Activities)
5 min: Introduction to the lesson. What is ethics and why it is important. 

40 min: Introducing students to specific ethical implications of technological and engineering systems. 

### Differentiation _(strategies for grouping, ELL, and inclusion)_


### Advanced preparation/Materials/Set Up (Including Misconceptions)

**Materials needed**

For Students: No material required

For Teachers: Slides (if desired), 


## SCRIPT OF TEACHING AND LEARNING ACTIVITIES

### Introducing The Lesson

Recommended: 5 minutes/hours

Teachers introduce ethics and explain why it is significant. 

<!--ethics: universal declaration of human rights --> 
Teachers explain the origin of the term ethics: 
The term ethics comes from the word "ethos", which is Greek for "way of living". 


Teachers explain what is ethics: 
When there is a difficult situation, there are multiple possible solutions. Ethics consists of moral principles and values of a person or a group of people. It affects how we choose to live our lives, what we think is wrong and right in morals and situations, and what our responsibilities are.

Teachers explain the importance of ethics: 

By considering ethics during decision making, we can make better decisions that would benefit individuals and society as a whole.


Specifically for ethical issues that are related to AI, they can be split into three different categories. 

The ethical implications of what AI is: 

1) Bias and Fairness  
2) Accountability and Remediability  
3) Transparency, Interpretability, and Explainability  

THe ethical implications related to what AI does: 

1) Safety  
2) Human-AI interaction  
3) Cyber-security and Malicious Use  
4) Privacy, Control, and Agency  

### Main Lesson

Recommended: 40 minutes/hours

Teachers will teach students about important ethical problems that are present in technology, autonomous systems, and engineering.

#### Correctness and Uncertainty of Algorithms and/or Autonomous Systems

Teachers explain autonomous systems, AI, ML, DL, and usage of algorithms: 

By incorporating artificial intelligence (AI) into systems, they gain the potential to accomplish tasks that usually rely on the intelligence of humans. Systems can become autonomous, and do not have to rely on human control and decisions. An example of an autonomous system that is currently developing is autonomous cars. 


AI systems utilize Deep Learning (DL) and Machine Learning (ML), which both rely on data matching and analysis algorithms. 


Teachers explain the benefits of AI autononous systems and the use of algorithms in decision making processes: 

There are benefits to this. 

Decisions can be made with more clearer and transparent criteria and choices will be less influenced by human emotions. The systems can learn from past actions and decisions that have been chosen and can analyze the consequences that resulted. If a result was non-favorable, then the system will remember and avoid picking the same choice for a similar future situation.

Teachers explain the disadvantages of AI autonomous systems and the use of algorithms in decision making processes: 

There are also some disadvantages to autonomous systems or relying on algorithms to make decisions. 

The algorithms may not represent all the factors that are related to a situation. There is also always chances that unexpected consequences will happen. There is no guarantee that a choice that had beneficial results in the past will still have the same result in the current scenario. 

Also, the way that AI systems learn and their actions may become more unpredictable as they are given more complicated tasks that require more decision making skills (Yampolskiy). 

##### Example: Husky Vs Wolf In Image Identification

Teachers explain a simple algorithmic inaccuracy due to unfair/unrepresentative data example. 

University of Washington wanted to create an image classifier that can identify wolves from huskies correctly. The AI systems were fed images to learn from. However, some photos of huskies are incorrectly categorized by the system as wolves. It turns out that the system was learning from the images that wolves are often found in images that had snowy backgrounds. So the system turned out to be simplying identifying if images had snow in the background (Medium). 

When there was a wolf in an image with no snow in the background, it would be categorized as a husky. If there was a husky with a snowy background, it would be categorized as a wolf (Ribeiro et al.). 

This inaccuracy of the system is because of a data set that was "unfair" or did not have a sufficient variety of scenarios (Besse et al.). 

<!--
Source: Ribeiro, Singh, Guestrin, Why Should I Trust You? Published in 2016

and 

https://www.researchgate.net/publication/329277474_Can_Everyday_AI_be_Ethical_Machine_Learning_Algorithm_Fairness_english_version
10.13140/RG.2.2.22973.31207

and

https://becominghuman.ai/its-magic-i-owe-you-no-explanation-explainableai-43e798273a08 
-->

##### Example: Artificial Neural Network to predict risk of pneumonia patients

University of Pittsburgh created a study in the 1990s to use a system to predict which pneumonia patients were low risk and which were at high risk. The system initially caused a large amount of concern to doctors because they found out that pneumonia patients with asthma was classified as low risk by the system. A rule system was implemented into the system to help solve this issue. After examining data closely, researchers founds that patients who had both pneumonia and asthma had a higher recovery rate. This is because when those patients were brought to the hospital, they were always considered to be at high risk, and immediately received proper treatment. However, the autonomous system simply believed that the presence of asthma results in being low risk, which is incorrect (Medium). 

<!-->
https://becominghuman.ai/its-magic-i-owe-you-no-explanation-explainableai-43e798273a08 --> 


##### Example: Teachers can teach about an example of Algorithmic inaccuracy: The Boeing 737 MAX.


There have been a number of accidents with the Boeing 737 MAX aircraft, which has resulted in the grounding of Boeing 737 MAX worldwide. 

1) Lion Air Flight 610: domestic flight that took place on October 29, 2018. It crashed into the Java Sea shortly after takeoff. Resulted in deaths of all 189 passengers and crew. 

2) Ehiopian Airlines Flight 302: international flight that took place on March 10, 2019. It crashed shortly after takeoff, and resulted in deaths of all 157 people on the flight.  


Teachers explain why MCAS was added and how the MCAS and a faulty sensor contributed to the grounding of the Boeing 737 MAX. 

There were several reasons that contributed to these fatal accidents:

The Boeing 737 Max 8 is different from the earlier Boeing 737 series. To allow for expanded seating capacity and better engines, Boeing 737 Max 8 had major design changes. The engines were moved forward and were raised. However, this made it more likely for the nose to pitch up while flying, so Maneuvering Characteristics Augmentation System or MCAS was developed to help correct the nose pitching problem by altering the control surface at the tail. The algorithm automatically detects whenever the nose pitches too high and corrects it (Seattle Times). 


<!--https://www.seattletimes.com/seattle-news/times-watchdog/the-inside-story-of-mcas-how-boeings-737-max-system-gained-power-and-lost-safeguards/ --> 

MCAS relies on only a single angle of attack sensor, instead of two. An angle of attack sensor helps warn pilots of a possibility of them losing control of the plane due to lack of lift (causing stall). Pilots are usually able to handle when the sensors are malfunctioning, however MCAS makes it a much larger problem. In both of the fatal accidents, MCAS was automatically switched on because of incorrect data from the single sensor (The Washington Post). 

<!-- https://www.washingtonpost.com/local/trafficandcommuting/boeing-minimized-to-faa-the-importance-of-flight-control-system-implicated-in-737-max-crashes-new-report-says/2020/07/01/9900adda-bba4-11ea-8cf5-9c1b8d7f84c6_story.html -->

Pilots can temporarily switch MCAS off, however the system will restart and continue to work if the sensor continues to warn pilots of stalls. MCAS cannot ever been overriden by the pilots. The pilots lost control of the plane during the Ethiopian Airlines and Lion Air flights as the system was continuously fed inaccurate data from the sensor indicating that there are stalls, and they were unable to pitch up when needed, causing both flights to dive into the sea (The Verge). 

<!-- https://www.theverge.com/2019/5/2/18518176/boeing-737-max-crash-problems-human-error-mcas-faa --> 

Teachers also explain other flaws with the incident:  

1) Insufficient testing: 

Boeing and FAA agreed to not install safety features, which analysts say later that these features could have saved both the planes from crashing (The Washington Post).

<!-- https://www.washingtonpost.com/local/trafficandcommuting/boeing-minimized-to-faa-the-importance-of-flight-control-system-implicated-in-737-max-crashes-new-report-says/2020/07/01/9900adda-bba4-11ea-8cf5-9c1b8d7f84c6_story.html--> 
2) Accountability: 

Boeing did not provide the risk assessment about the MCAS until very late, a couple of months before the MAX was certified. FAA also based on findings by Boeing that were inaccurate (The Washington Post). 
 

3) Lack of notice to pilots: 

During their findings, Boeing calculated that an MCAS failure was also impossible. If it did happen, it is believed to be relatively low risk because according to the FAA, it is assumed that pilots can respond to unexpected situations within three seconds (Seattle Times). 

Because of the low chances that were predicted, Boeing decided to not include the MCAS in the pilot manuals (Seattle Times). 

<!--https://www.seattletimes.com/seattle-news/times-watchdog/the-inside-story-of-mcas-how-boeings-737-max-system-gained-power-and-lost-safeguards/ --> 

#### Algorithmic Bias

Teachers teach that algorithmic bias can result from multiple sources. 

1) The algorithm may be programmed by someone who is biased, and inherit their biased views.

2) Since the systems often rely on pattern matching algorithms, an algorithm may act in a biased way because of being provided data that comes from biased sources. 

3) The dataset given to the system to learn from could have biases that the developer is unaware of. Regarding the point made before regarding algorithmic uncertainty, from the data it receives, robots may unintentionally develop a biased and stereotypical way of thinking while trying to establish which factors it should prioritise during decision making.

##### Bias through a AI controlled Hand-Soap Dispenser 

An autonomous soap dispenser was found to have trouble dispensing people for darker skin color 

<!-- https://reporter.rit.edu/tech/bigotry-encoded-racial-bias-technology --> 

##### Example: Amazon: Congress Matched to Criminals 

Teachers teach about another example of algorithmic inaccuracy in AI systems, this one is more applicable to humans. 

Amazon created Rekognition, which is a facial recognition software. ACLU tested the software by matching Congress members, and the result was shocking: 28 members were matched with criminals. In addition, it was found that 40% of the inaccurate image matches were of people of color (ACLU NorCal).  

This is risky to be actually implemented for law enforcememt purposes, as it can make a police officer more biased before an initial encounter, or it can increase the chances of a person being questioned or searched, or can increase bias towards people of color (ACLU NorCal).

<!--https://www.aclunc.org/blog/amazon-s-face-recognition-falsely-matched-28-members-congress-mugshots -->

##### An example: Autonomous systems and identification by skin tone

According to a study done with autonomous systems by Georgia Institute of Technology, AI systems were more consistently accurately identifying people with lighter skin tones than darker. Their results show that detection of people with darker skins were less accurate by 5%. 

This can result in racial bias by the algorithm, and in the case of autonomous cars, people with darker skin would be more likely to be harmed or involved in an accident than those with lighter skin. 

##### Another example: autonomous cars and the morality/trolley problem

 <!-- done as a game, data set is not entirely reliable -->

<!--  internet cyber security/how much trust assumption/use for good or bad are possible ; unintended uses when developing --> 

Another difficulty of autonomous cars is with the "trolley problem". MIT has created a series of questions/scenarios that involve autonoous cars. Examples include whether to ____. There are general trends found such as _____. There are also general trends found in certain cultures. Examples of this include: saving the lawful ______. 

While this is a gamefied way, it is very interesting to take into consideration moral concepts that we think about it dire situations. 

#### Security, on time, backups, as these systems become relied upon 

There are many systems in society that utilize autonomous systems that are important to society. 
 
##### An example: Autonomous Systems Used in Social Credit System Development in China

AI facial reconition systems have begun to be in use in China for developing a social credit system. 

##### American
<!-- ex: compass US, criminal scoring system: 
# close source vs open source to look for bias problems or data sets in source code --> 


##### An example: Unsecured/Exposed Robots Running on ROS and Internet:

A research team at Brown University discovered that they found almost 100 exposed systems that ran on ROS. "Up to 19 were considered to be fully operational robots". They found that they could access the cameras of the robots, and be able to give them commands for movement remotely (Brown University).  

<!-- https://www.brown.edu/news/2018-07-24/robots -->
#### Militarization

There has been consideration of using autonomous systems for militarization. This could be for making military based decisions or using these systems to take action on made military decisions. 

<!-- discussion of ITAR, weapons, discussion of stopping war robots; robotics weapons vs chemical weapons; strong regulations? -->

##### ITAR

##### Example: Predator drones utilized by the United States

There have been several predator drones that have been used by the United States Air Force (USAF) and Central Intelligence Ageny (CIA). 

It was initially utilized for primarily reconaissance and spying, but was later equipped to be able to engage in warfare.

It is remotely piloted. There has been many concerns regarding to human safety. 

With drone contro____. 

##### Should we handle autonomous weapons like chemical weapons

#### Medical, Healthcare, and Caregiver Robots

Autonomous systems and AI systems have been also considered for usage in the healthcare industry. 

This includes the uses of robots to help with identification, medical diagnosis, treatment, or surgery. 

It also includes the uses of robots to help keep elderly, disabled, young children, or patients company and to surpervise them. 

This presents an important topic: the interactions between humans and robots. Robots do not have emotions. This may present several ethical concerns:

1) Privacy/Security: 

Robots that spend a lot of time monitoring their patients or people that they are responsible for, may have the capability to be tapped into.

Especially in the medical field, these robots may contain snippets of important information such as health records about patients, or ______. 

2) Trust between robots and humans, and their interactions:

Th ______. 

##### The Emergency Exit Robot Study, Georgia Tech Howard



#### Availability/Accessibility/Uses

The cost of autonomous systems may be high depending on the purpose of the robot, and how regulated it is. 

##### UN Guidelines for Emergency Uses of Drones

##### Humanitarian Drone Guidelines

#### Future impact of AI on human jobs and responsibilities

With the development of AI, there has been a growing reliance on them as tools in our daily lives. 

Ethical implications related to what AI can impact: 

1) Automation, Job Loss, Labor Trends
2) Impact to Democracy and Civil Rights
3) Human-Human or Human-Agent interaction

There are large impacts of AI: 

Some of this include affecting human jobs. There have come to time where many jobs can be taken over by robots _____. 


### Ending The Lesson

Recommended: 5 minutes/hours

With the development of AI/autonomous systems being developed, 

Teachers remind that there will be a safety module for the course coming up in one of the future classes:   

There will be a future lesson specifically regarding how to keep yourself and those around you safe when operating your drone. 

**Useful Resources and References**

More information about the MCAS system for the Boeing 737 MAX: 
https://www.seattletimes.com/seattle-news/times-watchdog/the-inside-story-of-mcas-how-boeings-737-max-system-gained-power-and-lost-safeguards/ and https://www.theverge.com/2019/5/2/18518176/boeing-737-max-crash-problems-human-error-mcas-faa

https://www.bbc.com/news/business-50177788



Paper: Predictive Inequity in Object Detection: 
https://arxiv.org/pdf/1902.11097.pdf


Moral machine: https://www.moralmachine.net

Paper on moral machine: https://doi.org/10.1038/s41586-018-0637-6 


https://ici.radio-canada.ca/info/2019/voitures-autonomes-dilemme-tramway/index-en.html