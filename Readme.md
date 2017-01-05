This is a specification for a robot programming language.

For now, we have a few supported functions at different levels:

1 : [Low level] Robot Assembly:
These are "atomic" commands that are executed by a robot. They must be completed or aborted before anything else can be executed.

2 : [Intermediate level] State Machine Commands:
These commands compile to a state machine of assembly commands. They may be interrupted/restarted. To support interrupts, they must have predefined entry and exit states (which could be one or many).

3 : [High level] Communicating Logic Processes:
These commands will allow specifying logic processes

