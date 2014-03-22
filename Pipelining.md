## Pipelining
===========

Design a state machine so that the outputs during one clock period depend on the state and inputs during the _previous_ clock period.

![Pipelined output](pipelined_output.png)

- one additional logic (flip-flops) is attached to the output
- usable only if you know the desired next output value one clock period _in_ _advance_

#### From computer architecture

Pipelining is an implementation technique in which multiple instructions are overlapped in execution. "like a assembly line."
