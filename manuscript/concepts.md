# Concepts

We start with a simple definition :-

> Modularity is the degree to which a system's components may be
> separated and recombined.

[http://en.wikipedia.org/wiki/Modularity](Wikipedia)

In this book we are concerned chiefly with software systems, and our
observations may not be universal.

## Components

We define a term to represent our graph cluster of densely connected
edges: a component. A component is a heavily used term in the software
industry, but most definitions broadly fit what we are describing
here. Many definitions of component also require some degree of
interface to define interactions between the component and other parts
of the system. We will address this in due course.

## Dependencies

Any directed edge between two components implies a dependency
relationship. We will discuss dependency relationships in a later
chapter.

## Interfaces

A dependency relationship is insufficient to define the interface
between two components. Interchangeability requires that we define
minimal agreements on how two components may interact. All modular
systems contain at least one common interface.
