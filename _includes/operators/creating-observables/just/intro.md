The `Just` operator converts an item into an Observable that emits that item.

`Just` is similar to `From`, but note that `From` will dive into an array or an
iterable or something of that sort to pull out items to emit, while Just will
simply emit the array or iterable or what-have-you as it is, unchanged, as a
single item.

Note that if you pass `null` to Just, it will return an Observable that _emits_
`null` as an item. Do not make the mistake of assuming that this will return an
empty Observable (one that emits no items at all). For that, you will need the
[`Empty`]() operator.
