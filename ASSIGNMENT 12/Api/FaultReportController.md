# Fault Report REST API

```java
@RestController
@RequestMapping("/api/reports")

public class FaultReportController {

 private final FaultReportService
 service;

 public FaultReportController(
 FaultReportService service){
   this.service = service;
 }

 @GetMapping
 public List<FaultReport> getAll(){

   return service.getAllReports();
 }

 @PostMapping
 public FaultReport create(
 @RequestBody FaultReport report){

   return service.createReport(
   report);
 }

}
```
