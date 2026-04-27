# Repository Factory

```java
public class RepositoryFactory {

 public static AssetRepository
 getAssetRepository(
 String storageType){

   switch(storageType){

      case "MEMORY":
      return new
      InMemoryAssetRepository();

      case "DATABASE":
      return new
      DatabaseAssetRepository();

      default:
      throw new IllegalArgumentException(
      "Invalid storage type");
   }

 }

}
```

## Why Factory Pattern?

Factory Pattern was chosen because:

- Easy swapping of storage
- Decouples services from storage logic
- Supports future extensions:
  - SQL
  - MongoDB
  - REST API
