RxJava implements this operator as `create`.

It is good practice to check the observer’s `isUnsubscribed` state from within
the function you pass to `create` so that your Observable can stop emitting
items or doing expensive calculations when there is no longer an interested
observer.

