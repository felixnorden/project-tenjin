# Half-time presentation

## Introduction (First slide)

Although logic is essential in both everyday life and science, it is not formally taught until university. Every time you make an argument, or draw conclusions based on some information, you form a logical statement. Despite this fact, very few have been introduced to the subject. The reason is probably due to limited time and the wide range of subjects needed to be taught in compulsory school. This means that some subjects need to be prioritized over others.

However, adding logical reasoning to your toolbox early on might be beneficial in many aspects, both in other school subjects and in everyday life. For example, programming is beginning to be taught in compulsory school. But not having a grasp on logic when learning programming is like putting the cart before the horse. Taking this approach might also inhibit a deeper understanding of programming.

## Project Motivation (Second slide)

Puzzles have been a part of human recreation over millennia, which indicates that people enjoy being challenged in logical thinking. With the introduction of smartphones, puzzles have found a new home as games and are more accessible and engaging than ever before. However, quite few do proofs in logic calculi for the same stimulation.

This is where our project comes in. Because, it is often unknown that doing a proof in a formal calculus is very similar to playing a game. Therefore, providing a smartphone game modeled after logic and proofs might be an efficient way to expose people to the logical reasoning used when creating proofs.

## Project Ambitions (Third slide)

In this project, we strive to create a smartphone game that:

-  Is based on logic and associated proof rules. We aim to focus on propositional logic, leveraging the operations found in Sequent calculus.
-  Has an intuitive visualization which allows players to create proofs without a formal education in logic and proofs.
-  Has an infinite source of proofs, with varying difficulty, which are created by a proof generator.

## Crash course in Sequent Calculus (Fourth slide)

For our application we will focus on implementing the three main connectives Negation, Disjunction and Conjunction. There are other operators, such as implication, that could be implemented later. But these three are enough to model all logical statements in propositional logic.

In Sequent calculus you also make use of a “meta” implication, called the turnstile, in order to separate the hypotheses from the conclusion An example sequent might look something like this. In our application we will work from “upwards”, i.e we cannot create operators but only eliminate them according to certain rules. For example:

## Project Plan (Fifth slide)

In order to make the project more manageable and agile, we have decided on a plan consisting of three iterations:

- Barebone-phase - For constructing the foundation of the application.
- Minimal Viable Product-phase - For developing a useable baseline product.
- Bells and Whistles-phase - For stretch-goals, such as extensions and refinement.

### Barebone Phase (Sixth slide)

- (..) - We've stated that the visualization should be "intuitive" - but what does that actually mean? In order to accomplish the visualization, we need to research and define some key aspects of what intuitive design would mean for this game.
- (..) - The models we have chosen are based on previous experience. We have seen that the most valuable aspects of models are to define the problem domain, limit the scope of the project and to have a well-defined concept of how the application should function.
- (..) - Each of these prototypes will focus on one of the previously mentioned key aspects. The reason why we want more than one prototype is that we want to evaluate our hypotheses regarding "intuitive" design and also go with the visualization that yields the best results.
- (..) - Why we want to create one of the paper prototypes this iteration is so that we can design the user tests and begin testing as soon as possible.
- (..) - ...

### Minimal Viable Product Phase (Seventh slide)

- (..) - When we say "implement frontend" the goal is to simply connect the underlying model with a "placeholder" interface. I.e. connecting the model to the outside world. Why we chose to go with Unity™ is simple - it is one of the most widespread game development engines to date, with a large community and plenty tools and assets available.
- (..) - ...
- (..) - When all prototypes have been created and tested, we will choose the visualization that showed the best results.
- (..) - At this state of the project, we will also look at the possibilities of generating additional proofs for the application. Since we want to generate proofs based on difficulty, we need to concretize what properties determine the difficulty of a proof.

### Bells and Whistles Phase (Eighth slide)

- (..) - At this point, we plan to replace the "placeholder" interface with chosen application design.
- (..) - If we have found feasible properties for proof difficulty, and concluded that generating proofs should be possible, then we also plan to implement the proof generator.

## Project so Far (Ninth slide)

At this stage, we have created a Domain model and a Requirements analysis document containing a minimal set of Use cases for the first iteration.

Visualization-wise, we have two possible candidates - the proposed "Card game"-theme and our own "Space"-theme. For the latter, we have a small set of mockups and tested the visualization with quite a few visually-demanding examples. This was to verify that the theme would function properly for the majority of possible proofs.

We have also set up both the Unity-project and the Model-project using C# and .NET.

And the class diagram is under construction!

## Space Theme
