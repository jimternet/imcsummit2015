##  In Memory Format

* BINARY vs OBJECT
* Complex objects
* Efficient if majority of operations are entry processor driven


note:
1. 140 kb entry
2. UPDATES > READS
3. Every update operation -> deserialize, mutate and serialize
	1. 2 network hops
4. OBJECT with entry processor
	2. eliminates 2 network hops
