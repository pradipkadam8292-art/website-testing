# Defect Report

Defects found while testing the Field Force Connect web application. Each defect ID is linked to the test cases that failed because of it (see the Defect_ID column in the Excel report).

| Defect ID | Module | Summary | Failed Test Cases | Status |
|---|---|---|---|---|
| DEF_01 | Sign Up | Company Name accepts special characters and numbers-only values | SU_04, SU_05 | Open |
| DEF_02 | Sign Up | Contact Person Name accepts numbers and special characters | SU_11, SU_12 | Open |
| DEF_03 | Sign Up | No maximum length limit on the name fields | SU_06, SU_14 | Open |
| DEF_04 | Sign Up | Duplicate Company Name is accepted | SU_08 | Open |
| DEF_05 | Sign Up | Duplicate Mobile Number is accepted | SU_22, SU_42 | Open |
| DEF_06 | Sign Up | Duplicate Email ID is accepted | SU_33, SU_42 | Open |
| DEF_07 | Sign Up | Country is not selected after choosing a country code | SU_23 | Open |
| DEF_08 | Forgot Password | Forgot Password shows an OTP sent message, but no OTP is received | FP_02 | Open |
| DEF_09 | Sign In with OTP | Sign In with OTP form can be submitted without a password | OTP_19 | Open |
| DEF_10 | Sign In with OTP | OTP is not received on email, it is only sent by SMS | OTP_20 | Open |
| DEF_11 | Sign Up, Sign In with OTP | No Back button on the Sign Up, Login and OTP pages | SU_43, OTP_18 | Open |
| DEF_12 | Sign In with OTP | No attempt limit message after repeated wrong OTPs | OTP_16 | Open |
| DEF_13 | Sign Up, Sign In with OTP, Login | Email ID starting with a capital letter is not accepted | SU_31, OTP_23, LG_08 | Open |
| DEF_14 | Forgot Password | Back button on Forgot Password opens the Sign Up page instead of Login | FP_17 | Open |
| DEF_15 | Forgot Password | No error message is shown for a used or expired reset link | FP_16 | Open |
| DEF_16 | Sign Up, Forgot Password, Login | Spaces before or after the email are not trimmed | SU_32, FP_07, LG_09 | Open |
| DEF_17 | Login | Same user can log in multiple times with the same details | LG_14 | Open |
| DEF_18 | Sign In with OTP | Resend OTP can be requested again and again, with no timer | OTP_15 | Open |
| DEF_19 | Forgot Password | No password length error on the reset password page | FP_12 | Open |
| DEF_20 | Forgot Password | Multiple reset requests can be sent for the same email | FP_08 | Open |

Total defects: 20
