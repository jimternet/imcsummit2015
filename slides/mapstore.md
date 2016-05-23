##  Map Store

* Store events to a persistent data store
* Write Behind and Write Coalescing
* Write behind queue capacity


note:
1. write delay seconds = 0 (write through)
2. entries will be executed after configured delay aync
3. write coalescing - be default coaleses updates on a specific key
