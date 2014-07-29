# Introduction

We start with a simple definition :-

> Modularity is the degree to which a system's components may be
> separated and recombined.

[http://en.wikipedia.org/wiki/Modularity](Wikipedia)

When applied to software systems, this definition holds true.

> "Complexity is the enemy" (Fred Brooks)

_citation needed_

To understand why modularity is required in large software systems, we
must first understand the nature of complexity and its effect on our
software.

The primary way in which complexity damages software is in making it
harder for a person to understand how a system works. Without proper
human understanding, software maintenance becomes a risky endeavour as
human mistakes lead to system instability and ultimately failure. In
order to build yet larger systems, we need methods to control and manage
the growth of complexity.

> Modularity is one measure of the structure of networks or graphs. It
> was designed to measure the strength of division of a network into
> modules (also called groups, clusters or communities). Networks with
> high modularity have dense connections between the nodes within
> modules but sparse connections between nodes in different
> modules. ... Biological networks, including animal brains, exhibit a
> high degree of modularity.

[http://en.wikipedia.org/wiki/Modularity_(networks)](Wikipedia)

A computer program can be considered a graph, made up of nodes and
edges. Every call to a procedure, subroutine or library function creates
an edge between the caller and the callee. Whether by design or
otherwise, a graph is nevertheless created.

This book describes some architectural programming techniques that have
the aim of creating clusters within the graph that have high internal
edge density and low external edge density. The reasoning behind this
approach is the observation, in practice, that complexity in computer
systems tends to rise exponentionally with system size. Complexity is
subject to a network effect. While it can be possible to manage a degree
of complexity at a small scale, such management tends not to scale to
larger systems. Therefore, we need to break our large systems up into
small components and at the same time carefully manage the relationships
between them.

We define the term _coupling_ as the density of edges between
components. We continually look for ways to reduce coupling, which is to
say, reduce the densite of edges between components.

The flip side of coupling is _cohesion_. Cohesion is the measure of the
density of graph edges inside a component. We are comfortable when this
increases, because when we treat the system as a whole we see that an
_increase in cohesion_ is balanced by a _reduction in coupling_. Both are
indicators that we are increasing modularity.

_find some mathematical treatment of graph density_

## 'Micro' and 'macro' modularity

As a theory of graph construction, modularity can be considered at any
scale in-continuum. However, in practice it is useful to draw a somewhat
arbitary distinction between modularity within the confines of a single
(operating system) process, modularity within a set of processes on a
single host, modularity within a set of locally distributed processes
(processes residing on multiple hosts attached to a local network) and
modularity within a set of geographically distributed processes.

_expand section_

## Concepts

### Components

We define a term to represent our graph cluster of densely connected
edges: a component. A component is a heavily used term in the software
industry, but most definitions broadly fit what we are describing
here. Many definitions of component also require some degree of
interface to define interactions between the component and other parts
of the system. We will address this in due course.

### Dependency relationships

Any directed edge between two components implies a dependency
relationship. We will discuss dependency relationships in a later
chapter.

### Interchangeability

A dependency relationship is insufficient to define the integration
semantics (surface) between two components. Interchangeability requires
that we define more fully how components may interact. Protocols, which
define sets of externally callable functions, do a better (though
arguably incomplete) job. We will discuss protocols in a later chapter.


## Benefits

We will discuss the main benefits of increased modularity in a later
chapter.
