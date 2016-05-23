##  Serialization
* DataSerializable and IdentifiedDataSerializable       <!-- .element: class="fragment" data-fragment-index="1" -->
* More resource efficient than Serializable     <!-- .element: class="fragment" data-fragment-index="2" -->
* Increased TPS     <!-- .element: class="fragment" data-fragment-index="3" -->
* Specific to Hazelcast     <!-- .element: class="fragment" data-fragment-index="4" -->


note:
1. Easy to Impement
2. more data serialized
3. increases the cpu load
Don't have exact control on how object or fields is serialized and deserialized. It also has suboptimal performance due to streaming class descriptors, versions, keeping track of seen objects to deal with cycles, etc. This causes additional CPU load and suboptimal size of serialized data.
4. less data serializaed
5. less CPU is consumed.
6. not free... you write a little more code :). 
IdentifiedDataSerializable. It relies on a factory to create the instance and therefore is faster when deserializing, since deserialization relies on creating new instances.
