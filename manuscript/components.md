# Components

## Single Responsibility Principle

Since Turing proved that all approaches to computation are ultimately
equivalent, principles in software development has primarily concerned
themselves with the organisation of code.

One of the more enduring principles, one that is continually
rediscovered in various guises, is the Single Responsibility Principle
(SRP):-

_SRP definition_

By reducing the influence a piece of code has on other parts of
the program, it is easier to avoid the mistakes which lead to problems
with the software.

Dividing a system's responsibilities into components requires skill in
software design and no small degree of pragmatism, but fortunately
software often allows its practitioners room for error and the
opportunity to continually correct poor judgements later on.

# Abstraction

The determinstic nature of mathematics allows software systems to
comprise a vast number of individual parts.

Abstraction is an essential tool which lets developers focus on
individual areas of logic, in isolation from everything else that is
going on in the program. Without abstraction, the sheer number of
details would be overwhelming and the size of systems we could build
would be severly contrained.

_upper tiers must call the functions of lower tiers_

# Pure functions

Functional languages treat functions as first-class entities. Functions
can be passed as arguments and returned as values.

A pure function is one that operates solely on its arguments, such that
its result is predictable. If such a function is called two separate
times, but with the same arguments, it is guaranteed to return the same
result. Functions are easily composed together to create specific
functionality. Pure functions are determinstic, and as such are ideal as
building blocks for reliable functionality.

# I/O

To be useful, most programs must interact with the outside world.

_I/O tends to be low-level_

_But we don't want to have to the upper tier of functions have intimate details of the lower tiers contextual state_

_define inputs and outputs_

_formalise state-management: configuration (initial internal state)_
