##  Javolution

Overlay on NIO ByteBuffer

```
    private ByteBuffer backingData;

    private static final ThreadLocal<ProductStruct> PRODUCT_STRUCT =
            ThreadLocal.withInitial(ProductStruct::new);

    private ProductStruct getProductStruct() {
        final ProductStruct productStruct = PRODUCT_STRUCT.get();
        productStruct.setByteBuffer(backingData, 0);
        return productStruct;
    }
    
    public int getProductId() {
        return getProductStruct().productID.get();
    }
    public void setProductId(int productId) {
        getProductStruct().productID.set(productId);
    }
```
