---
{"dg-publish":true,"permalink":"/process-model-se/","tags":["notes"],"created":"2024-09-25T15:57:32.148+05:30","updated":"2024-09-25T23:13:38.267+05:30"}
---

# Framework Activities
- Communication
- Planning
- Modelling
- Construction
- Deployment
# Important Process Flow
- Linear Process
- Iterative Process
- Evolutionary Process
- Parallel Process
![[Process Model Slide Set 3 (1).pdf#page=7&rect=90,36,678,456|Process Model Slide Set 3 (1), p.7]]
# Process Assessment and Improvement
> [!PDF|yellow] [[Process Model Slide Set 3 (1).pdf#page=9&selection=4,0,6,1&color=yellow|Process Model Slide Set 3 (1), p.9]]
> > Standard CMMI Assessment Method for Process Improvement (SCAMPI) 
> 
> provides a five step process assessment model that incorporates five phases: initiating, diagnosing, establishing, acting and learning


> Give this a look
![[Process Model Slide Set 3 (1).pdf#page=9&rect=93,85,700,456&color=yellow|Process Model Slide Set 3 (1), p.9]]

# Software Life Cycle
Series of identifiable stages that a software product goes during its life time
- Feasibility Study
- Requirements analysis and specification
- Design
- Code
- Testing
- Maintenance

This life cycle model is adhered to
- the project manager can at any time fairly accurately tell
	- at which stage the product is
- Otherwise, it becomes very difficult to track the progress of the project
	- he would have to depend on the guesses of team members

# Attention to Specific Models
■ Classical waterfall model
■ Iterative waterfall, 
■ Evolutionary,
■ Prototyping, and
■ Spiral model

# Top 8 Software Development Models
- [1. Waterfall Model](https://www.geeksforgeeks.org/top-8-software-development-models-used-in-industry/#1-waterfall-model)
- [2. V-Model](https://www.geeksforgeeks.org/top-8-software-development-models-used-in-industry/#2-vmodel)
- [3. Incremental Model](https://www.geeksforgeeks.org/top-8-software-development-models-used-in-industry/#3-incremental-model)
- [4. RAD Model](https://www.geeksforgeeks.org/top-8-software-development-models-used-in-industry/#4-rad-model)
- [5. Iterative Model](https://www.geeksforgeeks.org/top-8-software-development-models-used-in-industry/#5-iterative-model)
- [6. Spiral Model](https://www.geeksforgeeks.org/top-8-software-development-models-used-in-industry/#6-spiral-model)
- [7. Prototype model](https://www.geeksforgeeks.org/top-8-software-development-models-used-in-industry/#7-prototype-model)
- [8. Agile Model](https://www.geeksforgeeks.org/top-8-software-development-models-used-in-industry/#8-agile-model)

## Waterfall Model
Diagram for reference
![[Process Model Slide Set 3 (1).pdf#page=14&rect=57,195,676,390&color=yellow|Process Model Slide Set 3 (1), p.14]]
- The waterfall model is a linear and sequential model, which means that a development phase cannot begin until the previous phase is completed. We cannot overlap phases in waterfall model.

We can imagine waterfall in the following way

> “Once the water starts flowing over the edge of the cliff, it starts falling down the mountain and the water cannot go back up.”

Similarly waterfall model also works, once one phase of development is completed then we move to the next phase but cannot go back to the previous phase. In the waterfall model, the output of one phase serves as the input for the other phase.

### Advantages of Waterfall Model

- This model is simple and easy to understand.
- This is very useful for small projects.
- This model is easy to manage.
- The end goal is determined early.
- Each phase of this model is well explained.
- It provides a structured way to do things.
- This is a ==base model==, ==all the SDLC models that came after this were created keeping this in mind, although they worked to remove its shortcomings==.
- In this model, ==we can move to the next phase only after the first phase is successfully completed so that there is no overlapping between the phases==.

### Disadvantages of Waterfall Model

- In this model, complete and accurate requirements are expected at the beginning of the development process.
- ==Working software is not available for very long during the development life cycle==.
- We cannot go back to the previous phase due to which it is very difficult to change the requirements.
- ==Risk is not assessed in this, hence there is high risk and uncertainty in this model==.
- In this the testing period comes very late.
- Due to its sequential nature this model is not realistic in today’s world.
- This is not a good model for large and complex projects.

## V-Model
Diagram for reference
![[Process Model Slide Set 3 (1).pdf#page=15&rect=160,28,574,403&color=yellow|Process Model Slide Set 3 (1), p.15]]
V-Model is an SDLC model, it is also called Verification and Validation Model. V-Model is widely used in the [software development process,](https://www.geeksforgeeks.org/software-development-process/) and it is considered a disciplined model. In ==V-Model, the execution of each process is sequential, that is, the new phase starts only after the previous phase ends==.
- It is based on the association of testing phase with each development phase that is in V-Model with each development phase, its testing phase is also associated in a V-shape in other words both [software development](https://www.geeksforgeeks.org/software-development/) and testing activities take place at the same time.
- So in this model, ==Verification Phase will be on one side, Validation Phase will be on the other side that is both the activities run simultaneously and both of them are connected to each other in V-Shape through Coding Phase, hence it is called V-Model.==
- ****V-Design:**** In V-Design the left side represents the development activity, the right side represents the testing activity.

### Advantages of V-Model

- This is a simple and easy to use model.
- ==Planning, testing and designing tests can be done even before coding.==
- This is a very disciplined model, in which phase by phase development and testing goes on.
- ==Defects are detected in the initial stage itself.==
- ==Small and medium scale developments can be easily completed using it.==

### Disadvantages of V-Model

- This model is not suitable for any complex projects.
- There remains both high risk and uncertainty.
- This is not a suitable model for an ongoing project.
- ==This model is not at all suitable for a project which is unclear and in which there are changes in the requirement==.

## Incremental Model
Diagram for reference
![[Process Model Slide Set 3 (1).pdf#page=16&rect=97,35,674,395&color=yellow|Process Model Slide Set 3 (1), p.16]]
In Incremental Model, the [software development process](https://www.geeksforgeeks.org/software-development-process/) is ==divided into several increments and the same phases are followed in each increment==. In simple language, under this model a complex project is developed in many modules or builds.

- For example, ==we collect the customer’s requirements, now instead of making the entire software at once, we first take some requirements and based on them create a module or function of the software and deliver it to the customer==. ==Then we take some more requirements and based on them add another module to that software==.
- Similarly, modules are added to the software in each increment until the complete system is created. However, the ==requirements for making a complex project in multiple iterations/parts should be clear.==
- If we understand the entire principle of Incremental methodology, then ==it starts by developing an initial implementation, then user feedback is taken on it, and it is developed through several versions until an accepted system is developed==. Important functionalities of the software are developed in the initial iterations.

### Advantages of Incremental Model

- Important modules/functions are developed first and then the rest are added in chunks.
- Working software is prepared quickly and early during the [software development life cycle (SDLC)](https://www.geeksforgeeks.org/software-development/).
- This model is ==flexible and less expensive to change requirements and scope.==
- The customer can respond to each module and provide feedback if any changes are needed.
- ==Project progress can be measured.==
- It is easier to test and debug during a short iteration.
- Errors are easy to identify.

### Disadvantages of Incremental Model

- ==Management is a continuous activity that must be handled.==
- Before the project can be dismantled and built incrementally,
- The complete requirements of the software should be clear.
- This requires good planning and designing.
- The ==total cost of this model is higher==.

## RAD Model
Diagram for reference
![[Process Model Slide Set 3 (1).pdf#page=17&rect=95,41,658,398&color=yellow|Process Model Slide Set 3 (1), p.17]]
RAD model stands for ==rapid application development model==. The methodology of RAD model is ==similar to that of incremental or waterfall model==. It is used for small projects.

- If the ==project is large then it is divided into many small projects== and these small projects are planned one by one and completed. In this way, ==by completing small projects, the large project gets ready quickly==.
- In RAD model, the ==project is completed within the given time== and all the requirements are collected before starting the project. It is very fast and there are very less errors in it
### Advantage of RAD Model

- ==It reduces the time taken in development==.
- ==In this the components are reused==.
- It is flexible and it is easy to make any changes in it.
- It is easy to transfer like scripts because high level abstraction and intermediate codes are used in it.
- There are very few defects in it because it is a prototype by nature.
- In this, productivity can be increased in less time with less people.
- ==It is cost effective.==
- It is suitable for small projects.

### Disadvantages of RAD Model

- In this ==we need highly skilled developers and designers==.
- It is very difficult to manage.
- ==It is not suitable for project that are complex and takes long time==.
- In this, feedback from the client is required for the development of each phase.
- Automated code generation is very expensive.
- ==This model is suitable only for component based and scalable systems==.

## Prototyping
Diagram for reference
![[Process Model Slide Set 3 (1).pdf#page=18&rect=182,46,581,387&color=yellow|Process Model Slide Set 3 (1), p.18]]
Prototype model is an activity in which prototypes of software applications are created. First a prototype is created and then the final product is manufactured based on that prototype.

- The ==prototype model was developed to overcome the shortcomings of the waterfall model==.
- This ==model is created when we do not know the requirements well.==
- The specialty of this model is that this model can be used with other models as well as alone.

One problem in this model is that if the end users are ==not satisfied with the prototype model, then a new prototype model is created again, due to which this model consumes a lot of money and time==.

### Advantages of Prototype model

- Prototype Model is ==suggested to create applications whose prototype is very easy and which always includes human machine interaction within it==.
- When we know only the ==general objective of creating software, but we do not know anything in detail about input==, processing and output. Then in such a situation we make it a Prototype Model.
- When a software developer is not very sure about the capability of an algorithm or its adaptability to an operating system, then in this situation, using a prototype model can be a better option.

### Disadvantages of Prototype model

- When the first version of the prototype model is ready, the customer himself often wants small fixes and changes in it rather than rebuilding the system. Whereas if the system is redesigned then more quality will be maintained in it.
- ==Many compromises can be seen in the first version== of the Prototype Model.
- Sometimes a software ==developer may make compromises in his implementation, just to get the prototype model up and running quickly, and after some time he may become comfortable with making such compromises and may forget that it is completely inappropriate to do so==.

## Spiral Model
Diagram for reference
![[Process Model Slide Set 3 (1).pdf#page=19&rect=143,45,653,395&color=yellow|Process Model Slide Set 3 (1), p.19]]
Spiral model is a [software development process](https://www.geeksforgeeks.org/software-development-process/) model. ==This model has characteristics of both iterative and waterfall models==. This model is used in projects which are ==large and complex==. This model was named spiral because if we look at its figure, it looks like a spiral,
A software ==project goes through these loops again and again in iterations==. After each iteration a more and more complete version of the software is developed. The most special thing about this model is that risks are identified in each phase and they are resolved through prototyping. This feature is also called Risk Handling.

### Advantages of Spiral Model

- If ==we have to add additional functionality or make any changes to the software, then through this model we can do so in the later stages also==.
- Spiral model is ==suitable for large and complex projects==.
- It is easy to estimate how much the project will cost.
- ==Risk analysis is done in each phase of this model==.
- The customer can see the look of his software only in the early stages of the development process.
- Since continuous feedback is taken from the customer during the development process, the chances of customer satisfaction increases.

### Disadvantage of Spiral Model

- This is the most complex model of SDLC, due to which it is quite ==difficult to manage==.
- This model is not suitable for small projects.
- The ==cost of this model is quite high==.
- It requires more documentation than other models.
- ==Experienced experts are required to evaluate and review the project from time to time.==
- Using this model, the success of the project depends greatly on the risk analysis phase.

# Iterative VS Incremental Model
![[Process Model Slide Set 3 (1).pdf#page=20&rect=98,54,682,390&color=yellow|Process Model Slide Set 3 (1), p.20]]

## Concurrent Model


## Unified Process
The **Unified Process (UP)** is a software development framework that ==organizes the software development lifecycle (SDLC) into distinct phases and activities==. It is ==iterative and incremental== in nature, which means the project is developed through repeated cycles (iterations), and its features are improved incrementally.
Phases
![[Process Model Slide Set 3 (1).pdf#page=24&rect=95,55,638,398&color=yellow|Process Model Slide Set 3 (1), p.24]]
Reference for those phases
![[Process Model Slide Set 3 (1).pdf#page=25&rect=82,11,684,402&color=yellow|Process Model Slide Set 3 (1), p.25]]

## Agile
Agile model is a combination of ==iterative and incremental models==, that is, it is made up of iterative and incremental models.

- In Agile model, ==focus is given to process adaptability and customer satisfaction==.
- In earlier times, iterative waterfall model was used to create software. But in today’s time developers have to face many problems. The biggest problem is that in the middle of software development, the customer asks to make changes in the software. It takes a lot of time and money to make these changes.

> So to overcome all these shortcomings, the agile model was proposed in the 1990s.

The ==agile model was created mainly to make changes in the middle of [software development](https://www.geeksforgeeks.org/software-development/)== so that the software project can be completed quickly.

# Table 1: When to use which model
| **Model**         | **Best Used When**                                                                                         | **Not Suitable When**                                                                                 |
|-------------------|-----------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| **Waterfall Model**| - Project requirements are clear and well-documented from the beginning                                    | - Requirements are not clear or are expected to change during the project                              |
|                   | - Small or simple projects                                                                                 | - Complex, long-term projects with evolving requirements                                               |
|                   | - Sequential process without the need for iteration                                                        | - Need for early testing or feedback                                                                    |
| **V-Model**       | - Testing needs to be associated with each development phase                                               | - Projects with unclear or changing requirements                                                        |
|                   | - Small to medium-sized projects where requirements are stable                                             | - Complex projects or ongoing developments requiring flexibility                                        |
|                   | - Early detection of defects is important                                                                  | - Projects that demand high flexibility or iterative development                                        |
| **Incremental Model**| - Project can be broken into smaller parts, with early functionality deliveries                          | - Poorly defined or unclear requirements                                                               |
|                   | - Customer feedback is needed after each module delivery                                                   | - Requires extensive upfront planning and design                                                       |
|                   | - Important features need to be delivered quickly                                                          | - When incremental development isn’t possible due to interdependencies among components                  |
| **RAD Model**     | - Small to medium-sized projects that require rapid development                                             | - Large, complex projects requiring thorough planning                                                  |
|                   | - When high modularity and reusability of components are critical                                           | - Projects without highly skilled developers or that lack client feedback availability                  |
| **Prototype Model**| - Requirements are unclear and need refining through experimentation                                       | - Well-defined, detailed requirements exist from the start                                             |
|                   | - User feedback is necessary to define functionalities                                                     | - When changes are costly or infeasible after the initial prototype                                     |
| **Spiral Model**  | - Large, complex projects with significant risks                                                           | - Small projects                                                                                       |
|                   | - Projects where risk analysis and risk management are essential                                           | - Projects with a limited budget or simple requirements                                                 |
| **Unified Process**| - Iterative and incremental development are needed                                                         | - Projects requiring rapid, ad-hoc development                                                          |
|                   | - Project phases and roles are clearly defined                                                             | - Projects lacking clear requirements                                                                  |
| **Agile Model**   | - Requirements are expected to change during development                                                   | - Projects with fixed, well-defined requirements                                                        |
|                   | - Customer involvement is frequent, and adaptability is important                                          | - Large projects where detailed documentation and strict schedules are necessary                       |
| **Concurrent Model**| - Multiple activities need to be executed simultaneously                                                  | - Sequential process is needed for simplicity                                                          |

# Table 2: Additional Features to Decide Which Model to Choose
| **Feature**                | **Description**                                                                                          | **Which Models It Favors**                                                    |
|----------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| **Project Size**            | Small, medium, or large project sizes influence the choice, as some models handle complexity better than others. | - **Small projects**: Waterfall, V-Model, RAD, Agile                          |
|                            |                                                                                                          | - **Large projects**: Spiral, Unified Process, Incremental                    |
| **Clarity of Requirements** | If requirements are clear from the start, sequential models work better. If requirements evolve, iterative models are preferable. | - **Clear requirements**: Waterfall, V-Model                                  |
|                            |                                                                                                          | - **Evolving requirements**: Agile, Incremental, Spiral, Prototype            |
| **Risk Management**         | Projects with high uncertainty or risk benefit from models that have built-in risk analysis mechanisms.  | - **High-risk projects**: Spiral, Prototype                                   |
|                            |                                                                                                          | - **Low-risk projects**: Waterfall, V-Model                                   |
| **Customer Involvement**    | Some models require frequent feedback from customers, while others follow a fixed process until the final delivery. | - **High involvement**: Agile, Prototype, RAD                                 |
|                            |                                                                                                          | - **Low involvement**: Waterfall, V-Model                                     |
| **Flexibility**             | Flexibility to adapt to changes mid-development is crucial in some projects, especially when requirements evolve. | - **Flexible models**: Agile, Incremental, Spiral                             |
|                            |                                                                                                          | - **Inflexible models**: Waterfall, V-Model                                   |
| **Time-to-Market**          | For projects where early delivery of a working product is essential, models with rapid development cycles are beneficial. | - **Rapid delivery**: Agile, RAD, Incremental                                 |
|                            |                                                                                                          | - **Slower delivery**: Waterfall, Spiral                                      |
| **Budget Constraints**      | Projects with strict budget constraints may prefer simpler, less expensive models. High-risk or complex models may require more resources. | - **Limited budget**: Waterfall, Agile, RAD                                   |
|                            |                                                                                                          | - **Higher budget**: Spiral, Unified Process                                  |
| **Team Size and Skill Level**| Projects with small or less experienced teams may need simpler, easy-to-manage models. Highly skilled teams can handle more complex methodologies. | - **Small teams/Low skill**: Waterfall, V-Model                               |
|                            |                                                                                                          | - **Experienced teams**: Agile, Spiral, RAD                                   |
| **Testing Requirements**    | Some models emphasize early and continuous testing, while others postpone testing until later stages.   | - **Continuous testing**: Agile, V-Model, Incremental                         |
|                            |                                                                                                          | - **Late-stage testing**: Waterfall                                           |
| **Documentation Needs**     | Some models require heavy documentation, while others focus on working software and customer collaboration. | - **High documentation**: Waterfall, V-Model, Spiral                          |
|                            |                                                                                                          | - **Low documentation**: Agile, RAD                                           |
| **Error Tolerance**         | Models that involve more frequent testing and iteration tend to handle errors better as they emerge.    | - **Error-friendly**: Agile, Incremental, Spiral                              |
|                            |                                                                                                          | - **Error-averse**: Waterfall, V-Model                                        |
| **Product Complexity**      | For projects with highly complex systems, models that allow iterations and revisions are crucial to success. | - **High complexity**: Spiral, Incremental, Unified Process                   |
|                            |                                                                                                          | - **Low complexity**: Waterfall, V-Model, RAD                                 |
| **Stakeholder Communication** | If frequent communication with stakeholders is needed throughout the development process, choose a model that encourages frequent feedback. | - **Frequent communication**: Agile, Incremental, Prototype, RAD              |
|                            |                                                                                                          | - **Infrequent communication**: Waterfall, V-Model                            |
