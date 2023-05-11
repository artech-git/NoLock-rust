# NoLock-Rust

![image](https://img.shields.io/badge/Rust-black?style=for-the-badge&logo=rust&logoColor=#E57324)

A Collection of non-locking data structures and crates supporting them 


## Why non-locking data structures
Lock-free data structures are designed to allow multiple threads or processes to access and modify shared data without the use of traditional synchronization mechanisms like mutual exclusion, semaphores etc . 

## Benefits of lock free data structures
Some potential benefits of using lock-free data structures include:

1.  **Increased scalability**: Traditional locking mechanisms can become a bottleneck when many threads are contending for the same lock, leading to contention and decreased performance. Lock-free data structures can potentially offer better scalability as there is no contention among threads.
    
2.  **Improved performance**: Lock-free data structures can avoid the overhead of acquiring and releasing locks, leading to better performance in scenarios where high concurrency is required.
    
3.  **Lower risk of deadlock**: Deadlocks can occur when multiple threads are waiting for each other to release a lock, leading to a deadlock. Lock-free data structures can help avoid this risk as there are no locks to be held or released.
    
4.  **Better fault-tolerance**: Lock-free data structures can be more fault-tolerant as there is no need to worry about locks being left held indefinitely due to a thread crashing or being terminated unexpectedly.
    
5.  **Easier to reason about**: Lock-free data structures can be simpler to reason about as there are no locks or potential deadlock scenarios to consider.
**offline!**


## when to avoid lock free data structures
1.  **Limited concurrency**: If your application has low concurrency requirements, then the overhead of designing and implementing lock-free data structures may not be worth the potential benefits.
    
2.  **High contention**: Lock-free data structures work best when there is little contention among threads. If many threads are frequently contending for the same shared data, the performance of lock-free data structures may actually be worse than traditional locking mechanisms.
    
3.  **Complex data structures**: Designing lock-free data structures can be challenging, especially for complex data structures. If the data structure is relatively simple, traditional locking mechanisms may be sufficient.
    
4.  **Portability**: Lock-free data structures may not be portable across different architectures or platforms, especially if low-level synchronization primitives are used.
    
5.  **Risk of data corruption**: Lock-free data structures require careful synchronization to avoid data corruption or lost updates. If the implementation is not done carefully, there may be subtle bugs that are difficult to detect and reproduce.


## List of crates designed/supporting this operation

 - [crossbeam](https://crates.io/crates/crossbeam)
 - [lockfree](https://crates.io/crates/lockfree)
 - [bus](https://crates.io/crates/bus)
 - [ringbuf](https://crates.io/crates/ringbuf)
 - [dashmap](https://crates.io/crates/dashmap)
 - [sharded-slab](https://crates.io/crates/sharded-slab)
 - [evmap](https://crates.io/crates/evmap)
 - [crossbeam skiplist](https://crates.io/crates/crossbeam-skiplist)

# Feel free to contribute to this repo 
