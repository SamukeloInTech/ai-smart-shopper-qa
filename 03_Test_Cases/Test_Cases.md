
# Executed Test Cases

| Test ID | Scenario | Expected Result | Status |
| :--- | :--- | :--- | :--- |
| TC_001 | Verify NSFAS warning for budget > R1,750 | System saves budget but displays a warning. | PASS |
| TC_002 | Verify mutually exclusive budgets | System blocks creating individual budgets if a combined one exists. | PASS |
| TC_003 | Verify "Proceed to Summary" is disabled when over budget | Button is disabled until list is under budget. | PASS |
| TC_005 | Verify successful login with valid credentials | User is redirected to Dashboard. | PASS |
| TC_006 | Verify login fails with invalid password | System displays error and denies access. | PASS |
| TC_007 | Verify rate limiting after multiple failed logins | System triggers rate limiter after rapid failed attempts. | PASS |
| TC_004 | Verify API rejects negative quantity | API should return 400 Bad Request. | FAIL (See BUG-001) |


## Detailed Test Case Example

<details>
<summary><b>Click to view detailed steps for TC_001 (NSFAS Warning)</b></summary>

<br>

**Precondition:** User is logged in and has no active budget.
**Test Data:** Combined Budget Amount = R1,800

**Steps:**
1. Navigate to the Budget page.
2. Select "Combined Budget".
3. Enter 1800 in the amount field.
4. Click Save.

**Expected Result:** The budget saves successfully, but a warning message appears stating the budget exceeds the NSFAS allowance of R1,750.

**Actual Result:** The system saved the budget and displayed a warning: *"Your budget is R1 800, which is R50 above the R1 750 NSFAS meal allowance reference. You can still save it."*

**Status:** PASS

</details>
