##  Javolution

Struct types, bitfields (ala C/C++)

```
    private static class ProductStruct extends Struct {

        final Signed32 productID = new Signed32();

        final Signed16 networkDemand = new Signed16();

        final Unsigned8 productIDType = new Unsigned8(1);

        final Unsigned8 multichannelOptions = new Unsigned8(7);

        final Unsigned8 itemStatus = new Unsigned8(3);

        final Unsigned8 limitedQuantityEnabled = new Unsigned8(1);

        final Unsigned8 preOrBackOrderEnabled = new Unsigned8(1);
     }
```
