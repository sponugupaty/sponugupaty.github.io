# Management : Program Management

Taken from a typical job description:

1. TOC
{:toc}

## Inventing Things
## Work with leadership , engineering and service owners
## Define and develop roadmaps
  - Roadmaps are a tool to think beyond the next few sprints
  - they help us to plan , communicate and to get buy in 
  - this would also mean that the teams are aligned , can focus on executio and hit long term goals
  - key sections of a roadmap document which can vary from 3-12 months plan 
    - Primary focus 
    - Deliverables 
    - Out Of Scope 
    - known risks
    - request to other teams 
    - current status 
   - Why create a product roadmap?
      - Lead → set clear goals for the org to get behind.
      - Plan → enumerate deliverables and timelines to achieve those goals.
      - Communicate → get buy in, set accountability, and align the org.
      - Deliver → create a reliable cadence for shipping, build confidence
   - How do I go about writing a quarterly roadmap?
    - Gather ideas 
    - Write broad roapmap 
    - Meeting with Engineering
    - Meeting with stakeholders 
    - Get Signoff 
      
  - [Product Roadmap](https://goberoi.com/on-writing-product-roadmaps-a4d72f96326c)

## Managing multiple projects 
  - Make ure plan , process and responsibilities are clear 
  - Make sure goals , schedules and who is responsible is clear
  - Ensuring that templates are clear for each of the projects leads 
  - priorotise projects based on impacts 
  - look at work across projects to balance orkloads and timelines
  - Adjust schedules to maximise team productivity 
    - stagger start dates for similar projects 
    - flag duplicates 
    - look for dependencies
  **reference**
  [Managing Multiple Projects](https://asana.com/resources/managing-multiple-projects)
  
## Understand customer needs 
  - One of the most famous frameworks is "Jobs To Be Done"framework 
  - What job is your product hired to do ?
  - Which progress is the customer trying to make in a given circumstance 
  - To inovate - start with customer struggle and not need 
  - Since the need is always archetyped on the existing world 
  - Minimize ( direction) + {the time OR the likelihood} ( metric) + object of control + [optional contextual clarifier].
  
  **References** 
  [Jobs To Be Done](https://uxdesign.cc/job-to-be-done-to-understand-customer-personas-better-3963eff273f8)
  [Jobs To Be Done](https://jtbd.info/great-innovators-start-with-customer-struggles-not-customer-needs-7f9a4fd9412a)
  [1 Key Construct](https://medium.com/frameplay/the-one-construct-you-need-to-describe-customer-needs-f5f8e6bc89ae)
  
## Define clear projects plans 
## Leading a software project
  - The key responsibilities of a project "Directly Responsible Individual"
  - Making sure the project is successful 
  - At a high level the responsibilities of a project DRI are 
    - **Decision Making** - Having a consultative decision making framework , being willing to move ahead 
      even when you dont have all the details 
    - **Intra Team Communication** - Priorotizing and splitting the tasks , set up a cadence for team to collaborate
      feeback mechanism ( project kickoffs and retros )
    - **Stakeholder Communication** - Who are the stakeholders and how do I communicate with them at the right detail
    - **High Level thinking** - Asking the hard questions , defining goals and getting the buy-in , thinking 3 steps to anticipate the          next roadblock 
    - **Technical Execution** - Writing a spec to get feedback and align work , scoping and sequencing tasks , ensuring the project           meets the quality bar , tracking cleanup work and future feature requests 
    - **TODO**   
    
 **References**
 [Blog](https://medium.com/@zhangela/how-to-lead-a-software-project-d59ab391dec8)



## Scoping Projects
- Scoping isnt something that you think about for 1 day and never think about it 
- You need to pay attention to scoping throughtout the project 
- Planning Phase : Early stages of defining the project and its goals 
- Scoping Phase : Where you plan for and estimate all the work that needs to happen 
- Execution Phase : where the works gets done 
- Details of **Planning Phase** 
  - Define very specific goals for the project which helps control feature creep
  - Explicitly defining anti-goals also helps ( todo : **Examples**)
  - dividing the scope into must-haves and nice to haves is also a good way 
  - Minimise the batch size of the project 
    - Having clear milestones and checkpoints in the project 
    - Making it launching only part of the project easy 
  - De-Risk the project as soon as possible 
    - Tackling the riskiest part of the project first 
    - Prototying the riskiest parts of the project first 
    - Typically external subsystems add the most risk to a project
  - Optimise for the total impact rather than amount of work done 
  - Avoid re-write of a system 
    - We tend to undeestimate the amount of time taken 
    - Tempted to add new features and improvements 
    - Build an overly complicated system since we are overly focused on the shortcomings of the first system
  - Details of **Scoping Phase**
    - Only engineers working on the code should scope 
    - Dont underestimate amount of work needed 
    - Divide the project into smaller tasks <5 days ideally 
    - Define measureable goals to get to the project milestones 
    - Think of project estimates as probability estimates . 50% chance we will be done in 4 weeks and 90% in 8 weeks
    - Use historical data 
    - timebox open ended questions of the project 
    - Add Buffer 
  - Execution Phase 
    - Re-scope regularly based on the planned vs actual time taken 
    - Use milestones to answer the question - Hows the project going 
    - If project slips , ensure that everyone understands why the project slipped 
      - Prepare a revised and realistic plan of the project plan

**References**
[Scoping](https://www.freecodecamp.org/news/how-to-effectively-scope-your-software-projects-from-planning-to-execution-e96cbcac54b9/)

## Execute to high expectations in rapindly changing environment 
  - https://sloanreview.mit.edu/article/three-meaningful-strategies-for-managing-rapid-change/
  - 
## Glue that is able to prioritize and manage dependencies across teams
  - https://www.girlsguidetopm.com/dependencies-and-constraints-an-introduction/
  - https://engineering.linkedin.com/blog/2018/09/managing-software-dependency-at-scale
  - https://thedigitalbusinessanalyst.co.uk/how-to-manage-dependencies-1551355b9025

## Dive deep to gather requirements from appropriate stakeholders
- **Requirements Engineering**
  - 4 step process 
    - Feasibility - Is the system useful for the business 
    - Elicitation And Analysis - Discovering requirements 
    - Specification - Convert requirements into standard format 
    - Validation - Is this what the business needs 
  - In real life is not a sequential process , but an iterative one with activities interleaved 
  - Requirements typically are at 2 levels of details for different readers 
  - User requirements : Describes in plain english the functions that system would provide and the constraints under which they operate
  - System Requirement: Detailed description of the system services and the operational constrains such as how the system will be used,     and development constrains such as the programming languages
  - System Requirements further classified into functional and no-functional requirements 
    - Functional Requirements: 
      - Main functions that the system would provide 
      - Primarily , inputs , processing and output 
    - Non functional 
      - Constraints provided on the system 
      - Sometimes non-functional requirements more important than functional since no workaround
      - They also need to be measurable 
      - Typically of one of these categories - Speed , Size , ease of use , robustness , portability
 - **Feasibility Study**
  - Identify whether the system is worth implementing and if it can be implemented under the current constraints of budget, technical       skills, schedule, and if it does contribute to the whole organization objectives or not, etc.
  - The input to the feasibility study is a set of preliminary business requirements, an outline description of the system and how the        system is intended to support business processes
  - The results of the feasibility study should be a report that recommends whether to go forward to the next process or you won’t be       able to implement the software at all
 - **Requirement Elicitation & Analysis**
 - It’s a process of interacting with customers and end-users to find out about the domain requirements, what services the system should    provide, and the other constrains.
 - Has 4 major steps 
  - **Requirements Discovery** : Interacting with stakeholders to gather high level requirements 
  - Interviews , Prototypes , Scenarios are some of the techniques 
  - Can be a difficult process since users dont always know what they want 
  - Interviews can be open-ended ( no set questions ) and close-ended( pre-defined set of questions)
  - **Requirement Classification & Organisation** : Tie all related requirements together 
  - **Requirement Priorotisation and Negotiation** : Conflict resolution 
  - **Requirements specification** : Convert into specified formats 
  - Specification should be clear , consistent and complete
  - **Requirements Validation** : different types of checks
    - Validity Checks - Funtions expected vs offered
    - Consistency Checks - No duplicated 
    - Completeness check - All requirements and constraints 
    - Realism Check : Is this practical 
    - Verifiability - Can it be tested 
  
  **Reference**
  [Requirements Engineering](https://medium.com/omarelgabrys-blog/requirements-engineering-introduction-part-1-6d49001526d3)
  [Requirements Engineering II](https://medium.com/techcatch/how-to-confirm-the-requirements-elicitation-results-500d1fd49438)
  [Requirements Engineering III](https://medium.com/techcatch/correctly-conducting-elicitation-in-business-analysis-91dbabc888ba)
## Write clear, detailed level requirements
  - https://medium.com/@karlwiegers/how-detailed-should-requirements-be-d2bc951e9266
  - https://medium.com/@jackiebo/asanas-spec-template-spec-training-33bfd9d4dd32
  - https://www.joelonsoftware.com/2000/10/02/painless-functional-specifications-part-1-why-bother/
## Interact and communicate with project stakeholders throughout the lifecycle of the project
  - Even if you love your stakeholders , addition of each one of them slows the project
  - Ability to translate between domains - designer , business anayst , engineer and executive is critical 
  - TradeOff's between domains are critical for projects to be a success 
  - You need 4 things while dealing with diverse stakeholders 
    - **Shared Goal**
      - It takes effort o translate 
      - If there is no shared goal - each stakeholder sticks to their interests and biases causing the project to fail
      - When things get frustruating you can remind of the shared goal and why it is worth 
    - **Empathy**
      - Listening to what other person is saying and claryfying it even if it is incovinient 
      - Value different perspectives 
    - **Patience**
      - Often will deal with people who know less than you 
      - How you deal with the knowledge gap will be key to success
    - **Prevention and Recovery from Communication Breakdowns**
      - Get rid of wishful thinking 
      - Clarify if things are unclear 
   **References**
  - [Scott Berkun](https://scottberkun.com/2013/how-to-survive-and-thrive-with-multiple-stakeholders/)
  
  - Soft Skills To Engage Stakeholders 
    - Communication: Adjusts message to stakeholders
    - Negotiation & Conflict resolution :  The ability of negotiation and conflict resolution isn’t about just getting what you want,         but being able to listen, understand,challenge and manage expectations of stakeholders so that solutions can be sought.
    - Leadership : Understanding the motivations and thoughts of people around you 
    - Being a good team worker is always needed to achieve common goals, being able to fit the required roles, knowing when to                 contribute and when to listen
    - Good **team** workers utilising each others strengths and minimise their weaknesses, assisting in the development of each other by       sharing knowledge and experience
    - Being **decisive** requires being able to review options, anticipate risks and make them in a timely manner — you are taking                 responsibility for your decision
    - You need to have a sense of direction of project and think if we need to continue , delay or close
    - **Confidence** : Need to be able to commnicate confidently on a variety of topics
    - **Flexibility** : Build relationship of give and take 
    - **Ability to work under pressure**    
 **Reference**
 [Medium Article](https://medium.com/@James.lane/ultimate-soft-skills-to-engage-your-stakeholders-b65c46f52bba)
- https://www.darzin.com/stakeholder-management-ultimate-guide
  
  
  
  
## Resolve roadblocks through driving trade-off decisions to move work forward
  - https://fs.blog/2019/12/tradeoffs-decision-making/
  - https://medium.com/better-programming/technical-debt-and-tradeoffs-in-engineering-4a8696d8a95e
  - https://femgineer.com/2015/03/how-smart-tradeoffs-software-products-development/
## Define, measure and utilize project/program KPIs
  - KPI's in today's business world has become an misunderstood word with each interpreting them diffrently
  - KPI's are used to turn a vision into measurable goals 
  - KPI's trickle down to everyone in the company and become their goals
  - KPI's are useful since they clarify where the employees need to focus on 
  - 2 kinds 
    - High level KPI's for which the executive team is responsible for 
    - Front line KPI's that middle managers onwards are responsible for 
  - Tie KPI's to goals and avoid the KPI's being manipulated by having counter goals 
  **Reference**
  - [KPI's II ](https://medium.com/swlh/a-managers-guide-to-key-performance-indicators-kpis-75042180e094)
  - [25 KPi's](https://www.clearpointstrategy.com/25-important-project-management-kpis/)  
  - [OKR](https://medium.com/@radoshi/10-tips-for-using-okrs-effectively-1c9e84161a67)
  - [KPI's](https://medium.com/@meetfelipe/okr-vs-kpis-what-is-the-difference-ffa54673fcf1)
  
## Identify and drive continuous process improvements in the PMO
  - [Improvement](https://medium.com/hackernoon/prioritizing-non-feature-work-and-continuous-improvement-bad2a612d860)
  - [Improvement II](https://medium.com/hackernoon/how-does-your-company-approach-continuous-improvement-9fa7ec3545d3)
  - [Improvement III](https://medium.com/@kevingoldsmith/building-a-culture-of-continuous-improvement-a29531bfef4)


