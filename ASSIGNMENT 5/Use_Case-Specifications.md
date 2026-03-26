# Use Case Specifications

## UC1: Register Asset
Actor: IT Administrator  
Precondition: Admin is logged in  
Postcondition: Asset is stored in the system  

Basic Flow:
1. Admin enters asset details
2. System validates data
3. System saves asset

Alternative Flow:
- Invalid data → system shows error

---

## UC2: Update Asset Location
Actor: IT Administrator  
Precondition: Asset exists  
Postcondition: Location updated  

Basic Flow:
1. Admin selects asset
2. Updates location
3. System saves changes  

Alternative Flow:
- Asset not found → error message  

---

## UC3: Update Asset Status
Actor: IT Administrator  
Precondition: Asset exists  
Postcondition: Status updated  

Basic Flow:
1. Admin selects asset
2. Updates status
3. System records update  

---

## UC4: Search Asset
Actor: All users  
Precondition: None  
Postcondition: Results displayed  

Basic Flow:
1. User enters search criteria
2. System retrieves results  

Alternative Flow:
- No results found  

---

## UC5: Record Maintenance
Actor: Maintenance Technician  
Precondition: Asset is faulty  
Postcondition: Maintenance record saved  

Basic Flow:
1. Technician logs repair
2. System updates history  

---

## UC6: View Reports
Actor: Manager  
Precondition: Data exists  
Postcondition: Report displayed  

Basic Flow:
1. Manager selects report type
2. System generates report  

---

## UC7: Report Fault
Actor: Warehouse Worker  
Precondition: Asset exists  
Postcondition: Fault recorded  

Basic Flow:
1. Worker selects asset
2. Submits fault report  

---

## UC8: Login
Actor: All users  
Precondition: User registered  
Postcondition: Access granted  

Basic Flow:
1. User enters credentials
2. System validates login  

Alternative Flow:
- Invalid login → access denied  
