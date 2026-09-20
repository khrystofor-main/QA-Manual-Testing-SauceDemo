# SauceDemo — Manual Testing Project

Manual functional and exploratory testing of the [SauceDemo](https://www.saucedemo.com)
web store, managed in **Qase.io**. This project demonstrates the full manual
QA workflow: test planning, test case design, test execution and defect
reporting.

## About

- **Application under test:** SauceDemo (https://www.saucedemo.com)
- **Type of testing:** Manual, functional, exploratory (E2E)
- **Tools:** Qase.io (test management)
- **Tester:** Oleksandr Khrystofor

## What this project covers

- A **Test Plan** defining scope, approach, environment and entry/exit criteria
- **26 test cases** across 5 suites: Login, Products/Sorting, Cart, Checkout, Menu/Logout
- A structured **test run** (25 passed / 1 failed)
- An **exploratory session** under broken account (`problem_user`)
- **3 documented defects** with steps to reproduce, severity and screenshots

## Repository structure

```
saucedemo-manual-testing/
├── evidence/               <- (test run dashboard + defect evidence)
├── README.md
├── defects.md
├── test-cases.csv          <- (exported from Qase)
├── test-plan.md            <- (Start here)
└── test-summary-report.md
```

## Results at a glance

| Metric | Value |
|--------|-------|
| Test cases | 26 |
| Passed | 25 |
| Failed | 1 |
| Defects logged | 3 (2 Major, 1 Minor) |

## Key defects

1. **All product images identical (problem_user)** — Major
2. **Sorting does not change product order (problem_user)** — Minor
3. **Reset App State does not reset product buttons** — Minor

See `test-summary-report.md` for the full report.

## Skills demonstrated

- Test case design (positive/negative, boundary cases)
- Defect reporting with clear, reproducible steps and severity/priority
- Exploratory testing
- Working in a test management system (Qase.io)
