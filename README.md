# 🏦 Guru99 Bank — Manual Testing Portfolio

![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)
![Test Cases](https://img.shields.io/badge/Test%20Cases-200%2B-blue)
![Modules](https://img.shields.io/badge/Modules-14-green)
![SRS Version](https://img.shields.io/badge/SRS-v2.0-orange)

## 📌 Project Overview

This repository contains a complete **manual testing suite** for the **Guru99 Bank** web application — a demo net banking platform used for QC practice. All test cases, test plans, RTM, and bug report templates were derived from the official **Software Requirements Specification (SRS) v2.0**.

> This project is part of a personal QA portfolio to demonstrate manual testing skills including test planning, test case design, traceability, and defect reporting.

---

## 🌐 Application Under Test

| Field              | Details                              |
|--------------------|--------------------------------------|
| **Application**    | Guru99 Bank — Net Banking            |
| **URL**            | https://demo.guru99.com/V2/ |
| **Browser Support**| Chrome 27 and above (per SRS)       |
| **SRS Version**    | 2.0 (dated 19/11/2013)               |
| **Testing Type**   | Manual — Functional Testing          |

---

## 👥 User Roles

| Role        | Access Level                                                                 |
|-------------|------------------------------------------------------------------------------|
| **Manager** | Full access: manage customers, accounts, deposits, withdrawals, transfers    |
| **Customer**| Limited access: own accounts only — balance, transfer, statement, password   |

> ⚠️ **Note:** The **Customer portal** was not accessible during test execution. Test cases for Customer-role features have been fully designed based on SRS requirements but are marked as `Not Executed`. They are ready to be executed once access is available.

---

## 📦 Modules Covered

| #  | Module                | Manager | Customer |
|----|----------------------|---------|----------|
| 1  | Login & Logout        | ✅       | ✅        |
| 2  | New Customer          | ✅       | —         |
| 3  | Edit Customer         | ✅       | —         |
| 4  | Delete Customer       | ✅       | —         |
| 5  | New Account           | ✅       | —         |
| 6  | Edit Account          | ✅       | —         |
| 7  | Delete Account        | ✅       | —         |
| 8  | Deposit               | ✅       | —         |
| 9  | Withdrawal            | ✅       | —         |
| 10 | Fund Transfer         | ✅       | ✅        |
| 11 | Balance Enquiry       | ✅       | ✅        |
| 12 | Mini Statement        | ✅       | ✅        |
| 13 | Customized Statement  | ✅       | ✅        |
| 14 | Change Password       | ✅       | ✅        |

---

## 📁 Repository Structure

```
guru99-bank-manual-testing/
│
├── README.md                                  ← Project overview (this file)
│
├── 01_Test_Plan/
│   └── Test_Plan.md                           ← Scope, approach, entry/exit criteria, risks
│
├── 02_Test_Cases/
│   └── Test_Cases.xlsx                        ← 214 TCs across 14 modules (1 sheet per module)
│                                                 Columns: TC ID | Title | Role | Precondition |
│                                                          Steps | Test Data | Expected | Actual | Status
│
├── 03_RTM/
│   └── RTM.xlsx                               ← Full traceability: T1–T110 + F1–F49 → Test Cases
│                                                 100% requirements coverage
│
├── 04_Bug_Reports/
│   └── Bug_Reports.xlsx                       ← Bug log + severity/priority reference guide
│
├── 05_Test_Summary_Report/
│   └── Test_Summary_Report.md                 ← Execution results, pass/fail counts, coverage
│
└── Assets/
    └── SRS_v2_original.docx                   ← Source requirements document (SRS v2.0)
```

---

## 📊 Requirements Coverage

| Requirement Type             | Count | Covered |
|-----------------------------|-------|---------|
| Technical Requirements (T)  | 110   | 110     |
| Functional Validations (F)  | 49    | 49      |
| **Total**                   | **159** | **159** |

---

## 🧪 Test Execution Status

> Results to be updated after execution.

| Module                | Total TCs | Pass | Fail | Not Executed |
|-----------------------|-----------|------|------|--------------|
| Login & Logout        | —         | —    | —    | —            |
| New Customer          | —         | —    | —    | —            |
| Edit Customer         | —         | —    | —    | —            |
| Delete Customer       | —         | —    | —    | —            |
| New Account           | —         | —    | —    | —            |
| Edit Account          | —         | —    | —    | —            |
| Delete Account        | —         | —    | —    | —            |
| Deposit               | —         | —    | —    | —            |
| Withdrawal            | —         | —    | —    | —            |
| Fund Transfer         | —         | —    | —    | —            |
| Balance Enquiry       | —         | —    | —    | —            |
| Mini Statement        | —         | —    | —    | —            |
| Customized Statement  | —         | —    | —    | —            |
| Change Password       | —         | —    | —    | —            |

---

## 🛠️ Tools Used

- **Test Cases / RTM / Bug Reports:** Microsoft Excel (.xlsx) — industry standard format
- **Test Plan / Summary Report:** Markdown (.md) — rendered natively on GitHub
- **Bug Tracking:** Manual bug log in Excel (Bug_Reports.xlsx)
- **Browser:** Firefox 148.0 (64-bit)
- **Version Control:** GitHub

---

## 👤 Author

**[Ahmed Abdelmawgod]**  
QC Engineer | Manual Testing Portfolio  
[LinkedIn](https://www.linkedin.com/in/ahmed-abdelmawgod5#) | [GitHub](https://github.com/Ahmed35003/#)
