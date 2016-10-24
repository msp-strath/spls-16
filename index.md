---
title: SPLS Nov '16
layout: default
---

## Scottish Programming Languages Seminar (SPLS)

### University of Strathclyde, 9 November 2016

### About SPLS

The Scottish Programming Languages Seminar is an informal meeting for
the discussion of any aspect of programming languages. The next SPLS
will take place on Wednesday 9 November at the University of
Strathclyde.

Information and updates about the November edition of SPLS will be sent
via the SPLS Mailing List.

### Time and place
12:00--17:45, 9 November, room 319, [McCance Building](https://goo.gl/maps/2JjoPR6FvY82), University of Strathclyde.

### Programme

|When   | What                                                                                          |
|-------|-----------------------------------------------------------------------------------------------|
| 12.00 | Lunch (provided)                                                                              |
| 13.00 | Consistency of Quine's NF using nominal techniques - Jamie Gabbay                             |
| 14.00 | Coffee                                                                                        |
| 14.30 | Relating Channels and Actor-based Languages in Concurrent Lambda-Calculi - Simon Fowler       |
| 15.00 | Provably Correct Transformation of Specifications into Programs - Martin Ward                 |
| 15.30 | Update on new SICSA Research Themes and funding - Katya Komendantskaya                        |
| 15.45 | Coffee                                                                                        |
| 16.15 | Type-Driven Design of Communicating Systems using Idris - Jan de Muijnck-Hughes               |
| 16.45 | The essence of Frank programming - Craig McLaughlin                                           |
| 17.15 | TBA                                                                                           |
| 17.45 | Pub                                                                                           |

### Abstracts

#### [Jamie Gabbay](http://www.gabbay.org.uk/) (Heriot-Watt)

##### Consistency of Quine's NF using nominal techniques

Naive set theory has one rule; naive sets comprehension: If φ is a predicate, then {a | φ(a)} is a set. This is inconsistent by Bertrand Russell’s famous observation of 1901 that {a | a ∉ a} ∈ {a | a ∉ a} if and only if {a | a ∉ a} ∉ {a | a ∉ a}.
Solutions proposed included Zermelo-Fraenkel set theory, simple type theory, and Quine’s New Foundations (NF). NF works by restricting comprehension to stratifiable formulae; those in which variables can be assigned ‘levels’, which are natural numbers, such that if a ∈ b occurs and a has level n, then b must have level n+1. Russell’s example is ruled out because a ∉ a cannot be stratified. Consistency of NF has been an open problem since it was proposed by Quine in 1937.  I will present a claimed proof of consistency of Quine’s NF (the paper is available from www.gabbay.org.uk/papers.html and on arXiv, and is under review). In use, NF feels more like a simple type theory than it does a set theory, and there are deep reasons for this which come out in my proof.  My proof, while ostensibly about set theory, is actually about applying ideas from rewriting and computing to ideas from set theory, along with a pinch of non-Tarskian thinking about what binders (including forall and lambda) are. In my talk I will present the proof with an emphasis on the implications that this specific result has more generally for the theory of computing.

#### [Simon Fowler](http://simonjf.com/) (Edinburgh)

##### Relating Channels and Actor-based Languages in Concurrent Lambda-Calculi

To aid the development of highly-concurrent and distributed systems,
communication-centric programming languages take communication and
concurrency to be central to their design.
Programming languages such as Go provide anonymous processes which communicate
using typed buffers known as channels, whereas programming languages such as
Erlang are related to the actor model of concurrency, providing addressable
processes with a single incoming message queue.

The relationship between the two models remains a source of confusion, and the
lack of a common representation makes it difficult to reason formally about the
translations that exist in the folklore.
Building on concurrent λ-calculi, we define a calculus λch for typed asynchronous
channels, and a calculus λact for type-parameterised actors.  We then show
translations from λact into λch and λch into λact, and prove
that both translations are type- and semantics-preserving.

(joint work with Sam Lindley and Philip Wadler)

#### [Martin Ward](http://www.tech.dmu.ac.uk/~mward/) (De Montfort University)

##### Provably Correct Transformation of Specifications into Programs

This talk will introduce the transformational programming method
of algorithm derivation. This starts with a formal specification
of the result to be achieved, plus some informal ideas as to what
techniques will be used in the implementation.
The formal specification is then transformed into an implementation,
by means of correctness-preserving refinement and transformation steps,
guided by the informal ideas.

With this approach, loops can be introduced and manipulated
while maintaining program correctness and with no need
to derive loop invariants.  At every stage in the process
we are working with a correct program: so there is no need
for a separate "verification" step.

These factors help to ensure that the method is capable of scaling
up to the development of large and complex software systems.

#### [Jan de Muijnck-Hughes](https://jfdm.github.io/) (St Andrews)

##### Type-Driven Design of Communicating Systems using Idris

The idea of communicating systems is a cornerstone of modern technology that allows heterogeneous collections of components to communicate through well-defined communication patterns.
However, there is a disconnect between the tooling and languages used to design, implement and reason about communication protocols.

Idris is a general purpose programming language that supports full-dependent types, providing programmers with the ability to reason more precisely about programs.
Inspired by work on Session types, our research looks to leverage dependent types to describe and reason about secure communication patterns and their implementation in different communication contexts.

This talk presents our current progress and introduces *sessions*, a library for describing, and reasoning about, the interactions of a communicating system.
Demonstrated is use of *sessions* to describe common communication patterns, and how the library enforces correctness of the pattern itself through type-level guarantees.

Given time future work will also be presented detailing our next steps in linking these descriptions to implementations such that compile time correctness guarantees over the actions of an entity in a communicating system can be given respective to a known specification.

#### [Craig McLaughlin](http://homepages.inf.ed.ac.uk/s1544843/) (Edinburgh)

##### The essence of Frank programming

Frank is a strict functional language supporting algebraic effects
(a la Plotkin & Power) and handlers (a la Plotkin & Pretnar) within an
effect
type system. Key to the design is the generalisation of functions to
*operators* which may handle effects by pattern matching on computation
trees. Operators are n-ary allowing the simultaneous handling of multiple
computations. I will describe the key features of Frank by way of example,
showing its similarities to regular functional programming and its
differences. I will highlight the conveniences afforded by some of the
design
choices, in particular achieving effect polymorphism while avoiding the need
to mention effect variables. I will describe the current implementation of
Frank and how we have leveraged existing technology in its
development. Finally, I will speculate on some future work. (Joint work with
Sam Lindley and Conor McBride to appear at POPL 2017.)

#### [Katya Komendantskaya](http://www.macs.hw.ac.uk/~ek19/) (Heriot-Watt University)

##### Update on new SICSA Research Themes and funding

### Registration

Please register using this [form](https://goo.gl/forms/Fngd3qYbwh4lDtjm2).

### Organizers

* [Bob Atkey](https://bentnib.org), University of Strathclyde
* [James Chapman](https://jmchapman.github.io), University of Strathclyde
* [Conor McBride](https://personal.cis.strath.ac.uk/conor.mcbride/), University of Strathclyde
* [Fredrik Nordvall Forsberg](https://personal.cis.strath.ac.uk/fredrik.nordvall-forsberg/), University of Strathclyde

### Acknowledgements

This meeting of SPLS has received financial support from the
[Theory, Modelling and Computation theme](http://www.sicsa.ac.uk/research/theory-modelling-computation/)
of the [Scottish Informatics and Computer Science Alliance](http://www.sicsa.ac.uk/).

![SICSA logo](sicsa_blue.jpg "SICSA logo")
