# Benefits

This chapter discusses the benefits of modularity in the design of
software systems.

In summary, benefits of increased modularity include :-

* Improved comprehension by individuals of individual entities and the
  system as a whole. A view of the architectural decomposition of the
  system is enabled by the explicit declaration of dependencies.

* The elimination of architectural dependency 'cycles' which inhibit
  software maintenance.

* Interchangeability of parts, thus improving adaptation to evolving
  environments and reducing the need for wholesale rewrites.

## Improved comprehension

> "Complexity is the enemy" (Fred Brooks)

_citation needed_

To understand why modularity is required in large software systems, we
must first understand the nature of complexity and its effect on our
software.

The reason complexity damages software is that it makes it harder for a
person to understand how the software works. Without proper human
comprehension of the whole system, maintenance becomes a risky endeavour
as human mistakes lead to system instability and ultimately failure. In
order to build yet larger systems, we need methods to control and manage
the growth of complexity.

### The role of consistency

When we attempt to comprehend a system we construct conceptual models in
our brains as a mental aid to remembering how each part of the system
works. A system that exhibits consistent abstractions and concepts is
highly compatible with our mental cognitive mechanisms and we take on
information about the system with ease. We begin to predict how other
parts of the system will work, based on the understanding we already
have. We build on these conceptual models, refining them where necessary
until we have achieved a working understanding, adequate for confidence
in making system improvements,

Systems that are inconsistent throughout require far more work on the
part of the developer to comprehend. Our mental models are discordant,
we are deluged in detail, which we soon forget.

Therefore we prefer designs for software that utilize patterns universal
throughout the architecture.

Modular applications make dependency relationships explicit. Therefore
it is usual to adopt a consistent pattern for an entity to resolve its
dependencies. There are different approaches. For example, dependency
resolution may be achieved indirectly via a component catalog or by
_dependency injection_, a method for connecting a component with its
dependencies at runtime.

To achieve consistency, we prefer that all dependency relationships are
resolved in a similar manner.

### Architectural visibility

_see 2 articles (in evernote) about this_
http://www.codingthearchitecture.com/2014/06/01/an_architecturally_evident_coding_style.html


## Reduction of dependency cycles

Despite great efforts to formalise software development, software is
still usually written _ad hoc_. After a few years of development, software systems are described by their owners with illustrative metaphors such as 'a great ball of mud', or 'spaghetti code'. This is often perceived by the system owners as an unfortunate accidental consequence of a flawed approach to development.

But that is precisely what any non-trivial software system is.

_balls of mud_

## Interchangeability

_the temporal aspect_


## Reuse

_ensure this is in the introduction_
_sync this with modular's README.md_
