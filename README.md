# RxIsDead

No Rx isn't really dead, but maybe you want to kill it in your project because you're using Coroutines. 

Add this library and you will get lint-check warnings for RxJava use-cases that can easily be replaced with a Kotlin Coroutine Equivalent.


## Installation
--------

```groovy
implementation 'com.jacquessmuts:rxisdead:{version}'
```

## Basic Use-cases:

| RxJava  | Coroutine |
| ------------- | ------------- |
| Single>T> | suspend fun: T |
| Maybe<T> | suspend fun: T? |
| Completable | suspend fun: Unit |
| Subject<T> | Channel<T> |
| Observable<T> | Flow<T> |
| Flowable<T> | Flow<T> |

