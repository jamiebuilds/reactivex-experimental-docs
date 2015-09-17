When you work with Observables, it can be more convenient if all of the data you
mean to work with can be represented as Observables, rather than as a mixture of
Observables and other types. This allows you to use a single set of operators to
govern the entire lifespan of the data stream.

Iterables, for example, can be thought of as a sort of synchronous Observable;
Futures, as a sort of Observable that always emits only a single item. By
explicitly converting such objects to Observables, you allow them to interact as
peers with other Observables.

For this reason, most ReactiveX implementations have methods that allow you to
convert certain language-specific objects and data structures into Observables.
