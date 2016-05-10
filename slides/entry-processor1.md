##  Entry Processor Code

```
	public class EmployeeSalaryEntryProcessor
      implements EntryProcessor<Integer, Double>,
                  EntryBackupProcessor<Integer, Double> {
    	public Object process(Entry<Integer, Double> entry) {
      		Double value = (Double) entry.getValue();
      		entry.setValue( value + 1.0 );
      		return (value + 1.0);
    	}
    	public EntryBackupProcessor getBackupProcessor() {
      		return EmployeeSalaryEntryProcessor.this;
    	}
    	public void processBackup(Entry<Integer, Double> entry) {
      		if(entry.getValue() != null) {
        		process(entry);
      		}
    	}
	}

```
