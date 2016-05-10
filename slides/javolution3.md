##  Javolution

Serialize/unserialize NIO ByteBuffer

```
    @Override
    public void writeData(ObjectDataOutput out) throws IOException {
        out.writeByteArray(backingData.array());
    }

    @Override
    public void readData(ObjectDataInput in) throws IOException {
        backingData = ByteBuffer.wrap(in.readByteArray();
    }
```
