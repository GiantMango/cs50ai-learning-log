# Week 1 - Knowledge

## Quick Notes
Session 1:
Lecture 0:00 ~ 30:00
Learned about propositional symbols. Implication, biconditional, and entailment are new concept that I have to take in. Model checking is to check entailment. It enumerates all the possible worlds to see if when KB is true, query Q is also true.

Session 2:
Lecture 30:00 ~ 50:00
Learned about applying the propositional symbols to real world problems like puzzling, Clue, mastermind game.

Session 3: 50:00 ~ End
Learned about inference rules, which we draw new conclusions based on the knowledge there already exists. There are a bunch of inference rules like `And Eliminateion`, `Modus Ponens`, `Implication Elimination`, `De Morgan's Law`, etc... We can use these rules to convert a really long propositional logic to **conjunctive normal form (CNF)**, and with this form, we can then apply `resolution algorithm` to try to get to empty clause. This process is called `inference by resolution`. 



## Progress
- Completed lecture [2026-05-26].

## Key Concept
- **Propositional Logic and Symbols**
    - **And ($\wedge$)**
    - **Or ($\vee$)**
    - **Implication ($\rightarrow$)**
    - **Biconditional ($\leftrightarrow$)**
- **Entailment ($\models$)**: KB entails Q if an only if in all possible worlds where KB is true, Q is also true.
- **Model Checking**: Is the process of checking entailment.
- **Inference Rules$**: A set of rules which can be used to draw new conclusion based on the existing knowledge.
- **Resolution**: $\frac{(P\vee Q) \wedge (\neg P\vee R)}{(Q \vee R)}$
- **Conjunctive and Disjunctive**
- **Inference by Resolution**: 
- **First-Order Logic**: In first-order logic, there are two types of symbols - constant symbols and predicate symbols. It's a different way than propositional logic to describe things.


## What I've learned..

## Challenges

## Next Step