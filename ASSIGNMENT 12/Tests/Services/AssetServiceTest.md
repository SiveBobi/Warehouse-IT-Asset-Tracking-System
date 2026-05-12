# Asset Service Tests

```java
@Test
public void registerAsset(){

 Asset asset =
 new Asset("A100");

 service.registerAsset(asset);

 assertTrue(
 repo.findById("A100")
 .isPresent()
 );
}
```
