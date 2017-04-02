### What is "Propositional Logic?" ###

Propositional calculus (also called propositional logic, sentential calculus, sentential logic, or sometimes zeroth-order logic) is the branch of logic concerned with the study of propositions (whether they are true or false) that are formed by other propositions with the use of logical connectives, and how their value depends on the truth value of their components.

Propositional calculus is first-order logic without variables or quantifiers

https://en.wikipedia.org/wiki/Propositional_calculus

Propositional languages cannot express the notion of "all". 
ex: Move All cargo from A to B

### What is "First Order Logic"? ###
First-order logic ( FOL )– also known as first-order predicate calculus and predicate logic – is a collection of formal systems used in mathematics, philosophy, linguistics, and computer science. First-order logic uses quantified variables over non-logical objects and allows the use of sentences that contain variables, so that rather than propositions such as Socrates is a man one can have expressions in the form "there exists X such that X is Socrates and X is a man" where there exists is a quantifier and X is a variable.[1] This distinguishes it from propositional logic, which does not use quantifiers.[2]

A theory about a topic is usually a first-order logic together with a specified domain of discourse over which the quantified variables range, finitely many functions from that domain to itself, finitely many predicates defined on that domain, and a set of axioms believed to hold for those things. Sometimes "theory" is understood in a more formal sense, which is just a set of sentences in first-order logic.

https://en.wikipedia.org/wiki/First-order_logic

### What is Situation Calculus? ###

The situation calculus is a logic formalism designed for representing and reasoning about dynamical domains.

The situation calculus represents changing scenarios as a set of first-order logic formulae. The basic elements of the calculus are:

Situation Calculus is FOL plus conventions for representing states and actions

1. The actions that can be performed in the world.
2. The fluents that describe the state of the world.
3. The situations.


A domain is formalized by a number of formulae, namely:
- Action precondition axioms, one for each action
- Successor state axioms, one for each fluent
- Axioms describing the world in various situations
- The foundational axioms of the situation calculus


A simple robot world will be modeled as a running example. In this world there is a single robot and several inanimate objects. The world is laid out according to a grid so that locations can be specified in terms of (x,y) coordinate points. It is possible for the robot to move around the world, and to pick up and drop items. Some items may be too heavy for the robot to pick up, or fragile so that they break when they are dropped. The robot also has the ability to repair any broken items that it is holding.

### What is PDDL? ###
Planning domain definition language

### What is a Fluent? ###

Statements whose truth value may change are modeled by relational fluents, predicates which take a situation as their final argument. Also possible are functional fluents, functions which take a situation as their final argument and return a situation-dependent value. Fluents may be thought of as "properties of the world"'.

In the example, the fluent is_carrying(o,s) can be used to indicate that the robot is carrying a particular object in a particular situation. If the robot initially carries nothing, is_carrying(Ball,S0) is false while is\_carrying(Ball,do(pickup(Ball),S0)) is true. The location of the robot can be modeled using a functional fluent location(s) which returns the location (x,y) of the robot in a particular situation.

Fluent = state variable. 5 fluents -> state spece has 2^5=32 states

what is SATPlan?