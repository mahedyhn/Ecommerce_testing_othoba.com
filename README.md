# 🧪 othoba.com — Complete QA Test Report

<div align="center">

![QA Badge](https://img.shields.io/badge/QA%20Status-In%20Progress-orange?style=for-the-badge&logo=testcafe)
![Tests](https://img.shields.io/badge/Total%20Tests-29-blue?style=for-the-badge&logo=checkmarx)
![Passed](https://img.shields.io/badge/Passed-24-brightgreen?style=for-the-badge&logo=checkmarx)
![Failed](https://img.shields.io/badge/Failed-5-red?style=for-the-badge&logo=checkmarx)
![Bugs](https://img.shields.io/badge/Bugs%20Found-5-critical?style=for-the-badge&logo=bugsnag)

**Prepared by:** MD Mahedy Hasan &nbsp;|&nbsp; **Website:** [Naiem.Website](https://Naiem.Website)  
**Target Site:** [https://othoba.com/](https://othoba.com/) &nbsp;|&nbsp; **Date:** May 2026

---

> *"Quality is not an act, it is a habit."* — Aristotle

</div>

---

## 📌 Table of Contents

- [🎯 Project Overview](#-project-overview)
- [📊 Test Metrics at a Glance](#-test-metrics-at-a-glance)
- [🗺️ Mind Map — Testing Coverage](#️-mind-map--testing-coverage)
- [📋 Test Plan Summary](#-test-plan-summary)
- [📝 Test Scenarios](#-test-scenarios)
- [🐛 Bug Report](#-bug-report)
- [✅ Final Verdict](#-final-verdict)
- [📁 Deliverables](#-deliverables)

---

## 🎯 Project Overview

| Field | Details |
|---|---|
| 🌐 **Application** | othoba.com — E-Commerce Platform |
| 🔗 **URL** | https://othoba.com/ |
| 👤 **Tester** | MD Mahedy Hasan |
| 🌍 **Profile** | [Naiem.Website](https://Naiem.Website) |
| 🗓️ **Test Period** | May 2026 |
| 🖥️ **Browsers Tested** | Chrome · Firefox · Edge · Brave |
| 🔬 **Test Types** | Functional · UI · Compatibility |
| 📦 **Total Modules** | 8 |
| 📄 **Total Test Cases** | 29 |

---

## 📊 Test Metrics at a Glance

### 🔢 Overall Results

```
Total Test Cases   ████████████████████████████░░  29
Passed             ████████████████████████░░░░░░  24  (82.76%)
Failed             ████░░░░░░░░░░░░░░░░░░░░░░░░░░   5  (17.24%)
Bugs Found         ████░░░░░░░░░░░░░░░░░░░░░░░░░░   5
```

### 📦 Module-wise Results

| Module | Total | ✅ Pass | ❌ Fail | Pass % |
|---|:---:|:---:|:---:|:---:|
| 🌐 Account / Browser | 1 | 1 | 0 | `100%` |
| 📝 Register | 11 | 7 | 4 | `63.64%` |
| 🔑 Login | 6 | 6 | 0 | `100%` |
| 🧭 Navigation Bar | 2 | 2 | 0 | `100%` |
| 🏠 Header | 4 | 4 | 0 | `100%` |
| 🛍️ Product Page | 2 | 2 | 0 | `100%` |
| 🛒 Cart | 2 | 2 | 0 | `100%` |
| 🚪 Logout | 1 | 1 | 0 | `100%` |
| **🔢 Total** | **29** | **24** | **5** | **`82.76%`** |

### 🐛 Bug Severity Breakdown

| Severity | Count | Visual |
|---|:---:|---|
| 🔴 Critical | 1 | `█░░░░` |
| 🟠 High | 2 | `██░░░` |
| 🟡 Medium | 1 | `█░░░░` |
| 🔵 Low | 1 | `█░░░░` |

---

## 🗺️ Mind Map — Testing Coverage

```
othoba.com Testing
│
├── 🌐 1. Account / Browser Compatibility
│   ├── ✅ Chrome
│   ├── ✅ Mozilla Firefox
│   ├── ✅ Microsoft Edge
│   └── ✅ Brave
│
├── 📝 2. Register
│   ├── Valid Field Tests
│   │   ├── ✅ Valid Phone Number
│   │   └── ✅ First Name Required
│   ├── Invalid / Missing Field Tests (BUGS FOUND)
│   │   ├── ❌ Invalid Email Accepted        ← BUG-001 [CRITICAL]
│   │   ├── ❌ Gender Not Mandatory          ← BUG-002 [HIGH]
│   │   ├── ❌ Last Name Not Required        ← BUG-003 [HIGH]
│   │   ├── ✅ DOB Date Required
│   │   ├── ✅ DOB Month Required
│   │   ├── ✅ DOB Year Required
│   │   ├── ✅ Password Required
│   │   └── ✅ Confirm Password Required
│   └── UI Checks
│       └── ❌ Font/Color Inconsistency     ← BUG-004 [MEDIUM]
│
├── 🔑 3. Login
│   ├── Positive Tests
│   │   └── ✅ Valid Credentials Login
│   ├── Negative Tests
│   │   ├── ✅ Empty Fields → Error Shown
│   │   ├── ✅ Wrong Password → Error Shown
│   │   └── ✅ Wrong Phone → Error Shown
│   ├── ✅ Forgot Password Redirect
│   ├── ✅ Login Page UI — All Fields Present
│   └── ⚠️  Error Message Mismatch          ← BUG-005 [LOW]
│
├── 🧭 4. Navigation Bar
│   ├── ✅ GET APP DEALS → App Download Page
│   └── ✅ Sell on othoba → Login/Signup
│
├── 🏠 5. Header
│   ├── ✅ Logo Visible & Aligned
│   ├── ✅ Search Returns Valid Results
│   ├── ✅ Wishlist Icon Redirect
│   └── ✅ Compare Icon Functionality
│
├── 🛍️ 6. Product Page
│   ├── ✅ Add to Cart → Success Message
│   └── ✅ Product Image Zoom on Hover
│
├── 🛒 7. Cart
│   ├── ✅ Increase Quantity → Price Updates
│   └── ✅ Remove Item → Cart Updates
│
└── 🚪 8. Logout
    └── ✅ Logout → Redirected to Homepage
```

---

## 📋 Test Plan Summary

### 🎯 Objective
> Validate the **functional correctness**, **UI/UX quality**, and **cross-browser compatibility** of the othoba.com e-commerce platform — covering Registration, Login, Navigation, Product Search, Cart, and Logout modules.

### ✅ Entry Criteria
- [x] Test cases written & reviewed
- [x] Test environment configured
- [x] Browser versions confirmed (Chrome, Firefox, Edge, Brave)
- [x] Test data prepared

### 🏁 Exit Criteria
- [x] All 29 test cases executed
- [ ] No Critical/High bugs open *(2 High + 1 Critical still open)*
- [x] Pass rate ≥ 80% *(achieved: 82.76%)*
- [x] Bug report submitted

### ⚠️ Risks & Assumptions

| Type | Description |
|---|---|
| ⚠️ Risk | Dynamic content may change between test runs |
| ⚠️ Risk | No backend/DB access to verify server-side validation |
| ℹ️ Assumption | Test data (phone, email) is disposable / non-production |
| ℹ️ Assumption | Screenshots referenced as "Click here" stored separately |

---

## 📝 Test Scenarios

<details>
<summary><b>📂 Register Module (11 Test Cases)</b></summary>

| ID | Scenario | Priority | Status |
|---|---|:---:|:---:|
| TS-REG-01 | Invalid Phone Number Rejected | 🟠 High | ✅ Pass |
| TS-REG-02 | Invalid Email Accepted *(Bug)* | 🔴 Critical | ❌ Fail |
| TS-REG-03 | Gender Field Not Mandatory *(Bug)* | 🟠 High | ❌ Fail |
| TS-REG-04 | First Name Required Field | 🟠 High | ✅ Pass |
| TS-REG-05 | Last Name Not Mandatory *(Bug)* | 🟠 High | ❌ Fail |
| TS-REG-06 | DOB Date Dropdown Required | 🟡 Medium | ✅ Pass |
| TS-REG-07 | DOB Month Dropdown Required | 🟡 Medium | ✅ Pass |
| TS-REG-08 | DOB Year Dropdown Required | 🟡 Medium | ✅ Pass |
| TS-REG-09 | Password Field Required | 🟠 High | ✅ Pass |
| TS-REG-10 | Confirm Password Required | 🟠 High | ✅ Pass |
| TS-REG-11 | UI / Font & Color Consistency *(Bug)* | 🟡 Medium | ❌ Fail |

</details>

<details>
<summary><b>📂 Login Module (6 Test Cases)</b></summary>

| ID | Scenario | Priority | Status |
|---|---|:---:|:---:|
| TS-LOG-01 | Login with Valid Credentials | 🔴 Critical | ✅ Pass |
| TS-LOG-02 | Login with Empty Fields | 🟠 High | ✅ Pass |
| TS-LOG-03 | Login with Wrong Password | 🟠 High | ✅ Pass |
| TS-LOG-04 | Login with Wrong Phone | 🟠 High | ✅ Pass |
| TS-LOG-05 | Forgot Password Redirect | 🟡 Medium | ✅ Pass |
| TS-LOG-06 | Login Page Field Presence | 🔵 Low | ✅ Pass |

</details>

<details>
<summary><b>📂 Navigation, Header, Product, Cart & Logout (12 Test Cases)</b></summary>

| ID | Scenario | Priority | Status |
|---|---|:---:|:---:|
| TS-NAV-01 | GET APP DEALS Redirect | 🟡 Medium | ✅ Pass |
| TS-NAV-02 | Sell on othoba Redirect | 🟡 Medium | ✅ Pass |
| TS-HDR-01 | Logo Visibility & Link | 🔵 Low | ✅ Pass |
| TS-HDR-02 | Product Search Returns Results | 🟠 High | ✅ Pass |
| TS-HDR-03 | Wishlist Icon Redirect | 🟡 Medium | ✅ Pass |
| TS-HDR-04 | Compare Icon Functionality | 🟡 Medium | ✅ Pass |
| TS-PRD-01 | Add to Cart Functionality | 🔴 Critical | ✅ Pass |
| TS-PRD-02 | Product Image Zoom on Hover | 🔵 Low | ✅ Pass |
| TS-CRT-01 | Quantity Increase Updates Price | 🟠 High | ✅ Pass |
| TS-CRT-02 | Remove Item from Cart | 🟠 High | ✅ Pass |
| TS-ACC-01 | Cross-Browser Compatibility | 🔵 Low | ✅ Pass |
| TS-OUT-01 | Logout Redirects Correctly | 🟡 Medium | ✅ Pass |

</details>

---

## 🐛 Bug Report

### BUG-001 — 🔴 CRITICAL
```
Title     : Invalid Email Accepted During Registration
Module    : Register
Test Case : TC-03
Severity  : Critical  |  Priority: High
Status    : OPEN

Steps to Reproduce:
  1. Open https://othoba.com/
  2. Click Register
  3. Enter "me@ofjgm.com" as email
  4. Fill all other fields with valid data
  5. Submit the form

Expected : Error — "Please enter a valid email address"
Actual   : ❌ Registration succeeded with invalid email format

Dev Note : Server-side email validation required
```

---

### BUG-002 — 🟠 HIGH
```
Title     : Gender Field Is Not Mandatory
Module    : Register
Test Case : TC-04
Severity  : High  |  Priority: High
Status    : OPEN

Steps to Reproduce:
  1. Open https://othoba.com/
  2. Click Register
  3. Leave Male/Female unselected
  4. Fill all other required fields
  5. Submit

Expected : Error — "Please select your gender"
Actual   : ❌ Registration completed without gender selection

Dev Note : Gender field should be marked as required
```

---

### BUG-003 — 🟠 HIGH
```
Title     : Last Name Field Is Not Required
Module    : Register
Test Case : TC-06
Severity  : High  |  Priority: Medium
Status    : OPEN

Steps to Reproduce:
  1. Open https://othoba.com/
  2. Click Register
  3. Leave last name blank
  4. Fill all other fields
  5. Submit

Expected : Error — "Last name is required"
Actual   : ❌ Registration completed without last name

Dev Note : Add required validation to last name field
```

---

### BUG-004 — 🟡 MEDIUM
```
Title     : UI Inconsistency — First Name Field Style
Module    : Register
Test Case : TC-18
Severity  : Medium  |  Priority: Low
Status    : OPEN

Steps to Reproduce:
  1. Open https://othoba.com/
  2. Click Register
  3. Observe First Name field font, color, and size

Expected : Consistent styling with all other form fields
Actual   : ❌ First Name field has visual mismatch

Dev Note : Align UI to design spec
```

---

### BUG-005 — 🔵 LOW
```
Title     : Login Error Message Missing "Phone" Reference
Module    : Login
Test Case : TC-13
Severity  : Low  |  Priority: Low
Status    : OPEN

Steps to Reproduce:
  1. Open https://othoba.com/
  2. Click Login
  3. Leave email & phone fields blank
  4. Click Login button

Expected : "Please enter your email or phone number"
Actual   : ❌ Shows only "Please enter your email"

Dev Note : Update error copy to mention phone as well
```

---

## ✅ Final Verdict

```
┌─────────────────────────────────────────────────────────┐
│                  OVERALL QA VERDICT                     │
│                                                         │
│   Pass Rate    :  82.76%  ████████████████████░░░░      │
│   Fail Rate    :  17.24%  ████░░░░░░░░░░░░░░░░░░░░      │
│                                                         │
│   Critical Bugs Open  :  1  🔴                          │
│   High Bugs Open      :  2  🟠                          │
│   Medium / Low Open   :  2  🟡🔵                        │
│                                                         │
│   RECOMMENDATION:                                       │
│   ⚠️  DO NOT RELEASE until BUG-001 (Critical) and       │
│      BUG-002, BUG-003 (High) are fixed and retested.   │
└─────────────────────────────────────────────────────────┘
```

### 🔧 Recommended Fix Priority

1. 🔴 **BUG-001** — Fix email validation (server-side) — *Release Blocker*
2. 🟠 **BUG-002** — Make gender field mandatory
3. 🟠 **BUG-003** — Make last name field mandatory
4. 🟡 **BUG-004** — Fix First Name field UI styling
5. 🔵 **BUG-005** — Update login error message copy

---

## 📁 Deliverables

| File | Description |
|---|---|
| 📊 `othoba_QA_Report_MahBudyHasan.xlsx` | Full Excel report — Test Plan, Scenarios, Bug Report, Metrics, Mind Map |
| 📄 `README.md` | This document — full visual overview |

---

<div align="center">

---

**MD Mahedy Hasan**  
QA Engineer · [Naiem.Website](https://Naiem.Website)  
Testing Site: [https://othoba.com/](https://othoba.com/)

*© 2026 — All testing performed manually on live environment*

</div>
