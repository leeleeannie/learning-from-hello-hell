#### atomic vs. nonatomic

* default / not default behaviour
* slower / faster
* [thread-safe](#WhatIsThreadSafe) / not thread-safe - Shared data which accessed by using atomic operations cannot be interrupted by other threads. That is, multiple read/write to a single property are serialized. For nonatomic, if multiple threads try to read/write the property at once, which can easily lead to crashes.
 

#### strong vs. weak

A strong reference means that you want to "own" the object you are referencing with this property. The compiler will take care that any object that you assign to this property will not be destroyed as long as you (or any other object) points to it with a strong reference. Only once you set the property to nil will the object get destroyed.

A weak reference means that you don't want to have control over the object's lifetime. The object you are referencing weakly only lives on because at least one other object holds a strong reference to it. Once that is no longer the case, the object gets destroyed and your weak property will automatically get set to nil. A weak reference can prevent from retain cycle, which is a form of memory leak.

Read [balloon metaphor](http://stackoverflow.com/questions/11013587/differences-between-strong-and-weak-in-objective-c) by MJN and [object ownership](http://rypress.com/tutorials/objective-c/properties) for more details.

#### What is accessor methods?

Simply getters and setters.


#### Segue: push, modal?

#### What is delegate?

#### What is memory leak?

#### @interface vs. @implementation

#### What is frame, bound and view?

#### Deal with multithreading?

<a name="WhatIsThreadSafe"></a>
#### What is thread-safe?

A piece of code is thread-safe if it functions correctly during simultaneous execution by multiple threads. In particular, it must satisfy the need for multiple threads to access the same shared data, and the need for a shared piece of data to be accessed by only one thread at any given time. [[more](http://stackoverflow.com/questions/261683/what-is-meant-by-thread-safe-code)]
