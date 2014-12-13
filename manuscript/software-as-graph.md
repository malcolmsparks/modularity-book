# Systems represented as graphs

> Modularity is one measure of the structure of networks or graphs. It
> was designed to measure the strength of division of a network into
> modules (also called groups, clusters or communities). Networks with
> high modularity have dense connections between the nodes within
> modules but sparse connections between nodes in different
> modules. ... Biological networks, including animal brains, exhibit a
> high degree of modularity.

[http://en.wikipedia.org/wiki/Modularity_(networks)](Wikipedia)

Every computer program may be represented as a graph of nodes connected
by edges. Every call to a procedure, subroutine or library function can
be represented by an edge between the nodes representing the caller and
the callee.

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
say, reduce the count of edges between components.

The twin of coupling is _cohesion_. Cohesion is the measure of the
density of graph edges inside a component. We are comfortable when this
increases, because when we treat the system as a whole we see that an
_increase in cohesion_ is balanced by a _reduction in coupling_. Both are
indicators that we are increasing modularity.

_find some mathematical treatment of graph density_

### 'Micro' and 'macro' modularity

Modularity, as a property of a graph, can be measured at any level of
granularity. However, in practice it is useful to draw distinctions
between modularity within a single address space, modularity within a
set of processes on a single host, modularity within a set of locally
distributed processes (processes residing on multiple hosts attached to
a local network) and modularity within a set of geographically
distributed processes.

_expand section_
