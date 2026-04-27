# Unit Tests

## CRUD Test Cases

| Test ID | Test | Expected Result |
|--------|------|----------------|
| TC01 | Save Asset | Asset stored |
| TC02 | Find Asset | Asset retrieved |
| TC03 | Find All | All assets returned |
| TC04 | Update Asset | Changes saved |
| TC05 | Delete Asset | Asset removed |

## Sample Test

```java
@Test
public void saveAsset(){

 Asset asset=
 new Asset("A100");

 repo.save(asset);

 assertTrue(
 repo.findById("A100")
 .isPresent()
 );
}
```
