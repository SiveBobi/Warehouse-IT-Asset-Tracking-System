# Asset REST API

```java
@RestController
@RequestMapping("/api/assets")

public class AssetController {

 private final AssetService service;

 public AssetController(
 AssetService service){
   this.service = service;
 }

 @GetMapping
 public List<Asset> getAll(){
   return service.getAllAssets();
 }

 @PostMapping
 public Asset create(
 @RequestBody Asset asset){

   return service.registerAsset(
   asset);
 }

 @PutMapping("/{id}")
 public Asset updateStatus(
 @PathVariable String id,
 @RequestParam String status){

   return service.updateStatus(
   id,status);
 }

}
```
