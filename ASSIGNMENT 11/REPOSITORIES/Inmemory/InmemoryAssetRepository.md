# In-Memory Repository Implementation

```java
import java.util.*;

public class InMemoryAssetRepository
implements AssetRepository {

 private Map<String, Asset> storage =
 new HashMap<>();

 @Override
 public void save(Asset asset){
   storage.put(asset.getAssetId(),asset);
 }

 @Override
 public Optional<Asset> findById(String id){
   return Optional.ofNullable(
      storage.get(id)
   );
 }

 @Override
 public List<Asset> findAll(){
   return new ArrayList<>(
      storage.values()
   );
 }

 @Override
 public void delete(String id){
    storage.remove(id);
 }

 public List<Asset> findByStatus(
 String status){
   return storage.values()
      .stream()
      .filter(a->a.getStatus()
      .equals(status))
      .toList();
 }
}
```
