# GroceryMate – Defect Report

## Issue 01 — Weak Password Accepted During Signup

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Severity
High

## Priority
High

## Type
Security / Validation Defect

---

## Description
The system allows users to register or use very weak passwords without enforcing password strength rules.

During testing, a weak password was accepted. The only warning displayed came from the browser’s password manager, not from the application itself.

The application should implement its own password strength validation.

---

## Steps to Reproduce
1. Navigate to Signup page
2. Enter user details
3. Enter weak password (e.g., 12345 or simple numeric password)
4. Submit form

---

## Expected Result
- Weak passwords rejected
- Password policy enforced (minimum length, complexity, special characters)
- Clear validation error message displayed

---

## Actual Result
- Weak password accepted
- No application-level validation message
- Only external browser warning shown

---

## Impact
- Security vulnerability
- Increased risk of account compromise
- Non-compliance with basic authentication standards

---

## Status
❌ FAIL

---<img width="1532" height="1022" alt="1  Asking for a strong password" 
     src="https://github.com/user-attachments/assets/21ee89fc-1d1a-476e-8765-4d7c1ce53c1a" />

## Evidence
Screenshot 01

---
---
# GroceryMate – Defect Report

## Issue 02 — "Shop Now" CTA Button Not Navigating to Product Catalog

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Severity
Medium

## Priority
High

## Type
Functional / Navigation Defect

---

## Description
The "Shop Now" call-to-action button on the homepage does not navigate users to the product catalog or shop page.

Clicking the button results in no action or redirection, preventing users from accessing products directly from the homepage.

This breaks the primary shopping flow.

---

## Steps to Reproduce
1. Open homepage
2. Locate "Shop Now" button in banner section
3. Click the button

---

## Expected Result
- User redirected to Shop/Product listing page
- Product catalog loads successfully

---

## Actual Result
- No navigation occurs
- Page remains unchanged
- Shop page not opened

---

## Impact
- Users cannot easily access products
- Broken purchase journey
- Reduced usability and conversions
- Negative user experience

---

## Status
❌ FAIL

---

## Evidence
Screenshot 02

<img width="1170" height="958" alt="2  On home page shop now link isn&#39;t functional" src="https://github.com/user-attachments/assets/cfc3b825-ffaf-4aac-b80b-be7463cb1dac" />

---
---

# GroceryMate – Defect Report

## Issue 03 — Price Filter Displays Products Outside Selected Range

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Severity
Medium

## Priority
Medium

## Type
Functional / Filtering Defect

---

## Description
The price filter does not correctly restrict products based on the selected price range.

When a price range below €20 is selected, products priced above €20 are still displayed in the product listing.

The filtering logic is not applied properly.

---

## Steps to Reproduce
1. Navigate to Shop page
2. Use "Filter by Pricing"
3. Select price range 0€–20€
4. Observe product list

---

## Expected Result
- Only products priced within €0–€20 are displayed
- All higher-priced products hidden

---

## Actual Result
- Products above €20 are still visible
- Filter criteria ignored

---

## Impact
- Incorrect search/filter results
- Poor user experience
- Users cannot find products within budget easily
- Reduces trust in filtering functionality

---

## Status
❌ FAIL

---

## Evidence
Screenshot 03

<img width="1697" height="922" alt="3  No items above Euro 20 still these prices are displayed" src="https://github.com/user-attachments/assets/df2e5b4e-aa5e-445f-a80b-950106a7b08f" />

---
---
