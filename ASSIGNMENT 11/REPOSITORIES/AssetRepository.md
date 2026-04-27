# Asset Repository

```java
public interface AssetRepository
extends Repository<Asset,String> {

   List<Asset> findByStatus(String status);

   List<Asset> findByLocation(String location);
}
```

## Entity-Specific Operations

Additional methods support:
- Search by status
- Search by location
- Asset-specific retrieval logic
