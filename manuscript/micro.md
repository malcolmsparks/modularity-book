# Micro-modularity

For our discussion of increasing modularity in the context of a single
process we shall use the Clojure programming language to discuss and
build the central ideas and techniques.

## Why Clojure?

In our treatment of computer programs as graphs we are particular
concerned with the avoidance of _side-effects_.

Side-effects, in computer systems, are unexpected behaviours that are
caused by the breakdown of the abstraction we are using to instruct the
computer. They are 'holes' in logical façade we erect to avoid dealing
with the low-level implementation details of a computer.

Side-effects imply the existence of 'hidden' edges in our graph, ones
that have no respect for the boundaries we draw between our clusters and
can thwart our attempts to reduce coupling.

Clojure represents a significant breakthrough in the design of computer
languages in that it provides _functional data structures_, offering
programmers greater scope to avoid side-effects in their
functions. While most functional programming languages encourage the
development of 'pure' functions operating on values, Clojure
significantly deepens the choice of data structure that can be passed to
and from functions as values. In Clojure, rich data structures including
collections, sets and maps (association sets) behave as if they were
values - operations on them in no way affect the original value.

While Clojure is not unique in offering 'functional data structures',
ensuring their ubiquity by the exclusion of alternative 'mutable'
choices is a key constraint not found in most other functional
languages, with the exception of Haskell (or one from its family of
descendants). Yet Haskell is chiefly concerned with the orthogonal
theory of types. For the purposes of this discussion on modularity,
therefore, we prefer to focus on the connectedness of edges rather than
their legality.
