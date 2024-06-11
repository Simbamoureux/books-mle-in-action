# books-mle-in-action

## What is a machine learning engineer ?

Use a system, set of standard tools, processes and methodology that aims to minimize the chances of failed ML projects. Those should prevent rework, confusion and complexity.

### Why ML Engineering ?

ML is *hard* ! Data Science knowledge doesn't help building  interfaces between the model solution and the real world. 

MLE needs to know *just enough* DE skills and Software skills to build & ship reliable systems. 

Why do projects fails ?

<img width="650" alt="Capture d’écran 2024-05-06 à 11 38 18" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/29d6d986-fd0f-4a1e-ad68-d1b790203ab7">

<img width="650" alt="Capture d’écran 2024-05-06 à 11 40 28" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/4db9ff80-3000-4fce-bd5f-6d89eaf67515">

### Core tenets of MLE

- Planning : Cause of failure of most ML Projects, adressing the wrong problem. You have to ask the right questions to ensure that you address the right problem. Focus on *what* will be built and *why* it needs to be built. Do not adress the *how* and *when* yet to avoid diverting from the business problem.
  * What would make this project a success ?
  * How is it done today if at all ?
- Scoping and research : The project can fail by doing too few scoping and research (and develop a useless solution) or too much also (and develop a good solution but for a budget and time that far outweights the business gains.
  * We need to compromise on those 2 approaches.
- Experimentation : Here also, we need to find a balance between over-experimentation and bad experimentation. The 2 cause ML projects to fail for different reasons.

<img width="732" alt="Capture d’écran 2024-05-06 à 11 56 57" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/082b87c7-6656-4525-b843-23cec3c92c52">

- Development : Same problem as in software engineering.
- Deployment : Always strive for the simplest design possible when building an architecture.
- Evaluation : If you can't justify the benefits in production of a ML product, it won't stay in production very long. A nearly flawless project can get cancelled if we can't justify how it contributes to the bottom line.
  * This is true for project with noticeable cost, if the cost is low enough, usually noone will notice.

### Goals of MLE

Use the process to deliver great ML projects ! ML that adresses a business problem, not the latest and greatest models, not the most shiny architecture. The goal is not a foolproof solution but a process that **increases the chances of a successful project** 

<img width="732" alt="Capture d’écran 2024-05-06 à 12 09 16" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/60eec623-e296-40b2-a5d6-dfd54f125aa8">

## Your data could use some MLE

### A foundation of simplicity

Focus on the simplest solution that solves the business's problem. **This concept is the foundation of MLE upon which all other aspects are built**. \
The only people that care on how a problem was solved are other data scientists, not stakeholders. A simpler solution has simpler maintenance.

<img width="732" alt="Capture d’écran 2024-05-07 à 11 44 40" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/607e6f76-d587-4143-8515-ff725b08d21d">

When you have to maintain solutions, complex, state of the art approaches lose their appeal because you're the one having to deal with this complex solution.

### Co-opting principles of Agile software development

Agile and Devops brought the world a demonstrable paradigm of successful engineering. Can we adapt this approach to DS work ?

<img width="732" alt="Capture d’écran 2024-05-07 à 11 50 06" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/db9ceb19-ecbf-427d-9a50-3192ad823546">

#### Communication and cooperation

A focus on people is necessary for successful ML work. This is even more true than for software work because of the complexity of what is being built, usually the layperson is very foreign to the result of ML/DS work and fitting the needs, and communicating is even more important than for software projects. \
2 biggest factors on the amount of **rework**: 
- Amount of collaborative involvement between the ML and business teams
- Amount of communication within the ML team
Lone wolf behaviour is *risky* for most projects.

<img width="732" alt="Capture d’écran 2024-05-07 à 11 54 52" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/90ee5f27-0bdb-441c-81e1-963f3cf768cd">

#### Embrace change

Be prepared for inevitable change to occur. Goals shift, assumptions are shown to be wrong. Sometimes even the use of ML to solve a problem can be put in question. \
Planning for this helps focusing on solving problems. This forces the team to work in a modular approach.

## Before you model : Planning and scoping a project

Contrary to academic setting : A company DS project is highly collaborative and peer-driven. *Focus more on the what than the how*. \
With adequate scoping, you have fewer **different approaches** to validate, which decreases the time spent building a solution.
- Early and often feedback needs to be received by the stakeholders.
- Also, each new feature development has a demo, and acceptance testing by the subject matter expert
  
<img width="767" alt="Capture d’écran 2024-05-14 à 11 19 34" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/75c9ced4-b132-42ad-b7b8-b553becdc358">

### Planning: You want me to predict what ?

Planning a project is not in contradiction with agile as long as the project plan is not too rigid to accommodate changes.

Don't blind trust your metrics : Do not rely on those metrics alone, supplement them with additional means of getting subjective measurements of the prediction's efficacy. Add vizualizations and demos. Validate results with SME, before larger demos with execs.

#### Basic planning for a project

**Why are we building this ?** Should be the main question of the first meetings. Answering this will define the expectations of the output of any ML work. It can also help with the measurement of the model's performance. \

This question should uncover assumptions of the business on how the solution should behave. e.g : The recommender system should exclude old items that are no longer in the catalog.
- assumption of business knowledge : The ML team often doesn't hold all the business knowledge necessary for the project -> Include SME in the loop !
- Assumption of data quality : The data isn't always reliable and uncovering all the quirks in the data can be accelerated by talking with SME that know the data and underlying concepts.
- Assumption of functionnality : Valid ideas for improvement always come from meetings with stakeholders to improve the model on things that are not linked to metrics
- Don't go "full nerd" : Assuming that people in the meeting understand the finer details of a solution as anything but a random collection of buzzwords is a disservice to yourself as an ML practitioner and to the audience. Use abstract terms, and link them to business outputs.

#### That first meeting

Don't think of implementation just yet ! Focus on the *why* and *what* rather than the *how*. 
Tips : 
- Try to understand what is being done now to address the problem : It often reveals a lot of useful requirements.
- Understand how the people work now on the problem

#### Plan for demos - Lots of demos

For most projects involving ML of sufficient complexity, far too many details and nuances exist to confidently build out dozens of features without having them reviewed. Only the ML team cares about the metrics, the SME will add another output to steer the work and improve actual usefulness of the project.

#### Experimentation by solution building: Wasting time for pride’s sake

It can be tempting to choose a few approaches and algorithms, and pit multiple people in the team to build the best solution, but the size of the batch is too big and need to be split in multiple phases with comparisons and demos (internally or with the cross functional team).

Divert resources on the most promising models so all the features can be built as fast as possible. Frequent demos even with features that are not finalized enables valuable feedback from SME, and narrowly focusing on the fewest and potentially most succesful options as early as possible allow a lean team to deliver successful projects.

<img width="767" alt="Capture d’écran 2024-05-14 à 12 17 32" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/e9391cc1-22f8-4120-9974-2e5a1e7ba2f4">

### Experimental scoping : Setting expectations and boundaries

Be clear about the expectations from experimentation. The goal is to produce a simulation of the end product that allows for unbiased comparison of the solutions considered.
At this stage you're interested by the performance of the solution and the dfficulty of developing the full solution.

What can be helpful is to use the first week or two to setup an experimentation testing plan that can be validated using a very simplistic model. To validate that we have an output and can evaluate it. This approach can help uncover complexities without spending first 4 weeks of data exploration etc...

Timeboxing experiments in sprints ensures that a decision can be taken quickly. Some DS could say that this is dumb, how can we really know if a solution is any good before tuning or working on it enough ? It's a fair point but this approach maximizes the amount on time spent on the final solution.
It's also less painful to throw away 2 weeks of work rather than 3 months.

<img width="767" alt="Capture d’écran 2024-05-14 à 14 00 38" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/39c930b1-37ed-4c4a-a2b4-0ad8de98e2d9">

How to define which experiments to run : 
- Brainstorm and list ideas
- Then score each one on risk and time to implement (low/medium/high)
- Work only on Low / medium risk and complexity ideas

**The goal of experimentation is to find the simplest approach that solves the problem, not use sophisticated tech**

At the end of this experimental phase, a PoC has been done, the solution is *understood* but not *implemented* yet.
You should then have identified risk factors and know : 
- How long will this take to build ?
- How much will this cost to run ?

To choose the best approach, you can weight the performance with the complexity, to obtain a final score where lowest is better.
<img width="767" alt="Capture d’écran 2024-05-14 à 14 46 08" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/fb23f1c4-14ed-40e3-ad97-7acc291378ce">

## Before you model : Communication and logistics of projects

Good tool : Communication path to understand a BU problem : 
- Why : Do you want this built ? (urgency / importance / will this be used ?)
- What do you expect the solution to do ? (basic functionnality / Scope of the project / Expected output)
- How is it done now ? (sucess criteria / Identifies SMEs / Critical features)
- What would be a perfect solution for this ? (accuracy expectations / realistic or attainable solution expectations)
- When would this solution become relevant ? (Is it worth doing ? If superseded by something else, maybe this should not be done)

Note that we don't talk about how we could do this just yet !

### Communication : Defining the problem

The scoping meeting should really focus on the why and not the how ! \n 
Keep in mind that the meeting is successful if the ML team gets the research and scoping details, but the business should get a review schedule. 

The other aspect of collectively discussing the project's key principles is to help define the simplest solution that solves the problem. 

<img width="630" alt="Capture d’écran 2024-05-28 à 11 45 33" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/f4904ea4-f1cd-4d76-8d0f-79d45d0730b8">

#### Understanding the problem

What can be useful to set expectations on how the system should work is to map user-focused journeys that are simple architectural focused journeys. \
Diagrams like this one are useful for conducting a planning discussion with a broader team. Breaking out the discussion from the point of view of the user includes even the non technical stakholders who will have insights.

<img width="548" alt="Capture d’écran 2024-05-28 à 11 52 41" src="https://github.com/Simbamoureux/books-mle-in-action/assets/18716146/0f450f0a-84d0-4364-ba63-14cdaf44ae17">

Don't ignore ideas, but also keep in mind that the MVP should not include Nice to haves, not every idea should make it into the experimentation plan.

Afterwards you can define the ideal end-state, and it is useful to understand what that could look like even if unfeasible.

**Scope creep** : If the discussion is flowing and ideas emerge, that's a really good thing but that leads also to a lot of ideas and the size and complexity of a project can spiral out of control. That's an almost certain assassination of a project. *ML Death by a thousand requests*

- Find a champion SME for the project ! To answer questions, help provide ideation. This should not be the executive or project owner !

#### Post research phase discussion (update meeting)

Don't discuss the implementation details of algorithms, don't mention the performances of algorithms that will take 2 years to build. Show the results in a manner that speaks to the business and distill the details needed for the next phase : Experimentation.
Show with each potential solution, what can and can't be done by the model and when can they expect a demo.

#### Post experimentation phase (SME/UAT Review)

Two prototypes are built. Lay the predictions out and show off what the solution looks like !
Show mockup of core features to the entire team but **don't do the full implementation**. You can also present an updated user-experience diagram. \ 
Every member of the team should now be aware of the elements and moving pieces. And ensures that the team understands which elements should be scoped.

#### MVP Review (Full demo with UAT)
- Code is tested
- The system functions as a whole in an evaluation environment with production scale data
- All agreed upon features that have been planned are complete and perform as designed

Metrics are useful but to really gauge a solution, when possible, a show of the actual result to the SME is best. Sometimes you can have discrepancies between the metrics and qualitative review of SMEs. This can uncover glaring issues not tracked by the metric.

Important : If you never have an issue during those demos meeting, it should setup an alarm, it may mean that the team has a confirmation bias, and showing the result to someone else in the company that has no stake in the project could help getting actual challenging reviews.

#### 4.2 Don't waste our time : Meeting with cross functional teams

- Experimental update meeting : Do we know what we're doing here ?
    - This is the second to last time for the team members to graciously raise a white flag if they've discovered that the solution is untenable.
    - The overriding question is "Can we actually figure this out ?". This is up to the DS team to report
    - We should share how is the progress toward the prototype coming along and what are the risks uncovered so far.
- SME review / prototype review : Can we solve this ?
    - Most critical meeting. Look for consensus on the recommended approach.
- Development progress reviews : Is this going to work ?
    - Opportunities to "right the ship" during development.
    - As development goes on, this meeting should be shorter and more focused on integration
- MVP Review : Did you build what was asked for ?
    - UAT by external team can bring a fresh view to the project
- Preprod review :
    - Everyone has one last chance to vet the built product "did we build what we set out to build?"
    - Compare original plans and final solution. Check that all the core features are here and work

#### Setting limits on your experimentation
