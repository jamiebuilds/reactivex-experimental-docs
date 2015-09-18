RxJava implements this operator as `defer`. This operator takes as its sole
parameter an Observable factory function of your choosing. This function takes
no parameters and returns an Observable.

`defer` does not by default operate on a particular [Scheduler]().

- Javadoc: [`defer()`]()
