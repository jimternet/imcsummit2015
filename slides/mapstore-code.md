##  Mapstore Configuration

```
	MapConfig mapConfig = new MapConfig();
	mapConfig.setName("employeeEvents");

	MapStoreConfig mapStoreConfig = new MapStoreConfig();
	mapStoreConfig.setImplementation(new EmployeeStore());
	// * Set 0 to write immediately, write-through map store.
	// * > 0 to implement a write-behind map store.
	mapStoreConfig.setWriteDelaySeconds(1);
	mapStoreConfig.setWriteBatchSize(100);
	mapStoreConfig.setWriteCoalescing(false);
	mapStoreConfig.setEnabled(Boolean.TRUE);

	mapConfig.setMapStoreConfig(mapStoreConfig);

```
note:
    Put your speaker notes here.
    You can see them pressing 's'.
