RxJS implements a somewhat similar operator called `case` (or `switchCase`).
This operator conditionally creates and returns one of a set of possible
Observables. It takes the following parameters:

1. A function that returns the key that determines which Observable to emit
1. An object that associates those keys with particular Observables.
1. (optional) a [Scheduler]() or an Observable:
  - **Scheduler:** The Scheduler you want this operator to use.
  - **Observable:** The default Observable to emit if the key does not associate
    with any Observables.
