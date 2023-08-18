# qa.perf.locks: Performance impact of multithreaded locking

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Use as few write-locks as possible, and prefer `RwLock` over `Mutex`.

**Note:** `RwLock` allows multiple read-locks on the same shared data.
