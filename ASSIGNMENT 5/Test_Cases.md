# Test Cases
Warehouse IT Asset Tracking System

## Functional Test Cases

| Test ID | Requirement | Description | Steps | Expected Result | Status |
|--------|------------|-------------|-------|----------------|--------|
| TC-001 | FR1 | Register asset | Enter details → Save | Asset saved | Pending |
| TC-002 | FR2 | Update location | Select asset → Update | Location updated | Pending |
| TC-003 | FR3 | Update status | Change status | Status saved | Pending |
| TC-004 | FR4 | Search asset | Enter keyword → Search | Results shown | Pending |
| TC-005 | FR5 | Maintenance record | Log repair | Record saved | Pending |
| TC-006 | FR7 | Generate report | Click report | Report generated | Pending |
| TC-007 | FR8 | Report fault | Submit fault | Fault recorded | Pending |
| TC-008 | FR10 | Login | Enter credentials | Access granted | Pending |

---

## Non-Functional Test Cases

### Performance Test
- Simulate 1000 users searching assets
- Expected: Results within 2 seconds

### Security Test
- Attempt login with incorrect password
- Expected: Access denied
