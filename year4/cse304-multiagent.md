# Multi-agent Systems (CSE304)

Past papers are available at [../past-papers/cse304](../past-papers/cse304).

## Lecture 2

### Notion of an agent

* Def1: An *agent* is a computer system that is capable of **independent** action on behalf of its user or owner.
* Def2: An *agent* is a **computer system** capable of **autonomous action** in some **environment**, in order to achieve its **delegated goals**.

### Notion of multi-agent systems

* A *multi-agent system* is one that consists of a number of agents, which **interact** with one-another.
* In most general cases, agents will be acting on behalf of users with different goals and motivations.
* To unsuccessfully interact, they will require the ability to **cooperate**, **coordinate**, and **negotiate** with each other, much as people do.

### Agent Design

TBA

### Society Design

TBA

### Properties of Environments

* Accessible vs. inaccessible
* Deterministic vs. non-deterministic
* Static vs. dynamic
* Discrete vs. continuous
 
### Decisions and Actions

* The key problem for an agent is to decide which of its action to perform in order to best satisfy its(design) objectives.

### Intelligent Agents

* Reactivity: perceive environment, response quickly to changes 
* Pro-activeness: take goal-directed behavior 
* Social ability: interact with other agents
    * cooperation
    * coordination
    * negotiation


### Difference between objects and agents

* Objects encapsulate some states
* Objects communicate via message passing
* Objects have methods corresponding to operations that may be performed on this state
* 
* Agents embody a stronger notion of autonomy than objects - in particular they decide whether or not to perform an action on request from another agent
* Agents are capable of flexible behavior

## Lecture 3

### Agent Architectures

* An agent architecture defines:
    * key data structures
    * operations on data structures
    * control flow beteween operations
* hybrid agent combines best from *symbolic reasoning* agents and *reactive* agents 
    * symbolic reasoning: use explicit logical reasoning in order to decide what to do
    * reactive: ?

### Deductive Reasoning Agents

* Traditional approach to build AI systems (symbolic AI)
    * symbolic representation of environment and behavior
    * syntactic manipulation of symbolic representation
* symbolic representation -> logical formulae
* syntactic manipulation -> logical deduction (theorem proving)

Transduction Problem: the problem of translating the real world into an accurate, adequate symbolic description, in time for that description to be useful
Representation/Reasoning Problem: the problem of how to symbolically represent information about complex real-world entities and processes, and how to get agents to reason with this information in time for the results to be useful

...

## Lecture 4

### Practical Reasoning

* Practical reasoning is reasoning directed towards actions - the process of figuring out what to do
* Practical reasoning a matter of weighing conflicting considerations for and against competing options, where the relevant considerations are provided by what the agent desires/values/cares about and what the agent believes.
* Practical reasoning is different than *theoretical reasoning* (directed towards beliefs)
* Practical Reasoning = Deliberation + Means-Ends Reasoning
    * deliberation: deciding **what** state of affairs we want to achieve - the outputs of deliberation are **intentions**
    * means-ends reasoning: deciding **how** to achieve these states of affairs - the outputs of means-ends reasoning are **plans**
* Intentions & Desires:
    * Intentions are stronger in influencing actions, than desires
    * Intentions drive means-end reasoning
    * Intentions persist
    * Intentions constraint further deliberation
    * Intentions influence beliefs upon which practical reasoning is based


### Symbolic Representation of Beliefs, Desires and Intentions

* *B* a variable for current beliefs
* *Bel* set of all such beliefs
* *D* a variable for current desires
* *Des* set of all desires
* *I* a variable for current intentions
* *Int* set of all intentions

### Means-Ends Reasoning

* Means-ends reasoning is the process of deciding how to achieve an **end** (an intention an agent has) using the available **means** (i.e., the actinos an agent can perform)
* Means-end reasoning is better known as planning
* Planning is essentially an automatic programming

### Planner

* a *goal*, *intention* or *task*
* the current state of environment - the agent's *beliefs*
* the *actions* available to the agent
* As output a planner generates a *plan*

### Basic Control Structure for a Practical Reasoning Agent

A loop:

1. observes the world, and updates beliefs
2. deliberates to decide what intention to achieve
3. uses means-ends reasoning to find a plan to achieve these intentions
4. executes the plan

* Note: Doesn't it basically reinforcement learning?