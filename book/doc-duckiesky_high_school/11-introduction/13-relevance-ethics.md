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

- Teachers explain the origin of the term ethics: 

See also: The term ethics comes from the word "ethos", which is Greek for "way of living" (BBC). 

- Teachers explain what is ethics: 

See also: When there is a difficult situation, there are multiple possible solutions. Ethics consists of moral principles and values of a person or a group of people. It affects how we choose to live our lives, what we think is wrong and right in morals and situations, and what our responsibilities are (BBC).

See also: Universal Declaration of Human Rights regarding ethics

- Teachers explain the importance of ethics: 

See also: By considering ethics during decision making, we can make better decisions that would benefit individuals and society as a whole.


See also: Specifically for ethical issues that are related to AI, they can be split into three different categories. 

See: The ethical implications of what AI is: 

1. Bias and Fairness  
2. Accountability and Remediability  
3. Transparency, Interpretability, and Explainability  

See: Te ethical implications related to what AI does: 

1. Safety  
2. Human-AI interaction  
3. Cyber-security and Malicious Use  
4. Privacy, Control, and Agency  

### Main Lesson

Recommended: 40 minutes/hours

- Teachers will teach students about important ethical problems that are present in technology, autonomous systems, and engineering.

##### Correctness and Uncertainty of Algorithms and/or Autonomous Systems

- Teachers explain autonomous systems, AI, ML, DL, and usage of algorithms: 

See also: By incorporating artificial intelligence (AI) into systems, they gain the potential to accomplish tasks that usually rely on the intelligence of humans. 

See also: AI systems utilize Deep Learning (DL) and Machine Learning (ML), which both rely on data matching and analysis algorithms. 

- Teachers explain the benefits of AI autononous systems and the use of algorithms in decision making processes: 

See also: Decisions will be less influenced by human emotions. The systems can learn from past actions and decisions that have been chosen and can analyze the consequences that resulted. 

- Teachers explain the disadvantages of AI autonomous systems and the use of algorithms in decision making processes: 

See also: The algorithms may not represent all the factors that are related to a situation. There is also always chances that unexpected consequences will happen. Also, the way that AI systems learn and their actions may become more unpredictable as they are given more complicated tasks that require more decision making skills (Yampolskiy). 


#### Example: Husky Vs Wolf In Image Identification

- Teachers explain a simple algorithmic inaccuracy due to unfair/unrepresentative data example. 

See also: University of Washington wanted to create an image classifier that can differentiate between wolves and huskies (Medium). The AI systems were fed images to learn from. Some photos were incorrectly classified. System was learning from the images that wolves were more often with snowy backgrounds. 

See also: When there was a wolf in an image with no snow in the background, it would be categorized as a husky. If there was a husky with a snowy background, it would be categorized as a wolf (Ribeiro et al.). 

See also: This inaccuracy of the system is because of a data set that was "unfair" or did not have a sufficient variety of scenarios (Besse et al.). 

<!--
Source: Ribeiro, Singh, Guestrin, Why Should I Trust You? Published in 2016

and 

https://www.researchgate.net/publication/329277474_Can_Everyday_AI_be_Ethical_Machine_Learning_Algorithm_Fairness_english_version
10.13140/RG.2.2.22973.31207

and

https://becominghuman.ai/its-magic-i-owe-you-no-explanation-explainableai-43e798273a08 
-->

#### Example: Artificial Neural Network to predict risk of pneumonia patients

- Teachers explain a simple algorithmic inaccuracy due to unfair/unrepresentative data example. 

See also: University of Pittsburgh studied system to predict which pneumonia patients were low risk and which were at high risk. Patients who had both pneumonia and asthma had a higher recovery rate because when those patients were brought to the hospital, they were always considered to be at high risk, and immediately received proper treatment. 

See: From the data it was learning from, the autonomous system simply believed that the presence of asthma results in being low risk and classified patients as so, which was incorrect and problematic (Medium). 

<!-->
https://becominghuman.ai/its-magic-i-owe-you-no-explanation-explainableai-43e798273a08 --> 


#### Example: Teachers can teach about an example of Algorithmic inaccuracy: The Boeing 737 MAX.

- Teachers can teach about another example: The Boeing 737 MAX: 

See also: There have been a number of accidents which resulted in many casualties with the Boeing 737 MAX aircraft, which has resulted in the grounding of Boeing 737 MAX worldwide: Lion Air Flight 610 and Ehiopian Airlines Flight 302

- Teachers explain why MCAS was added and how the MCAS and a faulty sensor contributed to the grounding of the Boeing 737 MAX. 

See also: Boeing 737 Max 8 had major design changes: engines were moved forward and raised. This made it more likely for the nose to pitch up while flying, so Maneuvering Characteristics Augmentation System (MCAS) was implemented to automatically detect whenever the nose pitches too high and correct it (Seattle Times). 

<!--https://www.seattletimes.com/seattle-news/times-watchdog/the-inside-story-of-mcas-how-boeings-737-max-system-gained-power-and-lost-safeguards/ --> 

See also: MCAS relies on only a single angle of attack sensor, instead of two. An angle of attack sensor helps warn pilots of a possibility of them losing control of the plane due to lack of lift (causing stall). Pilots are usually able to handle when the sensors are malfunctioning, however MCAS makes it a much larger problem. In both of the fatal accidents, MCAS was automatically switched on because of incorrect data from the single sensor (The Washington Post). 

<!-- https://www.washingtonpost.com/local/trafficandcommuting/boeing-minimized-to-faa-the-importance-of-flight-control-system-implicated-in-737-max-crashes-new-report-says/2020/07/01/9900adda-bba4-11ea-8cf5-9c1b8d7f84c6_story.html -->

See also: Pilots can temporarily switch MCAS off, however the system will restart and continue to work if the sensor continues to warn pilots of stalls. MCAS cannot ever been overriden by the pilots. The pilots lost control of the plane during the Ethiopian Airlines and Lion Air flights as the system was continuously fed inaccurate data from the sensor indicating that there are stalls, and they were unable to pitch up when needed, causing both flights to dive into the sea (The Verge). 

<!-- https://www.theverge.com/2019/5/2/18518176/boeing-737-max-crash-problems-human-error-mcas-faa --> 

- Teachers also explain other flaws with the incident:  

See also: Insufficient testing: Boeing and FAA agreed to not install safety features due to calculations of impossibility of a MCAS failure, which analysts say later that these features could have saved both the planes from crashing (The Washington Post).

<!-- https://www.washingtonpost.com/local/trafficandcommuting/boeing-minimized-to-faa-the-importance-of-flight-control-system-implicated-in-737-max-crashes-new-report-says/2020/07/01/9900adda-bba4-11ea-8cf5-9c1b8d7f84c6_story.html--> 

See also: Accountability: Boeing did not provide the risk assessment about the MCAS until very late, a couple of months before the MAX was certified. FAA also based on findings by Boeing that were inaccurate (The Washington Post). 
 
See also: Lack of notice to pilots: Assumed that pilots can respond to unexpected situations within three seconds and since low chances of MCAS failure, Boeing decided to not include the MCAS in the pilot manuals (Seattle Times). 

<!--https://www.seattletimes.com/seattle-news/times-watchdog/the-inside-story-of-mcas-how-boeings-737-max-system-gained-power-and-lost-safeguards/ --> 

##### Algorithmic Bias

- Teachers teach that algorithmic bias can result from multiple sources. 

See also: The algorithm may be programmed by someone who is biased.

See also: Algorithm may learn from data that comes from biased sources.

See also: The dataset given to the system does not have enough variety, or simply the data contains bias that developers are unaware of.


#### Example: Amazon: Congress Matched to Criminals 

- Teachers teach about another example of algorithmic inaccuracy in AI systems and possible consequences, this one is more applicable to humans. 

See also: Rekognition: a facial recognition software. ACLU tested the software by matching Congress members, and the result was that 28 members were matched with criminals. 

See also: 40% of the inaccurate image matches were of people of color (ACLU NorCal). 

See also: Risks with implementation in law enforcement: police officer more biased before an initial encounter, increase the chances of a person being questioned or searched, or can increase bias towards people of color (ACLU NorCal).

<!--https://www.aclunc.org/blog/amazon-s-face-recognition-falsely-matched-28-members-congress-mugshots -->

#### An example: Autonomous systems and identification by skin tone

- Teachers teach about a persistant problem in autonomous systems: how they identify people of different skin tones

See also: An autonomous soap dispenser by Technical Concepts was found to have trouble dispensing people for darker skin color. See also: Many systems rely on IR sensors, measures how much light is reflected back. Darker skin tones absorb more light than people with lighter skin tones (Reporter). 

See also: This design flaw was believed to be because of a lack of diversity in the workplace at Technical Concepts, who did not think to test their products on people with darker skin tones (Reporter). 

<!-- https://reporter.rit.edu/tech/bigotry-encoded-racial-bias-technology --> 

See also: According to a study done with autonomous systems by Georgia Institute of Technology, AI systems were more consistently accurately identifying people with lighter skin tones than darker. Their results show that detection of people with darker skins were less accurate by 5%. 

See also: This can result in racial bias by algorithms, and in the case of autonomous cars, people with darker skin would be more likely to be harmed or involved in an accident than those with lighter skin. 

#### Another example: MIT's Moral Machine

- Teachers teach about the Moral Machine. 

See also: In 2014, MIT has created a series of questions and scenarios that involve autonomous cars and artificial intelligence, which is known as the Moral Machine. The Moral Machine asks people which choices autonomous cars should make when facing different variations of the trolley problem (Technology Review). 

The Moral Machine focuses on 9 different themes: 

1. Humans or pets/animals?

2. Passengers or pedestrians?

3. More or fewer lives?

4. Women or men?

5. Young or old?

6. Healthy or those with health conditions?

7. People of those of higher or lower status? 

8. Action or no action? 

See also: The results of the Moral Machine was closely related with culture and economics (Technology Review). 

See: Students may read this article: https://www.technologyreview.com/2018/10/24/139313/a-global-ethics-study-aims-to-help-ai-solve-the-self-driving-trolley-problem/ to learn more about the experiment and findings.

See also: While this is presented in a very "game" like way, it is very interesting to take into consideration moral concepts that we think about in extreme situations. 

<!-- https://www.media.mit.edu/projects/moral-machine/overview/ 

https://www.media.mit.edu/publications/the-moral-machine-experiment/

https://www.technologyreview.com/2018/10/24/139313/a-global-ethics-study-aims-to-help-ai-solve-the-self-driving-trolley-problem/

-->

#### Security, on time, backups, as these systems become relied upon 

- Teachers teach that there are many systems in society that utilize autonomous systems that are important to society. 
 
See also: There has been ongoing debate whether these systems should be close or open sourced. 

See also: Open source code means that the source code can be accessed by the public. 

See also: Closed source code means that the source code cannot be accessed by others, or it remains classified, only seen by those who are authorized to. 

See also: While closed source codes may safer from prying eyes or hackers, it also prevents closer scrutiny for potential biases or problems in the code by the public. 

See also: an interesting question is how much trust do we put into these autonomous systems? People can easily use these systems in ways that are beyond what developers anticipate. 


#### An example: Autonomous Systems Used in Social Credit System Development in China

- Teachers can teach about an example of a system that utilized AI to be implemented in an entire society

See also: The Chinese government began experimenting with social credit scores in 2015, when it allowed private companies to assign credit scores to people. Financial and social behaviors are analyzed and people are assigned scores (Time). People who accomplish good deeds are awarded points and can receive rewards. Those who do bad deeds, such as smoking or spending too much time on video games, are deducted points. Those with an extremely low social credit score are placed on the “List of Untrustworthy Persons” and will be prohibited from certain activities such as the ability to use public transportation or to make large purchases.

See also: This is being implemented with the help of AI and facial recognition. 

See also: There has been many concerns with the use of China's social credit system, fears about leading to social inequality and alienation. There are also fears of preventing a free market economy. While the benefits include trying to reduce the amount of crimes or bad habits of people. 

<!-- 
https://time.com/collection/davos-2019/5502592/china-social-credit-score/
-->

#### Correctional offender Management Profiling for Alternative Sanctions (COMPAS) 

- Teachers can teach about COMPAS, which is a system used in the US

See also: COMPAS is an software that is used by US courts to assign scores to predict the risk of a certain person commiting another crime. 

See also: It is an algorithm that utilizes an algorithm that considers answers to a questionnaire (The Atlantic). 

See also: In 2016, ProPublica has analzyed COMPAS and has found that COMPAS displays bias against African Americans. 

<!-- https://www.theatlantic.com/technology/archive/2018/01/equivant-compas-algorithm/550646/ -->


#### An example: Unsecured/Exposed Robots Running on ROS and Internet:

- Teachers can teach about risks of vulnerable systems can be when connected to the internet.

- Students will learn more about Robotics Operating System (ROS) in a later module, but it is a set of open source libraries that can help with programming of robots. 

See also: A research team at Brown University discovered that they found almost 100 exposed systems that ran on ROS. "Up to 19 were considered to be fully operational robots". They found that they could access the cameras of the robots, and be able to give them commands for movement remotely (Brown University).  

<!-- https://www.brown.edu/news/2018-07-24/robots 
and https://www.wired.com/story/security-robotics/
-->


##### Militarization

- Teachers can teach that there has been consideration of using autonomous systems for militarization. This could be for making military based decisions or using these systems to take action on made military decisions. 

See also: Students can watch this video to learn more about Slaughterbots: https://www.youtube.com/watch?v=9CO6M2HsoIA

#### International Traffic in Arms Regulations (ITAR)

- Teachers can teach about ITAR: 

See also: International Traffic in Arms Regulations (ITAR) specifically covers: 

1. Covers military items or defense articles  
2. Regulates goods and technology designed to kill or defend against death in a military setting  
3. Includes space-related technology because of application to missile technology  
4. Includes technical data related to defense articles and services  
5. Involves strict regulatory licensing and does not address commercial or research objectives  

(Source: Digital Guardian)

<!-- https://digitalguardian.com/blog/what-itar-compliance --> 

#### Example: Predator drones utilized by the United States

- Teachers about the predator drones as an example of drones/robotic systems that are currently/previously in use by the US government related to milatary operations.

See also: There have been several predator drones that have been used by the United States Air Force (USAF) and Central Intelligence Ageny (CIA). Initially many are utilized for primarily reconaissance and spying, but many have been later equipped to be able to engage in warfare.

#### Should we handle autonomous weapons like chemical weapons

See also: In the US, there are two types of chemical warfare agents: stockpiled and non stockpiled. 

See also:"In 1996, it was mandated that all stockpiles of lethal chemical agents must be destroyed. 

See also: In 1997, the US ratified Chemical Weapons Convention Treaty and agreed to destory any remaining stockpiles of chemical warfare agents to no later than April 29, 2012" (CDC).

See also: There has been much debate if autonomous weapons should be treated like chemical weapons? Should they also be prohibited from use and fully destroyed? 

<!-- https://www.cdc.gov/nceh/demil/history.htm --> 

##### Medical, Healthcare, and Caregiver Robots

- Teachers can teach that autonomous systems and AI systems have been also considered for usage in the healthcare industry. 

See also: This includes the uses of robots to help with identification, medical diagnosis, treatment, or surgery. It also includes the uses of robots to help keep elderly, disabled, young children, or patients company and to surpervise them. While there are many benefits such as being able to take care and monitor health of whoever they are responsible for and can provide them with company, there are several ethical concerns:

See: Privacy/Security: Robots that spend a lot of time monitoring their patients or people that they are responsible for, may have the capability to be tapped into.Especially in the medical field, these robots may contain snippets of important information such as health records, or video feeds of their patients. 

See: Trust between robots and humans, and their interactions: Humans have emotions while robots do not. Humans may have the capability to trust their robots too much, which can result in harm from the remote or manipulation of humans. 

#### The Emergency Exit Robot Study, Georgia Tech Howard

- Teachers can teach students about an experiment that utilizes robots in a care setting and show the risks of putting to much trust into robots.

See also: There was a study conducted by researchers at the Georgia Institute of Technology, highlighted the potential risks of putting too much trust into robots during emergency situations. 

See also: They did an experiment that simulated an emergency situation. It was found that all participants of the experiment decided to follow the robot during the emergency, even if it led them through an noticeably incorrect path. Half of the participants have also seen the robot fail at navigating earlier before the specific experiment (Robinette et al.).  

<!-- https://www.cc.gatech.edu/~alanwags/pubs/Robinette-HRI-2016.pdf
-->

##### Availability/Accessibility/Uses

- Teachers can teach about the extent that robots are available to the public vs private sectors, accessibility of robots to people who may have accessibility issues, and the large amount of uses of UAV and autonomous systems. 

See also: The cost of autonomous systems may be high depending on the purpose of the robot. The high prices of robots currently are barring many people from more complex robots. 

See also: Robots can be used to help those with accessbility issues. 

See also: Beyond the other purposes already explained, autonomous systems and advanced technology may also be used to help with emergency aid purposes. Drones can be used to help with potentially locating lost items or people, or helping transport emergency items quickly (water for forest fires ex.). 

#### UN Guidelines for Emergency Uses of Drones

- Teachers can teach that drones have been utilized by the UN. 

See also: UAVs have potential in three areas: humanitarian, development, and peacekeeping operations (UN). 

See also: In 2013, the UN has launched the first UAV mission to help protect civilians in the Democratic Republic of Congo (UN News). 

See also: Read this article for more information: https://news.un.org/en/story/2017/09/564452-feature-does-drone-technology-hold-promise-un and https://news.un.org/en/story/2013/12/456942-un-launches-unmanned-surveillance-aircraft-better-protect-civilians-vast-dr 

See also: "The most promising uses of drones include: Mapping, Delivering lightweight essential items to remote or hard-
to-access locations, Supporting damage assessments, Increasing situational awareness, Monitoring changes" (Relief Web).


<!-- https://reliefweb.int/sites/reliefweb.int/files/resources/Drones%20in%20Humanitarian%20Action.pdf --> 

##### Future impact of AI on human jobs and responsibilities

- Teachers can teach that with the development of AI, there has been a growing reliance on them as tools in our daily lives. They have a large impact on all of us: 

See also: Ethical implications related to what AI can impact: 

See also: Automation, Job Loss, Labor Trends: With the automation of many jobs, people may lose those jobs to robots. This may be because some tasks are able to be done more efficiently by robots. Because some jobs are more adaptable to robots than others, this may produce labor trends. There will be new jobs created that are more oriented towards maintaining robots or certain jobs will die out. 

See also: Impact to Democracy and Civil Rights: AI may have a strong impact on democracy and civil rights. AI may be able to automatically detect certain messages or actions that are not permitted and can be used to prevent them. There has been related concerns to that and the Chinese Social Credit System, and fear that it may create a society focused around surveillance and conformity. 

See also: Human-Human or Human-Agent interaction: As explored slightly in the medicine uses of robots, there will be much more interactions between human and non humans/robots in the future, which is different from interactions between humans only. 

##### Possible Assignments or Discussion Topics: 



### Ending The Lesson

Recommended: 5 minutes/hours

- Teachers can summarize ethics and the large positive and negative benefits of AI

- Teachers remind that there will be a safety module for the course coming up in one of the future classes:   

**Useful Resources and References**

More information about the MCAS system for the Boeing 737 MAX: 
https://www.seattletimes.com/seattle-news/times-watchdog/the-inside-story-of-mcas-how-boeings-737-max-system-gained-power-and-lost-safeguards/ and https://www.theverge.com/2019/5/2/18518176/boeing-737-max-crash-problems-human-error-mcas-faa

https://www.bbc.com/news/business-50177788

Paper: Predictive Inequity in Object Detection: 
https://arxiv.org/pdf/1902.11097.pdf

Moral machine: https://www.moralmachine.net

Paper on moral machine: https://doi.org/10.1038/s41586-018-0637-6 

https://ici.radio-canada.ca/info/2019/voitures-autonomes-dilemme-tramway/index-en.html