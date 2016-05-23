##  In Memory Format

* BINARY vs OBJECT     <!-- .element: class="fragment" data-fragment-index="1" -->
* Complex objects		<!-- .element: class="fragment" data-fragment-index="2" -->
* Efficient if majority of operations are entry processor driven		<!-- .element: class="fragment" data-fragment-index="3" -->


note:
1. 140 kb entry
2. Majority of operations - UPDATES > READS
3. Every update operation -> deserialize, mutate and serialize
	1. 2 network hops
4. OBJECT with entry processor
	1. executed the operation upon a member where data resides
	2. eliminates 2 network hops
