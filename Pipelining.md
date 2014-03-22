## Pipelining
===========

Design a state machine so that the outputs during one clock period depend on the state and inputs during the _previous_ clock period.

![Pipelined output](pipelined_output.png)

- one additional logic (flip-flops) is attached to the output
- usable only if you know the desired next output value one clock period _in_ _advance_
    - because your next input could depend on it!

### From computer architecture

> like an assembly line.

Pipelining is an implementation technique in which multiple instructions are overlapped in execution. It increases instruction _throughput_ instead of instruction _execution_ _time_ or _latency_.

![Pipelined laundry](pipelined_laundry.png)

#### Pipeline hazards

1. structural hazard: cannot support the combination of instructions in the same clock period.
2. data hazard: when current instruction has to be _stalled_ to wait for another to complete
3. control hazard: when proper instructions cannot be executed in proper clock period because output of some instructions are not expected.
