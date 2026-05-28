# [Week 1 - Knowledge](https://cs50.harvard.edu/ai/weeks/1/)

## Progress
- Completed lecture [2026-05-26].
- Completed project 1 knight [2026-05-27].
- Completed project 1 minesweeper [2026-05-27].

## Key Concept
- **Propositional Logic and Symbols**
    - **And ($\wedge$)**
    - **Or ($\vee$)**
    - **Implication ($\rightarrow$)**
    - **Biconditional ($\leftrightarrow$)**
- **Entailment ($\models$)**: KB entails Q if an only if in all possible worlds where KB is true, Q is also true.
- **Model Checking**: Is the process of checking entailment.
- **Inference Rules$**: A set of rules which can be used to draw new conclusion based on the existing knowledge.
    - **Modus Ponens**
    - **And Elimination**
    - **Double Negation Elimination**
    - **Implication Elimination**
    - **Biconditional Elimination**
    - **De Morgan's Law**
    - **Distributive Property**
    - **Resolution**: $\frac{(P\vee Q) \wedge (\neg P)}{Q}$.
- **Conjunctive and Disjunctive**: conjunction is a bunch of symbols connected using And($\wedge$), while disjunction is a bunch of symbols connected using Or($\vee$). And **clause** is a disjunction of literals i.e. it could be $\neg P$, $P$, $Q$, $\neg Q$.
- **Conjunctive Normal Form (CNF)**: a conjunction of clauses. We apply inference rules to convert the propositional logic to CNF.
- **Inference by Resolution**: $\frac{(P\vee Q) \wedge (\neg P\vee R)}{(Q \vee R)}$. Q and R can be chained as $Q_1\vee Q_2\vee ...\vee Q_n$. If we get an **empty clause ()** $\equiv$ `False`. Why is it useful?
- **Entailment by Resolution**: Instead of enumerating all possible worlds and checking whether both the knowledge base and query are true, we can prove entailment by contradiction. To prove $KB \models Q$, we check whether $KB \wedge \neg Q$ leads to a contradiction. If resolution derives the empty clause, then $KB \wedge \neg Q$ is unsatisfiable, meaning there is no possible world where $KB$ is true and $Q$ is false. Therefore, $KB \models Q$.
- **First-Order Logic**: In first-order logic, there are two types of symbols - constant symbols and predicate symbols. It's a different way than propositional logic to describe things.


## What I've learned..
I had heard about propositional logic when I was in middle school. It sounded like just common sense. And after this lecture, I feel like logic can get very intimidating and complicated real quick. Think about the house.py, when we represent all the things with propositional logic, look how the output returns out. I came to this lecture not knowing what I would have seen. And this give me a new perspective to see through politicians lies. I didn't know we can tweak logics like this using all the inference rules. And what I used my brain juice the most was during the minesweeper project. I looked at the structure and try to understand how an AI is implemented in a simple game like this. I also did the same thing for the tictactoe project in week 0. I do find some similarities in these two projects. They both have a runner.py file to actually put up the game in pygame and shows the windows with the buttons and stuff. And in an additional file, tictactoe.py or minesweeper.py is the actual logic behind the game. Using object-oriented programming would help modularizing the algorithm and make them more maintainable and easier to debug.

## Challenges
Minesweeper project actually took me a lot of time. I think I spent like maybe more than 5 hours on it. The most difficult part was the add_knowlegde method in the MinesweeperAI class. It was the part where we have to compare the new added knowledge with the existing knowledge and infer new rules and I kept losing track on which sentence I've already added in the knowledge base or haven't. Updating the knowledge base with valid sentence was important. And cleaning the knowledge base was important, too. I thought my logic was proofing the duplicates and the empty sets but it wasn't. Additionally, finding a way to just debug the add_knowledge method was crucial. I had to add a piece of code at the end of the file under the “if __ name __ == '__ main __' statement. I also added some helper functions to find the surrounding cells and the possible moves on the board.

## Next Step
Start Lecture 2 Uncertainty.