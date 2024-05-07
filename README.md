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
