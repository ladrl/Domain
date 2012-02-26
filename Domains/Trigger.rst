Trigger
=======

Name
----
 
Trigger
   
Context
-------

The base is a web of systems. In order isolate a sub-set of this web, a border has to be drawn through it. The isolation allows for 
a different abstraction inside the border. This is the driving factor for the isolation, since a change in the abstraction can enable
additional capabilities of the system, like resue.

 * Assumptions
 
   - There is the necessity for an abstraction gap
   
Purpose
-------

Isolating a system requires a border. This border needs gates to connect to it's around systems.
The trigger defines the behavior of these gates.
   
Challenge
>>>>>>>>>

There is a constant stream of information flowing to the isolated sub-system from it's around systems. These flows cross
the border using a gate. How does the gate decide when and what is allowed to pass?
The isolation of the system allows an abstraction gap. The trigger must accumulate the information necessary to bridge the
gap.
     
Solution
>>>>>>>>

The gate is equipped with a trigger, describing the rules controlling the behavior. This rule may access all data attempting to 
come through the gate and take its decision. If it decides that the data may pass, the gate will open. The rule is not able to
access the system behind the gate - thus it cannot be vetoed by it. In order to represent different states of acceptance from the 
around-systems, the system can install different triggers representing them.
  
Glossary
--------
   
 Gate
  A point of interaction on the border of a system. It allows data to flow into the system. It's behavior is controlled by the
  associated trigger. It enforces a certain structure of the data. (~~> This part is not in the scope of this domain, 
  but relates to another one... How should I handle this?)
  
 Trigger
  A bundle of rules and data used to decide if a block of data is allowed to pass. A trigger has a one to one relation with a 
  gate when it is installed on it.
 
 Abstraction gap
  The conceptional difference a border represents. This difference expresses itself in the usage of at least partially disjunct 
  domains on the sides of the gap.
 
 (Rule)
 
 Data
  Information in a certain structure directed at the system and terminating at a gate. The dimensions of this structure can be 
  arbitrary and can include time. One important attribute of data is that it needs to have a minimal structure, a chunking which
  seperates individual data chunks. (~~> Not clear, elaborate! )
 
 Chunk
  The structure of the data which indicates the completeness of the data, that it is ready to be judged by the trigger of the gate.
 
 Pass
  A chunk of data is allowed to pass when the trigger allows it after examination of the chunk.
 
 Install
  The name of the process which associates a trigger with a gate. If the gate already had a trigger, this is disconnected. If a 
  judgement of a chunk is already in progress, it is not disconnected until the decision is made.

 Border
  The conceptual line which is drawn to enclose a system which differs in abstraction from its surroundings.

Semantics
---------

A Gate allows data to pass through the border.
The decision to let data pass is taken on the data streaming to the gate by the trigger which is associated with the gate.
The data collected while taking the decision can extend the data streaming in and allows to bridge the abstraction gap.
A gate remains in place as long as the system lives, but the system can decide to install different triggers on its gates to reflect internal state.

..todo:: Add the semantics for all the glossary entries
