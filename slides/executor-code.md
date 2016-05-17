##  Executor Synchronization
```
	public class SynchronizationExecutorService {
    	private static final int NUMBER_OF_THREADS = 40;
    	private ExecutorService[] threadPool
          = new ExecutorService[NUMBER_OF_THREADS];

    	public SynchronizationExecutorService() {
        	for(int i = 0; i < NUMBER_OF_THREADS; i++) {
            	threadPool[i] = Executors.newSingleThreadExecutor();
        	}
    	}
    	public void executeOnProduct(Integer id, Runnable runnable) {
        	int index = Math.abs(id.hashCode()%NUMBER_OF_THREADS);
        	threadPool[index].execute(runnable);
    	}
	}

```

note:
    Put your speaker notes here.
    You can see them pressing 's'.
