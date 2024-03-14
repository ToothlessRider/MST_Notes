#  SDP Notes for MST
> Author : Aaron Augustine

> Star the gist so that I can get a consensus on how many people are using this resource

### Reference Links 
1. [Class diagram](https://www.youtube.com/watch?v=HuL9EMx8NQo)
2. [Use Case diagram](https://www.youtube.com/watch?v=Hj6Lkoi_VoM)
3. [State chart diagram](https://www.youtube.com/watch?v=TzTl4pdEYWE)
4. [ER diagram](https://www.youtube.com/watch?v=Yxz0Vy1uPoc)
5. [Activity diagram](https://www.youtube.com/watch?v=LyhTDsjjjrE)


# PYQ's
#### Q1 a. Why should software development  focus on the needs of Users? 
*Ans*. Software development should focus on the needs of the users for the following reasons : **R<sup>3</sup>**
* To *reduce training and support* costs ( i.e, make it so that users naturally understand how to use the software ).
* To *reduce time to learn* the system..
* To *reduce costs by developing only the required features*.
* To *create a UI accurate to what the user wants*.
* Since UI is the entire application for users, making sure it is good and according to what the user wants is very important.


<hr>

#### Q1 b. Why must software engineers  develop an understanding of the Users?
*Ans*. The reasons why software engineers must develop and understanding of users are : 
* To understand the goals for the system
	* What is the work the user needs to get done ?
* Potential patterns of use
* Demographics
* Knowledge of application domain
* Physical Ability


<hr>

#### Q2 a. Differentiate between Usability and Utility with reference to software design pattern
*Ans* 
### Usability

* Does the system allow the user to learn and to use raw capabilities easily?

The Key aspects of usability are : 
- **Learnability:** How easy is it for users to learn how to use the system?
- **Efficiency:** Once users have learned the system, how quickly can they perform tasks?
- **Memorability:** After a period of not using the system, how easily can users re-establish proficiency?
- **Error Prevention and Recovery:** How well does the system prevent errors, and if errors occur, how easily can users recover?
- **User Satisfaction:** How satisfied are users with their overall experience?

*Example:* An e-commerce website with a clear and intuitive navigation menu, simple checkout process, and helpful error messages has good usability.

### Utility

* Does the system provide the raw capabilities to allow the user to achieve their goal

The key aspects of utility are :
- **Relevance:** How well does the system address the user's specific requirements or objectives?
- **Functionality:** Does the system provide the necessary features and tools to accomplish tasks?
- **Value:** How much value does the user perceive in using the system?
- **Fit for Purpose:** Is the system designed to serve its intended purpose effectively?
   
*Example:* A project management software that includes features such as task tracking, team collaboration, and reporting provides utility for users managing complex projects.

<hr>

#### Q2 b. Consider software is to be built for automatic recording of online meeting attendance, assume suitable data and perform class based modelling.

*Ans* 


<hr>

#### Q3 a. Online teaching software is to be built which should have the following major functionalities:
1. User interface and control
2. Creating meeting, inviting participants
3. Presenting screen along with audio and video
4. Recording and storing in database
5. Computer graphics along with display
6. Taking attendance
7. Giving quiz and assignment
8. Peripherals attachment / external hardware attachment
Perform use case modelling. assume suitable data.

*Ans* 


<hr>

#### Q3 b. List and explain usability principles? How will you evaluate user interface explain with an example.

*Ans* The principles of Usability are as follows : *DEEPEEBUBCEP*
* Do not rely on usability guidelines - Always test with users
* Ensure that the sequences of actions to achieve a task are as simple as possible
* Ensure that a user knows what they should do next
* Provide good feedback including effective error messages
* Ensure the user can always get out, or revert an action
* Ensure that response time is adequatw.
* Base UI designs on user's tasks
* Use understandable encoding techniques
* Be consistent
* Consider the needs of different groups of users
* Ensure that the UI's appearance is uncluttered
* Provide all necessary help

<hr>

#### Q4 a. What are Ddifficulties and risks in Use Case Modelling and User Interface Design

*Ans*.

<hr>

## MST Questions
#### Q1. What is the abstraction-occurence pattern ?

*Ans*.
**Context** :
* 

#### Q2. What are design patterns ?

*Ans*. They are related to small and medium scale design of objects and frameworks.

Applicable to designing a solution for connecting the large scale elements defined via architectural pattern 

They are a group of objects, ( and their relationships ) designed to support a good object design

Good objects have *high cohesion* and *low coupling*


#### Q3. What are pattern description patterns ?

*Ans*. 
#### Context : 
* The general situation in which a pattern is applicable

#### Problem : 
* A short sentence or two raising the main difficulty

#### Forces :
* The issues or concerns, to consider when solving the problem

#### Solution : 
* The recommended way to solve the problem in the given context


#### References : 
* Who developed or inspired the pattern.


#### Q5. What is Design? Define the process of design

*Ans*. Design is a problem-solving process whose objective is to find a way to : 
* implement a systems functional requirements
* While respecting the constraints set by the non functional requirements like : 
	* performance
	* maintainability
	* security
	* cost
	* reliability
	* portability, etc
* all while adhering to the principles of *good quality*

Design is all about **decisions**
* Approach : top down or bottom up
* Design Principles to use
* Satisyfing func req
* Accomodating non func req
* Looking at tradeoffs
* Develop s/w arch to support your design

<hr>

#### Q6. What is object oriented analysis ?
Ans. An investigation of the problem ( Rather than how to find a solution )

During OO analysis, there is an emphasis on finding and describing objects in the problem domain.

Ex. In a library information system include Book and Library.

<hr>

#### Q7. What is object oriented design ?

*Ans* In OO design there is an emphasis on a conceptual solution that fulfils the requirements

You need to define s/w objects and how their relationships fulfil the requirements

Designs are implemented in a programming language


#### Q8. What are the steps taken from design to implementation ?
Ans 
1. Analysis : We investigate the problem
2. Design : Find a logical solution and build a design
3. Construction : Code out the solution

Ex. 
* Book ( Concept )

|Book|
|--|
|title|
|print()|

```
public class Book{
	public void print();
	private String title;
}
```

<hr>

#### Q9. What is design space ?

*Ans*. The space of possible designs that could be achieved by choosing different set of alternatives is often called the design space.
**![](https://lh7-us.googleusercontent.com/gy7NYBCzfejVKCIe_Yy-NB2c8S6xZUCjYPsqi2eVCgpqO3dYljMIRifWL1HeAmhPaTOZb5kSiIMLXPTzPSu5CSWF_AeeRC4J0QaGZ8Slvav2e10PdzB076LODVmAyiGAVhD1KlbV_VBTCC5r8Wen-Lk)**

<hr>

#### Q10. What is a design model/modeling ?

*Ans*. A design model is a set of diagrams showing logical design 
( It assumes a good domain model depicting the concepts shown in the business domain )

This includes software class diagrams, sequence diagrams as well as package diagrams


#### Q11 Give features of top down and bottom up design 
Ans. 

#### Top-down 
* First design the high level structures of the system
* Then work your way down to the low level constructs
* Finally arrive at the detailed decisions such as : 
	* Format of data items
	* Individual algorithms

Start with the software architecture and the type of database to be used

#### Bottom-up design
Make decisions about the low level utilities first
Then decide how they will be put together to make the higher level constructs

* This type of designing helps to create reusable components

<hr>

#### Q12. What are the different types of design ? 
 
 *Ans*. The different types of design are : 
 * Architecture design : 
	 * The division into subsystems and components
		 * How they're connected
		 * How they interact
		 * THeir interfaces




