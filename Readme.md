This is a specification for a robot programming language.

********
Commands
********

For now, we have a few supported functions at different levels:

1 : [Low level] Robot Assembly:
These are "atomic" commands that are executed by a robot. They must be completed or aborted before anything else can be executed.

2 : [Intermediate level] State Machine Commands:
These commands compile to a state machine of assembly commands. They may be interrupted/restarted. To support interrupts, they must have predefined entry and exit states (which could be one or many).

3 : [High level] Communicating Logic Processes:
These commands will allow specifying logic processes.

******
Schema
******

Each set of commands has an associated schema, and a set of exemplars.
These are contained in json files. 
When in doubt, refer to the schema for a general idea of what is possible.

NOTE : A command that satisfies the schema doesn't necessarily compile to a robot executable program

*************
Robot Program
*************

The purpose of the programming language is to structure commands that
can then be translated into a control library's functions..
