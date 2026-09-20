# Test Summary Report — SauceDemo

**Project:** SauceDemo (https://www.saucedemo.com) — manual functional testing
**Tester:** Oleksandr Khrystofor
**Date:** 19 September 2026
**Test management tool:** Qase.io
**Type of testing:** Manual, functional, exploratory (E2E)


## 1. Scope

Manual testing of the core user flows of the SauceDemo web store: login,
products & sorting, cart, checkout, and the side menu (logout / reset app state).
Backend, API, security and load testing were out of scope.

## 2. Test execution summary

| Metric | Value |
|--------|-------|
| Total test cases | 26 |
| Suites | 5 (Login, Products/Sorting, Cart, Checkout, Menu/Logout) |
| Executed | 26 |
| Passed | 25 |
| Failed | 1 |
| Completion rate | 100% |
| Defects logged | 3 |

Execution was performed as a structured test run under `standard_user`
(the reference account), followed by an exploratory session under
`problem_user` to surface account-specific defects.

## 3. Defects found

| # | Title | Severity | Account |
|---|-------|----------|---------|
| 1 | Reset App State clears the cart badge but does not reset product buttons from 'Remove' to 'Add to cart' | Minor | standard_user |
| 2 | All product preview images are identical/unrelated on the Products page | Major | problem_user |
| 3 | Sorting does not change product order when a sort option is selected | Minor | problem_user |

## 4. Conclusion

The core purchase flow works correctly under the standard account. The most
significant issues appear under `problem_user` (broken product images and
non-functional sorting), which would seriously affect a real shopper.
Recommended priority: fix the Major product-page defects first, then the
Minor Reset App State inconsistency.
