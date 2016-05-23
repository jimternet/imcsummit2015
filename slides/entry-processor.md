##  Entry Processor

* Concurrent operations 	<!-- .element: class="fragment" data-fragment-index="1" -->
* Distributed Lock 	<!-- .element: class="fragment" data-fragment-index="2" -->
* Eliminates costly network hops	<!-- .element: class="fragment" data-fragment-index="3" -->
* Avoid long running executions		<!-- .element: class="fragment" data-fragment-index="4" -->
* Serialization savings		<!-- .element: class="fragment" data-fragment-index="5" -->


note:
1. Executes the code upon a member where data resides - more granular
2. Distributed lock - less granular
	1. lock at a client level
	2. get the data : Server to Client
	3. validaion
	4. Set the data : Client to Server
3. you could starve operations of a thread.
