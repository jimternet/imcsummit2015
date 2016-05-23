##  Map Store

* Store events to a persistent data store   <!-- .element: class="fragment" data-fragment-index="1" -->
* Write Behind and Write Coalescing  	<!-- .element: class="fragment" data-fragment-index="2" -->
* Write behind queue capacity		<!-- .element: class="fragment" data-fragment-index="3" -->


note:
1. write delay seconds = 0 (write through)
2. entries will be executed after configured delay aync
3. write coalescing - be default coaleses updates on a specific key
