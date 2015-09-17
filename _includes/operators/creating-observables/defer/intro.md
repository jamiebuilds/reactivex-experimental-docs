The `Defer` operator waits until an observer subscribes to it, and then it
generates an Observable, typically with an Observable factory function. It does
this afresh for each subscriber, so although each subscriber may think it is
subscribing to the same Observable, in fact each subscriber gets its own
individual sequence.

In some circumstances, waiting until the last minute (that is, until
subscription time) to generate the Observable can ensure that this Observable
contains the freshest data.
