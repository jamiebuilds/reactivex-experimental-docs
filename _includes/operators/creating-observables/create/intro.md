You can create an Observable from scratch by using the Create operator. You pass
this operator a function that accepts the observer as its parameter. Write this
function so that it behaves as an Observable — by calling the observer’s
`onNext`, `onError`, and `onCompleted` methods appropriately.

A well-formed finite Observable must attempt to call either the observer’s
`onCompleted` method exactly once or its `onError` method exactly once, and must
not thereafter attempt to call any of the observer’s other methods.
