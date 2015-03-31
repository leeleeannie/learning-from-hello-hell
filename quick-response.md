#### atomic vs. nonatomic

* default / not default behaviour
* slower / faster
* [thread-safe](#WhatIsThreadSafe) / not thread-safe - Shared data which accessed by using atomic operations cannot be interrupted by other threads. That is, multiple read/write to a single property are serialized. For nonatomic, if multiple threads try to read/write the property at once, which can easily lead to crashes.
 

#### strong vs. weak

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
