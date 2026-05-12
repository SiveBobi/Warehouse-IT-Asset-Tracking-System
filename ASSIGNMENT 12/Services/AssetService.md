# Asset Service

```java
public class AssetService {

 private final AssetRepository assetRepo;

 public AssetService(
 AssetRepository assetRepo){
   this.assetRepo = assetRepo;
 }

 public Asset registerAsset(
 Asset asset){

   if(asset.getAssetId()==null){
      throw new IllegalArgumentException(
      "Asset ID required");
   }

   assetRepo.save(asset);

   return asset;
 }

 public Asset updateStatus(
 String id,
 String status){

   Asset asset =
   assetRepo.findById(id)
   .orElseThrow();

   asset.setStatus(status);

   assetRepo.save(asset);

   return asset;
 }

 public List<Asset> getAllAssets(){
    return assetRepo.findAll();
 }

}
```
