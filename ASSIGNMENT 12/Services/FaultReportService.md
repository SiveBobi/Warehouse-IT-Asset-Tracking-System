# Fault Report Service

```java
public class FaultReportService {

 private final FaultReportRepository
 repo;

 public FaultReportService(
 FaultReportRepository repo){
   this.repo = repo;
 }

 public FaultReport createReport(
 FaultReport report){

   repo.save(report);

   return report;
 }

 public List<FaultReport>
 getAllReports(){

   return repo.findAll();
 }

}
```
