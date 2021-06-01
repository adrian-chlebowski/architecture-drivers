# Architecture drivers
This repository describes the architecture drivers that drive the direction of application development

## Functional requirements

How the application is supposed to work. 
These requirements state what the system must do, and how it must behave or react to runtime stimuli.

In order to design software, you need to know something about the goals that it needs to satisfy.
If this sounds obvious, it’s because it is. Having said that, I have seen teams designing software
(and even building it) without a high-level understanding of the features that the software should
provide to the end-users. Some might call this being agile, but I call it foolish. Even a rough, short
list of features or user stories (e.g. a Scrum product backlog1) is essential. Requirements drive
architecture.

## Quality attribute requirements

These requirements are qualifications of
the functional requirements or of the overall product. A qualification of a
functional requirement is an item such as how fast the function must be
performed, or how resilient it must be to erroneous input. A qualification
of the overall product is an item such as the time to deploy the product or a
limitation on operational costs e.g. testability, observability, reliability, scalability, availability, security, usability

Quality attributes are represented by the non-functional requirements and reflect levels of
service such as performance, scalability, availability, security, etc. These are mostly technical
in nature and can have a huge influence over the resulting architecture, particularly if you’re
building “high performance” systems or you have desires to operate at “Google scale”. The
technical solutions to implementing non-functional requirements are usually cross-cutting and
therefore need to be baked into the foundations of the system you’re building. Retrofitting high
performance, scalability, security, availability, etc into an existing codebase is usually incredibly
difficult and time-consuming.

## Constraints

Project constraints , project knowledge, how time is to implementation. 

A constraint is a design decision with zero degrees of freedom.
That is, it’s a design decision that’s already been made. Examples include
the requirement to use a certain programming language or to reuse a certain
existing module, or a management fiat to make your system service oriented. These choices are arguably in the purview of the architect, but external factors (such as not being able to train the staff in a new language, or
having a business agreement with a software supplier, or pushing business
goals of service interoperability) have led those in power to dictate these
design outcomes.

We live in the real world and the real world has constraints. For example, the organisation that
you work for probably has a raft of constraints detailing what you can and can’t do with respect
to technology choice, deployment platform, etc.

## Conventions

Where constraints are typically imposed upon you, principles conventions are the things that you want to
adopt in order to introduce consistency and clarity into the resulting codebase. These may be
development principles (e.g. code conventions, use of automated testing, etc) or architecture
principles (e.g. layering strategies, architecture patterns, etc). This means consistent solutions e.g. use a consistent user login library that is already used in your company


## Bibliography

- Software Architecture for Developers - Simon Brown
- Software Architecture in Practice - Len Bass, Paul Clements, Rick Kazman
