Domain
======

Name
----

Application domain
 
Context
-------

When faced with the need to split up a problem into composable sub-problems, one needs criteria and concepts
to decide where and how to divide. Each division must adhere to a common understanding
of these criteria and concepts, otherwise these divisions will be inconsistent and hard to understand.
The collection of these criteria and concepts form the base of the division-rationale.

Assumptions
***********

 - a problem can be split into sub-problems which then in turn can be composed to solve the initial problem
 - the criteria and concepts will make each sub-problem distinct from the other sub-problem    

Purpose
-------

Communicate the terminology and the semantics necessary to solve a certain

Problem
-------

Challenge
*********
Clearly identifying and describing the concepts and structures necessary to split up a problem into composable sub-problems.
   
Solution
********
Definition of a template with clearly defined sections and rules for the relations
between these sections. The relations are stated as rules about terms and must facilitate the 
description of the evolution of the domain out of its context. The terms introduced by the 
description of the solution of the domain must be defined in a glossary and be set into relation to 
each other in a semantics description.
   
Glossary
--------

Template :
  A document containing the structure and the rules to describe a domain.
   
Section :
  The structuring element of the template. It has a title, a purpose and is filled with some content. This content must adhere to the rules 
  stated for the section.
  
Rule :
  A set of constraints a section must fulfill. Each rule is formulated to ensure the evolution of the domain from 
  section to section.

Term :
  A name for a concept or a criteria
  
Domain :
  A name for the concepts an criteria making a sub-problem separate from the other sub-problems
  
Context :
  The description of conceptual environment a domain lives in
  
Glossary :
  A list of definition of terms. The definition creates a new term based on already known terms
  
Semantics :
  A list of rules the terms of the glossary follow. These rules allow reasoning using the glossary to come to conclusions phrasable in terms
  from the glassary.
  
Relation :
  A description of a concept which allows to reason about a set of terms. The relation itself is a term, as defined in this glossary, but 
  has the additional constraint of this term describing a set of terms.

Semantics
---------

 - A template is made up from a serie of sections.
 - Each section has an associated rule describing the constraints governing the section's content.
 - The individual sections have a fixed purpose and they build upon the preceeding sections.
 - Filling the sections builds a domain by defining its name, its context, its purpose in the form of a challange
   and a solution, its terms and their relations.
 - The final domain description contains the terms, the semantis and the evolution of the domain from its context which forms (hopefully) a complete model in
   the readers mind.


Annotations
-----------

As this is the domain description of domain, its inavoidable for it to be at least partly recursive.