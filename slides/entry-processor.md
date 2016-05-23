##  Entry Processor

* Concurrent operations
* Distributed Lock
* Eliminates costly network hops
* Avoid long running executions
* Serialization savings

note:
1. more granular
2. Dist lock less granular
	1. lock at a client level
	2. get : Server to Client
	3. validation
	4. Set : Client to Server
3. could starve operations of a thread.
