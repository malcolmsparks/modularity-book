# About the author

Malcolm Sparks has been thinking and writing about modular software
design since the mid 1990s.

In 1997, Malcolm began work on a modular workflow engine, using a
bespoke Java component model. In 1998, Malcolm adopted the newly
announced Enterprise JavaBeans specification as a standardised component
model and together with Peter Morgan built a complaint container and
server which was acquired by IONA Technologies the following year.

While at IONA, Malcolm continued his research into modularity, this time
focusing on the packaging and distribution of software components,
winning a company award for his Xsume packaging technology, which was
used in the packaging and distribution of IONA's second-generation
software portfolio. Xsume used dependency metadata to components and
their dependencies, across different languages and target platforms. It
enabled the packaging of software across engineering departments and
distribution of software, including updates and patches, via optical
media and the internet.

Upon leaving IONA in 2003, Malcolm distilled his ideas into a set of
patterns known as _PackageWare_ together with a website.

In 2004, Malcolm began consulting for a start-up, LeCayla, and together
with Eamon Walshe and Alan Spencer, built a system composed of over 140
separate components. Each component was managed as a separate project
within the IntelliJ IDEA IDE. A build system was also developed that
built components according to the dependency hierarchy inferred IntelliJ
project metadata.

In 2006, Malcolm consulted at the BBC and with James Parkin,
successfully developed a multi-departmental build system based on the
same ideas, this time using dependency information gleaned from the
Eclipse IDE project metadata. A reformulation of these ideas were
distilled to form CleanBuild, a modular build system used by a number of
companies.

In 2007, Malcolm joined a large investment bank and began working with
Maven. At the time, Maven's support for multi-module projects was
primitive but maturing. Malcolm helped to migrate many of the
departments systems to a mutli-module Maven build process. Meanwhile,
frustrated by Maven's rigid and prescriptive design, Malcolm continued
to work on CleanBuild, re-writing it in Kawa, a Scheme implementation
running on the JVM. This led him to adopt Clojure, once it had become a
viable alternative to Kawa. Malcolm continued to construct build
systems, but began to imagine software systems that would not need them.

In 2013, Malcolm left his employment in banking, and with Jon Pither set
up a JUXT, a Clojure consulting firm. While working for JUXT, Malcolm
has continued to research techniques for building modular software
applications. In 2013 he released _Jig_, a development harness for
building modular applications, while in 2014 he released _modular_ and
_Cylon_, collections of components based on Stuart Sierra's component
library.
