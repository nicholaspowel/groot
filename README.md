# The Groot Programming Language

Groot is an [esoteric programming language](http://en.wikipedia.org/wiki/Esoteric_programming_language), which
uses the language of an extraterrestrial plant from Planet X called [Groot](http://en.wikipedia.org/wiki/Groot) as its syntax.

### Commands

There are eight commands like [Brainfuck](http://en.wikipedia.org/wiki/Brainfuck):

phrase|meaning|
--------|---------|
`i am groot`|increment the byte at the data pointer.|
`I am Groot`|decrement the byte at the data pointer.|
`I AM GROOOT`|output the byte at the data pointer.|
`I AM GROOT`|increment the data pointer.|
`I am groot`|decrement the data pointer.|
`I am grooot`|accept one byte of input.|
`I'm Groot`|if the byte at the data pointer is zero, then instead of moving the instruction pointer forward to the next command, jump it forward to the command after the matching `We are Groot` command.|
`We are Groot`|if the byte at the data pointer is nonzero, then instead of moving the instruction pointer forward to the next command, jump it back to the command after the matching `I'm Groot` command.|

### Building

To build, run:
```bash
$ cargo build
```

### Running

To run:
```bash
$ cargo run helloworld.groot
```

The Rust version used to build this:
`rustc 1.0.0-nightly (dfc5c0f1e 2015-02-18) (built 2015-02-19)`

It will probably work with any nightly build.
