# Test Case Design — GroceryMate Webshop (Upcoming Release)

This document contains **test case designs only**.  
Execution will be performed in a later testing phase.

---

## 1. Product Rating System

### Test Design Techniques:
- Equivalence Partitioning (EP)
- Boundary Value Analysis (BVA)
- Use Case Testing
- Error Guessing
- Security Testing

---

### Boundary Value Analysis:
**Test Case:** Verify submission of minimum allowed star rating  
**Input:** Rating = 1 star  
**Expected Outcome:** Rating is accepted and saved successfully.

---

### Boundary Value Analysis:
**Test Case:** Verify submission of maximum allowed star rating  
**Input:** Rating = 5 stars  
**Expected Outcome:** Rating is accepted and saved successfully.

---

### Equivalence Partitioning:
**Test Case:** Verify valid rating submission by logged-in user  
**Input:** Logged-in user submits a valid star rating (1–5)  
**Expected Outcome:** Rating is saved and reflected in the product rating summary.

---

### Equivalence Partitioning:
**Test Case:** Verify guest user behavior when attempting to rate  
**Input:** Guest user attempts to submit a rating  
**Expected Outcome:** Rating is not accepted; user is prompted to log in or register.

---

### Error Guessing:
**Test Case:** Verify system behavior when no star rating is selected  
**Input:** Submit rating form without selecting stars  
**Expected Outcome:** Error message displayed indicating rating selection is required.

---

### Error Guessing:
**Test Case:** Verify system behavior for invalid rating values  
**Input:** Rating value outside allowed range (e.g., 0 or 6 via request manipulation)  
**Expected Outcome:** Rating is rejected; invalid data is not stored.

---

### Boundary Value Analysis (Text Input):
**Test Case:** Verify written feedback exceeding maximum character limit  
**Input:** Feedback text exceeding maximum allowed length  
**Expected Outcome:** Error message displayed indicating character limit exceeded.

---

### Security Testing:
**Test Case:** Verify XSS prevention in rating feedback  
**Input:** Feedback containing script or HTML tags  
**Expected Outcome:** Script does not execute; input is sanitized or rejected.

---

### Use Case Testing:
**Test Case:** Verify average rating update after multiple user ratings  
**Input:** Multiple users submit ratings for the same product  
**Expected Outcome:** Average rating and rating count are recalculated correctly.

---

## 2. Age Verification for Alcoholic Products

### Test Design Techniques:
- Boundary Value Analysis (BVA)
- Equivalence Partitioning (EP)
- Use Case Testing
- Error Guessing
- Security Testing

---

### Use Case Testing:
**Test Case:** Verify age verification prompt when accessing alcohol category  
**Input:** User navigates to Alcohol category  
**Expected Outcome:** Age verification modal is displayed before access is granted.

---

### Boundary Value Analysis:
**Test Case:** Verify access denial for underage user  
**Input:** Age = 17  
**Expected Outcome:** Access denied with appropriate underage message.

---

### Boundary Value Analysis:
**Test Case:** Verify access granted at minimum allowed age  
**Input:** Age = 18  
**Expected Outcome:** Access to alcoholic products is granted.

---

### Equivalence Partitioning:
**Test Case:** Verify access for users above minimum age  
**Input:** Age > 18  
**Expected Outcome:** Alcohol category is accessible.

---

### Error Guessing:
**Test Case:** Verify behavior for invalid age input  
**Input:** Empty field, non-numeric input, or future date  
**Expected Outcome:** Validation error displayed; access denied.

---

### Security Testing:
**Test Case:** Verify alcohol product access via direct URL without verification  
**Input:** Directly open alcoholic product URL  
**Expected Outcome:** Access blocked or age verification enforced.

---

### Use Case Testing:
**Test Case:** Verify re-verification after session or cookie clearance  
**Input:** Clear session/cookies and revisit Alcohol category  
**Expected Outcome:** Age verification modal appears again.

---

## 3. Shipping Cost Changes

### Test Design Techniques:
- Boundary Value Analysis (BVA)
- Equivalence Partitioning (EP)
- Use Case Testing
- Error Guessing

---

### Equivalence Partitioning:
**Test Case:** Verify shipping fee applied below free-shipping threshold  
**Input:** Cart total below defined threshold  
**Expected Outcome:** Shipping fee is applied to order total.

---

### Boundary Value Analysis:
**Test Case:** Verify shipping behavior at exact threshold value  
**Input:** Cart total equals free-shipping threshold  
**Expected Outcome:** System applies shipping rule as defined (free or charged).

---

### Equivalence Partitioning:
**Test Case:** Verify free shipping above threshold  
**Input:** Cart total exceeds free-shipping threshold  
**Expected Outcome:** Shipping cost is zero or marked as free.

---

### Use Case Testing:
**Test Case:** Verify shipping recalculation when cart quantity changes  
**Input:** Increase or decrease item quantity around threshold  
**Expected Outcome:** Shipping cost recalculates correctly in real time.

---

### Use Case Testing:
**Test Case:** Verify shipping cost consistency across checkout flow  
**Input:** View cart → checkout → order confirmation  
**Expected Outcome:** Shipping cost remains consistent across all stages.

---

### Error Guessing:
**Test Case:** Verify shipping cost behavior for empty cart  
**Input:** No items in cart  
**Expected Outcome:** No shipping fee is displayed.

---

## 4. Regression Considerations (High-Level)

### Use Case Testing:
**Test Case:** Verify search and sorting functionality after changes  
**Expected Outcome:** Search and sort behave as before with no regression.

---

### Use Case Testing:
**Test Case:** Verify favorites functionality remains unaffected  
**Expected Outcome:** Users can add and remove favorites successfully.

---

### Use Case Testing:
**Test Case:** Verify checkout form validation remains intact  
**Expected Outcome:** Field-level validation messages appear correctly.
