# Website Testing Assignment - Field Force Connect

Manual testing of the authentication pages of the Field Force Connect web application. Test cases were written and executed for four modules, and the results and defects are recorded in the Excel report.

**Website tested:** https://test.fieldforceconnect.com/auth/register

## Modules covered

1. Sign Up
2. Forgot Password
3. Sign In with OTP
4. Login

## Files in this repository

| File | What it contains |
|---|---|
| `Test_Cases_and_Execution_Report.xlsx` | Test cases for each module (one sheet per module), actual results, status, defect IDs and a Summary sheet with charts |
| `Defect_Report.md` | List of all defects found, with the failed test cases for each one |
| `images/test-summary.png` | Screenshot of the Summary sheet |

## Test case format

Every module sheet uses the same columns: TC ID, Module, Test Scenario, Test Data, Expected Result, Actual Result, Status and Defect_ID.

## Results

| Module | Total Test Cases | Passed | Failed | Pass % | Fail % |
|---|---|---|---|---|---|
| Sign Up | 47 | 27 | 15 | 64.3% | 35.7% |
| Forgot Password | 17 | 7 | 6 | 53.8% | 46.2% |
| Sign In with OTP | 23 | 16 | 6 | 72.7% | 27.3% |
| Login | 20 | 12 | 3 | 80.0% | 20.0% |
| **Total** | **107** | **62** | **30** | **67.4%** | **32.6%** |

Pass % and Fail % are calculated on the test cases executed so far. 20 defects were logged in total.

![Test summary](images/test-summary.png)

## Main findings

- **Sign Up:** the name fields have almost no validation. Special characters, numbers and very long values are accepted, and the same company name, mobile number and email can be registered more than once.
- **Forgot Password:** a success message says an OTP was sent, but no OTP is received. Because of this the reset flow cannot be used properly. The Back button also opens the Sign Up page.
- **Sign In with OTP:** OTP login works for valid details, but there is no attempt limit, no resend timer, and the OTP is not received on email.
- **Email handling:** an email starting with a capital letter is rejected, and spaces before or after the email are not trimmed on the Sign Up, Forgot Password and Login pages.
- **Navigation:** there is no Back button on the Sign Up, Login and OTP pages.

All defects are listed in [Defect_Report.md](Defect_Report.md).
