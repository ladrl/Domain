How to design an interface?
===========================

What is the objective of an interface?
--------------------------------------

To allow the application to be divided into independent parts. What parts 
can be imagined?

 - Business
   The operations which deliver the 'business value'. 
   
 - Input
   The operations which convert events/data from the outside into the business domain
   
 - Output
   The operations which convert events/data from the business domain to the outside
   
Which of these parts can/should be reusable?
--------------------------------------------

Ideally, all of them. The current state is that there is no reusability of parts 
on such a granularity. The reuse is made on a lower level of abstraction, in the
for of libraries.


 
My thoughts
-----------
It should be possible to make this parts reusable. But: There are different
scopes for reuse. The domain of the interface defines in which scope the 
reuse lies - this could be in a particular business domain, but it could 
as well be in some GUI scenario.

So, an interface is tied to a particular domain. This has as a consequence that
it must be clear what the domain is and how it is structured to be able to define
a sensible interface for it. The interface must express the functionality in 
the language/terminology of the domain _only_. 

To be able to do this, the domain must be defined in some 'well-known' manner. As
for design patterns, there should be a similar description of a domain, listing
its purpose, its terminology, its tradeoffs, etc. It would be great to define
a domain as a language construct and to relate the interfaces to this, thus 
enabling checking by compilers. But I think I leave this for later...