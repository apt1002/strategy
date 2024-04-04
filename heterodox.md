# Heterodox Technology

Many people[who?], who disagree on most things[which?], agree that they need
foundational software technologies that they can reach into and change.


## Big Tech versus society

Already it has become difficult to do many things without using software of
some sort. Without it:

- You cannot communicate.
- You cannot publish.
- You cannot organise.
- You cannot keep records.
- You cannot buy specialist goods, such as dance shoes.
- You cannot have a bank account.
- You cannot pay your taxes.
- You cannot even watch TV.

The old ways of doing these things still work, of course, but they are
relatively terrible, and increasingly unfamiliar. It cannot be long before
computers will be necessary for buying essential food and clothes, paying
utility bills, owning a house, and participating in politics.

Most people rely on software written by other people, and in particular by big
technology companies including Microsoft, Apple, Google, Meta, and others. The
downside of such a small group of companies having so much influence is
obvious, and I don't need to rehearse it here. However, it is an efficient way
to serve the mass market [it’s a local maximum], and I'm sure it will continue.

Many organisations need more control than that [than what? for what? most organizations use cloud-based subscription services from GAFAM, surely?], and require custom software [so they don’t require custom software].
The same is true of many creative individuals, including researchers, artists
and entrepreneurs. Such software is written to serve only thousands of people,
or even fewer. Often this software must be written by a specialist programmer,
who is not an expert in whatever purpose the software is supposed to serve.
This disconnect, and the shortage of specialist programmers, is a significant
expense, and an obstacle.

The situation is comparable to the 18th century, in which most people could
not read and write, and relied heavily on the services of professional
scribes, translators, priests, and each other. Many gave up any prospect of
understanding the world around them, of control over their lives, and of
advancement in society. Such people were vulnerable and generally oppressed.
They were often the victims of scams, and their lives were full of risk. Such a
situation is not healthy, and it is getting worse [worth noting some differences? e.g. many scams rely on decline in face-to-face interaction, which largely survived oral→written→postal transitions: imagine a world in which by the 1960s most banks had closed down and banking was conducted by post].

On current trends, most of us, if we do nothing, will eventually find ourselves
part of a digitally illiterate underclass. A 21st century person who cannot
use a computer will be like an 18th century person who cannot read, and a 21st
century person who cannot program will be like an 18th century person who
cannot write. This widespread illiteracy is not good for anybody. It's bad for
those who do become helpless; it's bad for those struggling not to be; and
it's bad for those who end up supporting everybody else.

The solution is not Luddism [debatable]. The incipient computer revolution,
like the ongoing industrial revolution, is happening because of strong forces,
and will not wait.

The solution is not the destruction of Big Tech [also debatable], though we
must at least partially escape from reliance on software written by other
people.

The solution is foundational technologies that people can reach into and
change [these are not a solution, these are a must have; if they’re incompatible with Luddism and/or Big Tech, then what gives?].

Programming (or whatever it will be called in the future) needs to be reframed
as a basic literacy skill. Programming must be easy: children will need to
learn it at school. People must insist on surrounding themselves with whatever
programs they need to run their lives, including some that they write or
customise themselves. This will require new technology. [Cite me! Cite me! End of Innocents in particular.]

I dare not predict what programming will look like in twenty years. I do
predict, however, that the way ordinary people use computers will converge
with the way computers are programmed. The trend in that direction is already
clear. But the digital literacy deficit is not going to close automatically.
Somebody needs to invent the missing foundational technologies. It won't be
Big Tech [why not? Apple already built the world’s biggest company on making computers easier to use.].


## Heterogeneous motivations

We can learn from those who are already shunning mainstream technologies in
favour of software that they can more easily control. There are many such
people, and they have very little motivation in common.

[Each item becomes a short subsection, relying on external links.]

- Computer science
- Digital archives
- Retro-computing
- Game engines
- Distributed computing
- Privacy
- Free software
- ...


## Homogeneous solutions

Studying the solutions people have come up with reveals many common elements:

- *Virtual machines*: Writing programs for an abstract machine is a cheap way of giving them a long life and broad compatibility.
- *Programming languages*: Anything sufficiently complex ends up being controlled by a programming language.
- *Package managers*: Anything with enough authors ends up needing a way of naming their creations and of tracking their versions and dependencies.
- *Social graphs*: Anything with enough users ends up grappling with concepts of ownership, groups, permission and delegation.
- *Secure networking*: Anything involving communication suffers the same kinds of attacks, and requires the same kind of defences.

[Need to flesh this out, relying on external links.]

### It doesn't have to be good

Heterodox technology always looks bad if it is evaluated as orthodox
technology, just as a hand-written notice looks bad next to a Hollywood
blockbuster. Rejecting heterodox technology for that reason is missing its
point. It doesn't need to be optimised for the mass market. It doesn't need to
be at the forefront of technology. It doesn't need to have tens of millions of
dollars spent on polish. It just needs to do its job, and to be easy to make.


## Proposal

We propose to write a bunch of adaptable foundational technologies. The idea is to provide simple, wise solutions to the problems that "everybody" needs to solve, in order to allow people to focus on whatever is unique to their situation.

What makes a technology foundational? We think these are important criteria:

- *Useful*: The technology should do something that many people need.
- *Feasible*: Providing the technology must be within our capabilities.
- *Simple*: A user should ideally be able to learn how to use the technology on the day that they discover that they need it. Note that the technology does not necessarily need to be internally simple.
- *Wise*: The technology must do something that the user might struggle to do well without it. It must be non-trivial. It should incorporate expert best practice. It should avoid common pitfalls.
- *Replicable*: The technology must be easily copied. The value of a technology that can serve one person is negligible beside that of a technology that can serve a million.
- *Modular*: While the technology provides a standard solution for people with standard needs, it must be easily replaceable by people who need something else. The technology must assume as little as possible about the context in which it is used. Integrated technologies are unhelpful.
- *High quality*: The technology must avoid flaws that would spoil projects built on top of it. Notably, the technology must be efficient, reliable and secure.

We have compiled a list of technologies that we think could meet these criteria:

- *Virtual machine*: abstracts CPU and memory, low-level portability
- *Programming language*: the glue which holds everything else together
- *Platform*
  - Standard libraries: common programming components that many people need
  - Accelerators: things without which software is uncompetitively inefficient
  - User interfaces
  - Databases: persistent, multiuser, larger than memory
  - Protocols: already existing, and novel
- *Packaging*
  - Distribution
  - Naming
  - Dependencies
  - Versions
- *Social graph*
  - Accounts: identifying information, contact details
  - Groups: accounts controlled by one or more other accounts
  - Ownership: permission, delegation
  - Friendship: levels of trust
  - News: aggregation and filtering of timely information
- *Secure networking*
  - Authentication: passwords, certificates
  - Encryption
  - Addresses: name resolution, routing
- *Key applications*
  - Messaging
  - Publishing
  - Collaborative editing: version control, issue tracking
  - Apps: untrusted programs, principle of least privilege

Some of these exist already. Some we are writing. Some are neglected.

### Organisations

- *Pubnix* organisations: always-on, public presence, can write and execute your own code.
