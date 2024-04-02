# Currently underway: the state of play

Starting from: gemini://gemini.ucant.org/notes/beetle-mit.gmi

# What are Beetle, Mit, Welly, etc?

There are these projects:

## Virtual machines

Reuben Thomas is trying to write a general-purpose virtual machine. Some of his attempts are as follows:

### [Beetle]((https://github.com/rrthomas/beetle))

Beetle, written in C, is an early version of this (for his degree). Beetle has two stacks, being designed to run Forth. Reuben ported pForth to run on Beetle. pForth is ANSI Forth compatible. Both Beetle and pForth are frozen in amber.

Direct descendants of Beetle are:

* Bee
* Mit
* (other obsolete things)

### [Bee](https://github.com/rrthomas/bee)

Bee, written in C, but simpler than Beetle and general purpose. It also runs a Forth-ish compiler (called Gnat; no connected with GNU Ada compiler). Bee has two stacks but it is intended to reduce this to one. Bee's instruction set is massively reduced compared to Beetle, and the semantics are much more C-like than the Forth-like model of Beetle.

### [Mit](https://github.com/rrthomas/mit)

Mit, written in C. It also descends from Beetle in a code sense. It is effectively an earlier incarnation of Bee. It is a single stack VM that also ran a Forth compiler. It had an ancestor of Mijit written for it. Mit had 30 instructions. As of right now (Mar 2023), Mit is the most sophisticated and complete general purpose of VM of Reuben's stable, but he dislikes how it is implemented.

While Mit has the more complete VM functionality, Bee interoperates better with the conventional binutils ecosystem.

### [Mite](https://github.com/rrthomas/mite)

The other root of Reuben's system is Mite. Mite is a completely different implementation approach from Beetle, designed specifically for AOT compilation, with load-time conversion from virtual code to machine code. This makes it a notional direct competitor of the JVM, of which it is a contemporary.  Mite had a C-compiler backend that targeted it. It only runs on RiscOS.


## Languages

### [Welly](https://wellylang.org)

Welly is a language by Alistair Turnbull and Tom Lynn. It is a compromise
between Python, C, Java and OCaml.

Welly should provide a different lingua franca for languages to interoperate. Welly has a REPL.

Welly ought to include a virtual machine.

### [Ursa](https://ursalang.github.io)

Ursa is a language that is designed to look familiar to users of mainstream languages circa 2020. It is an imperative functional language that will offer static type checking and a class system that will have a circa 2000 feel. It will come with a standard library that offers file system and network access, keyboard and mouse interaction, and basic sound and graphics support.

### [pForth](https://github.com/rrthomas/pforth)

pForth was implemented in the 1990s alongside Beetle. Originally targeted 26-bit ARM, ported to Beetle and Mit and the various other systems.

Relatedly, [Gnat](https://github.com/rrthomas/gnat) was the start of pForth with the brakes of backward compatibility removed.


## [Tooling](https://github.com/apt1002/mijit)

Mijit - a JIT-compiler generator, written in Rust, but callable from other languages, and it works with C. It developed out of ideas in Mit. So far it has been used to write JIT compilers for Beetle and Bee. The intention is to use it as the JIT compiler for Welly. Mijit has backends for x86-64 and aarch64.

## Future plans

Work on Bee. Conform it to Mit.

The plan for Welly is to have a calling convention which acknowledges garbage collection. The JIT compiler and GC will be below that calling convention, the advantage being that when languages call across to each other you can inline from one to the other.

Complete Ursa, with back-ends for JavaScript, WASM, LLVM, JVM, Python.

The Mit programme is implementing the core of Mite approach on the basis of the more traditional approach of Beetle.

## Miscellaneous

Alistair is also working on image compression:

Fractal Vector Quantizer (https://github.com)
