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
FAIL

## Evidence
Screenshot 01

---<img width="1532" height="1022" alt="1  Asking for a strong password" 
     src="https://github.com/user-attachments/assets/21ee89fc-1d1a-476e-8765-4d7c1ce53c1a" />


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
FAIL

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
FAIL

---

## Evidence
Screenshot 03

<img width="1697" height="922" alt="3  No items above Euro 20 still these prices are displayed" src="https://github.com/user-attachments/assets/df2e5b4e-aa5e-445f-a80b-950106a7b08f" />

---
---

# GroceryMate – Defect Report

## Issue 04 — Fruits Displayed Under Vegetables Category (Incorrect Product Classification)

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
Data / Catalog Classification Defect

---

## Description
Products that belong to the Fruits category are incorrectly listed under the "Fresh Vegetables" category.

This indicates improper product classification or missing category separation in the catalog.

Fruits and vegetables should be organized into their respective categories for accurate browsing and filtering.

---

## Steps to Reproduce
1. Navigate to Shop page
2. Open "Fresh Vegetables" category
3. Observe listed products

---

## Expected Result
- Only vegetable products displayed
- Fruits appear under a separate "Fruits" category

---

## Actual Result
- Fruit products (e.g., apples) shown in Vegetables category
- No proper category separation

---

## Impact
- Confusing navigation
- Poor user experience
- Incorrect filtering/search behavior
- Reduces catalog accuracy and professionalism

---

## Status
FAIL

---

## Evidence
Screenshot 04
<img width="1697" height="922" alt="4  Fruits are available in vegetable category, no separate category for fruits" src="https://github.com/user-attachments/assets/585ab8f8-0356-4e90-bdf5-5a56eabd32af" />

---
---

# GroceryMate – Defect Report

## Issue 05 — Missing Product Image in Product Listing

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Severity
Low

## Priority
Medium

## Type
UI / Content Defect

---

## Description
One or more products in the catalog are displayed without an image.

The product card shows a blank or broken image area instead of the expected product photo.

Product images are essential for identification and purchasing decisions.

---

## Steps to Reproduce
1. Navigate to Shop/Product listing page
2. Scroll through product catalog
3. Observe product cards

---

## Expected Result
- Every product displays a valid image
- No broken or empty image placeholders

---

## Actual Result
- Product displayed without image
- Visual placeholder or blank space shown

---

## Impact
- Poor user experience
- Reduced product clarity
- Lower customer trust
- Potential decrease in conversions

---

## Status
FAIL

---

## Evidence
Screenshot 05

<img width="1080" height="427" alt="5  Absent photo for web store purchaser" src="https://github.com/user-attachments/assets/a60475c0-3012-4d38-aa76-86135ec44800" />

---
---

# GroceryMate – Defect Report

## Issue 06 — Meat & Poultry Products Displayed in Vegetables Category

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
Data / Catalog Classification Defect

---

## Description
Products belonging to the Meat & Poultry category are incorrectly displayed under the "Fresh Vegetables" category.

This is a serious product classification issue that can mislead customers and cause confusion while browsing.

Proper categorization is critical for accurate filtering and user trust.

---

## Steps to Reproduce
1. Navigate to Shop page
2. Open "Fresh Vegetables" category
3. Observe listed products

---

## Expected Result
- Only vegetable products displayed
- Meat & poultry products appear only in their correct category

---

## Actual Result
- Meat & poultry items visible inside Vegetables category

---

## Impact
- Incorrect product discovery
- Confusing user experience
- Potential dietary/religious concerns for customers
- Reduces trust in product organization

---

## Status
FAIL

---

## Evidence
Screenshot 06

<img width="1020" height="406" alt="6  Meat and Poultry item in vegrtable section" src="https://github.com/user-attachments/assets/132ea202-4655-4ee0-96d1-6f0c841ab160" />


---
---

# GroceryMate – Defect Report

## Issue 07 — Shipping Fee Always Calculated as €0 Regardless of Cart Total

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
Business Logic / Pricing Defect

---

## Description
The system calculates the shipping cost as €0 for all cart totals.

Shipping charges are not applied even when the cart value is below the free-shipping threshold.

This indicates that the shipping fee calculation logic is not functioning correctly.

---

## Steps to Reproduce
1. Add low-priced product(s) to cart
2. Ensure cart total is below free-shipping threshold
3. Open cart or checkout page
4. Observe shipping cost

---

## Expected Result
- Shipping fee applied when cart total is below threshold
- Free shipping only when threshold conditions are met

---

## Actual Result
- Shipping cost displayed as €0 for all totals
- No fee applied

---

## Impact
- Direct revenue loss
- Incorrect order pricing
- Business rule violation
- Financial risk for store

---

## Status
FAIL

---

## Evidence
Screenshot 07

<img width="478" height="650" alt="7  For all values the shipment charge is 0" src="https://github.com/user-attachments/assets/fda77984-9c8a-4563-8717-b0f51874d280" />

---
---

# GroceryMate – Defect Report

## Issue 08 — CVV Number Visible in Plain Text (Sensitive Data Exposure)

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Severity
Critical

## Priority
Blocker

## Type
Security / Payment Data Exposure

---

## Description
The CVV (Card Verification Value) is displayed in plain text on the payment/checkout screen.

Sensitive payment information should never be visible or stored in readable format.

CVV must be masked and handled securely according to PCI-DSS compliance standards.

Displaying this information exposes users to fraud and serious security risks.

---

## Steps to Reproduce
1. Navigate to Checkout page
2. Enter card details including CVV
3. Observe how CVV is displayed

---

## Expected Result
- CVV field masked (***)
- CVV not stored or displayed after entry
- Sensitive data hidden from UI

---

## Actual Result
- CVV displayed in plain text
- Sensitive information visible on screen

---

## Impact
- Severe security vulnerability
- Risk of payment fraud
- Non-compliance with PCI-DSS standards
- Legal and financial liability
- Loss of customer trust

---

## Status
FAIL

---

## Evidence
Screenshot 08

<img width="507" height="627" alt="8  CVV is getting displayed" src="https://github.com/user-attachments/assets/c707b3e7-63f4-4851-8a01-140e97646c8e" />

---
---

# GroceryMate – Defect Report

## Issue 09 — Free Shipping Message Displayed Incorrectly When Conditions Not Met

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
Business Logic / UI Messaging Defect

---

## Description
The system displays a free-shipping promotional message even when the cart total does not meet the required free-shipping threshold.

This results in inconsistent and misleading information being presented to users.

Shipping eligibility messaging should accurately reflect the actual cart conditions.

---

## Steps to Reproduce
1. Add items to cart below free-shipping threshold
2. Navigate to cart page
3. Observe shipping or promotional message

---

## Expected Result
- Free-shipping message hidden when threshold not met
OR
- Message clearly indicates remaining amount needed for free shipping

---

## Actual Result
- Free-shipping message displayed despite cart being below threshold
- Messaging contradicts pricing rules

---

## Impact
- Confusing user experience
- Misleading pricing information
- Potential customer dissatisfaction
- Reduced trust in checkout calculations

---

## Status
FAIL

---

## Evidence
Screenshot 09

<img width="467" height="532" alt="9  Free shipment clause is redered void" src="https://github.com/user-attachments/assets/afdc4b9e-3e09-4137-874d-3a2d6a14cf26" />

---
---

# GroceryMate – Defect Report

## Issue 10 — Age Verification Not Enforced During Alcohol Purchase (Bypass Possible)

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Severity
Critical

## Priority
Blocker

## Type
Security / Compliance / Business Rule Defect

---

## Description
The system does not enforce age verification when purchasing alcoholic products.

Users are able to add alcohol items to the cart and proceed through checkout without being prompted for age confirmation.

This allows underage users to potentially purchase restricted products.

Age verification must be mandatory before accessing or purchasing alcoholic items.

---

## Steps to Reproduce
1. Navigate to alcohol product page
2. Add alcoholic product to cart
3. Proceed to checkout
4. Observe verification behavior

---

## Expected Result
- Age verification modal displayed before checkout
- Purchase blocked until age eligibility confirmed
- Underage users denied access

---

## Actual Result
- No age verification requested
- Checkout proceeds normally
- Alcohol purchase allowed without validation

---

## Impact
- Legal and regulatory violations
- Risk of selling alcohol to minors
- Compliance failure
- Potential fines or penalties
- Serious reputational damage

---

## Status
FAIL

---

## Evidence
Screenshot 10

<img width="460" height="398" alt="10  Didn&#39;t check for age while purchasing alcohol" src="https://github.com/user-attachments/assets/6a234172-d14a-4de6-a678-9d8a7962ef01" />

---
---

# GroceryMate – Defect Report

## Issue 11 — Search Results Do Not Display All Matching Products

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
Functional / Search Defect

---

## Description
The search functionality does not return all products that match the entered keyword.

When searching for a product category or keyword, only partial results are displayed even though additional relevant products exist in the catalog.

This indicates incomplete or incorrect search indexing/filtering logic.

---

## Steps to Reproduce
1. Open homepage
2. Enter a keyword in search bar (e.g., "cleaning")
3. View search results

---

## Expected Result
- All matching products displayed
- Complete and accurate results returned

---

## Actual Result
- Only limited products shown
- Other relevant items missing

---

## Impact
- Users cannot find products easily
- Poor search experience
- Reduced sales opportunities
- Decreased usability

---

## Status
FAIL

---

## Evidence
Screenshot 11

<img width="640" height="128" alt="11  Search doesn&#39;t display all the items belonging to that category" src="https://github.com/user-attachments/assets/e810001f-fc15-4e7a-b5f9-90a019f59bb4" />

---
---

# GroceryMate – Test Execution Report

## Test Case 12 — Product Rating System Functionality

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Test Type
Functional Testing

## Test Technique
Use Case Testing / Equivalence Partitioning

---

## Test Scenario
Verify that a logged-in user can submit a rating and that the product rating system updates correctly while preventing duplicate reviews.

---

## Preconditions
- User logged in
- Product detail page open

---

## Steps to Reproduce
1. Open product page
2. Submit star rating
3. Add review comment
4. Submit review
5. Attempt to review same product again

---

## Expected Result
- Rating saved successfully
- Rating count updated
- Average rating recalculated
- Review displayed in comments
- Duplicate review prevented with message

---

## Actual Result
- Rating displayed correctly
- Review added successfully
- Rating summary updated
- System shows message: "You have already reviewed this product"
- Duplicate submission blocked

---

## Status
PASS

---

## Severity
Low

## Priority
Medium

---

## Notes
Product rating system functions correctly.  
Validation prevents multiple reviews from the same user.

---

## Evidence
Screenshot 12

<img width="1103" height="930" alt="12  Product rating system" src="https://github.com/user-attachments/assets/e01b3e3e-0fe7-4f44-bd0c-b696d7248c0a" />

---
---

# GroceryMate – Test Execution Report

## Test Case 13 — Rating Boundary Value (Maximum = 5 Stars)

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Test Type
Functional Testing

## Test Technique
Boundary Value Analysis (BVA)

---

## Test Scenario
Verify that the system accepts the maximum valid rating value (5 stars).

---

## Preconditions
- User logged in
- Product detail page open
- Rating control visible

---

## Steps to Reproduce
1. Open any product page
2. Select 5-star rating
3. Add optional comment
4. Submit review

---

## Expected Result
- Rating accepted
- Review submitted successfully
- No validation error
- Rating count updated

---

## Actual Result
- 5-star rating accepted
- Review saved successfully
- No error message displayed

---

## Status
PASS

---

## Severity
Low

## Priority
Low

---

## Notes
System correctly handles the maximum boundary value for rating input.

---

## Evidence
Screenshot 13

<img width="777" height="907" alt="1  Boundry Value Rating 5" src="https://github.com/user-attachments/assets/d46e439d-98aa-41e3-95b3-589d6a4dcc32" />

---
---

# GroceryMate – Test Execution Report

## Test Case 14 — Rating Boundary Value (Minimum = 1 Star)

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Test Type
Functional Testing

## Test Technique
Boundary Value Analysis (BVA)

---

## Test Scenario
Verify that the system accepts the minimum valid rating value (1 star).

---

## Preconditions
- User logged in
- Product detail page open
- Rating control available

---

## Steps to Reproduce
1. Open any product page
2. Select 1-star rating
3. Add optional comment
4. Submit review

---

## Expected Result
- Rating accepted
- Review saved successfully
- No validation error
- Rating included in overall average

---

## Actual Result
- 1-star rating accepted
- Review submitted successfully
- No error displayed

---

## Status
PASS

---

## Severity
Low

## Priority
Low

---

## Notes
System correctly handles the lower boundary value for rating input.  
Boundary validation works as expected.

---

## Evidence
Screenshot 14

<img width="391" height="906" alt="2  Boundry Value Rating 1" src="https://github.com/user-attachments/assets/f3075c06-4a4c-4850-9c7d-bc50be4868be" />

---
---

# GroceryMate – Test Execution Report

## Test Case 15 — Rating Submission (Valid Equivalence Partition = 4 Stars)

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Test Type
Functional Testing

## Test Technique
Equivalence Partitioning (EP)

---

## Test Scenario
Verify that the system accepts a valid rating value within the allowed range (1–5).

---

## Preconditions
- User logged in
- Product detail page open
- Rating widget visible

---

## Steps to Reproduce
1. Open any product page
2. Select 4-star rating
3. Enter comment (optional)
4. Submit review

---

## Expected Result
- Rating accepted
- Review saved successfully
- Rating count updated
- Average rating recalculated

---

## Actual Result
- 4-star rating accepted
- Review submitted successfully
- No validation error shown

---

## Status
PASS

---

## Severity
Low

## Priority
Low

---

## Notes
Represents normal valid input from the equivalence class (1–5).  
System behaves correctly for standard rating submissions.

---

## Evidence
Screenshot 15

<img width="392" height="907" alt="3  Equivalance Partitioning Rating 4" src="https://github.com/user-attachments/assets/e06b754e-01b4-4603-870c-31bba6c39c61" />

---
---

# GroceryMate – Test Execution Report

## Test Case 16 — Invalid Rating Value Rejected (Rating = 0)

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Test Type
Negative Testing

## Test Technique
Error Guessing

---

## Test Scenario
Verify that the system rejects invalid rating values outside the allowed range (1–5).

---

## Preconditions
- User logged in
- Product detail page open
- Rating control available

---

## Test Data
Rating = 0

---

## Steps to Reproduce
1. Attempt to submit rating value 0 (via UI or request manipulation)
2. Submit review form

---

## Expected Result
- Rating rejected
- Validation error message displayed
- No rating saved in system
- Database not updated

---

## Actual Result
- Rating submission blocked
- System does not accept 0 value
- No invalid rating stored

---

## Status
PASS

---

## Severity
Low

## Priority
Low

---

## Notes
System correctly validates rating boundaries and prevents invalid inputs.  
Demonstrates proper defensive validation.

---

## Evidence
Screenshot 16

![4  Error Guessing With Rating Zero](https://github.com/user-attachments/assets/cbb61eb2-1668-4e29-9cc6-79455ffa46cf)

---
---

# GroceryMate – Defect Report

## Issue 12 — Age Verification Not Triggered When Accessing Alcohol Products

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Severity
Critical

## Priority
Blocker

## Type
Security / Compliance Defect

---

## Description
The system does not enforce age verification when a user accesses alcoholic products.

Users can directly view alcohol product listings without being prompted to verify their age.

Age verification should be mandatory before allowing access to restricted products.

---

## Steps to Reproduce
1. Navigate directly to Alcohol category or alcoholic product page
2. Observe page behavior

---

## Expected Result
- Age verification modal displayed
- Access restricted until age confirmed
- Underage users denied access

---

## Actual Result
- No age verification prompt shown
- Alcohol products accessible immediately

---

## Impact
- Legal and regulatory violations
- Risk of underage access to alcohol
- Compliance failure
- Potential fines and penalties
- Reputational damage

---

## Status
FAIL

---

## Evidence
Screenshot 17

![5  Use Case Test - No age verification for alcoholic product](https://github.com/user-attachments/assets/fcb4428e-f156-4cfe-95c9-ac5457df1907)

---
---

# GroceryMate – Test Execution Report

## Test Case 17 — Shipping Fee Applied Below Free-Shipping Threshold

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Test Type
Functional Testing

## Test Technique
Equivalence Partitioning (EP)

---

## Test Scenario
Verify that the system applies a shipping fee when the cart total is below the free-shipping threshold.

---

## Preconditions
- User logged in
- Cart contains products
- Cart total below €20 threshold

---

## Test Data
Cart total < €20

---

## Steps to Reproduce
1. Add low-priced items to cart
2. Ensure total remains below threshold
3. Open cart/checkout page
4. Observe shipping charge

---

## Expected Result
- Shipping fee applied
- Shipping cost added to order total
- Total amount updated correctly

---

## Actual Result
- Shipping fee displayed
- Order total includes shipping charge
- Calculation correct

---

## Status
PASS

---

## Severity
Low

## Priority
Low

---

## Notes
Shipping logic correctly applies charges for orders below the free-shipping threshold.  
Business rule functions as expected.

---

## Evidence
Screenshot 17

<img width="540" height="767" alt="6  Equivalence Partitioning Shippig cost below 20" src="https://github.com/user-attachments/assets/969fa6dc-00e1-48f4-8499-243ab9040c36" />

---
---

# GroceryMate – Test Execution Report

## Test Case 18 — Shipping Fee Calculation Applied Correctly

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Test Type
Functional Testing

## Test Technique
Equivalence Partitioning (EP)

---

## Test Scenario
Verify that the system correctly applies and calculates the shipping fee when applicable.

---

## Preconditions
- User logged in
- Items added to cart
- Cart total does not qualify for free shipping

---

## Steps to Reproduce
1. Add products to cart
2. Open cart page
3. Observe shipping line item
4. Verify total calculation

---

## Expected Result
- Shipping fee displayed
- Fee added to order total
- Correct calculation shown

---

## Actual Result
- Shipping fee displayed correctly
- Total amount updated accurately
- No discrepancies observed

---

## Status
PASS

---

## Severity
Low

## Priority
Low

---

## Notes
Shipping cost calculation behaves correctly for standard charge scenarios.  
Business rule validated successfully.

---

## Evidence
Screenshot 18

<img width="523" height="616" alt="7  Equivalence Partitioning Shipping fee is applied" src="https://github.com/user-attachments/assets/d585886e-6c80-4c9a-b51d-6774a68f5ac0" />

---
---

# GroceryMate – Test Execution Report

## Test Case 19 — Shipping Rule Applied Correctly at Threshold Value

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Test Type
Functional Testing

## Test Technique
Boundary Value Analysis (BVA)

---

## Test Scenario
Verify that the system applies the correct shipping rule when the cart total equals the free-shipping threshold.

---

## Preconditions
- User logged in
- Cart available
- Free-shipping threshold defined (e.g., €20)

---

## Test Data
Cart total = threshold value

---

## Steps to Reproduce
1. Add items so total equals exactly the threshold amount
2. Open cart/checkout page
3. Observe shipping calculation

---

## Expected Result
- Shipping rule applied exactly as defined by business logic
- Either free or charged correctly per specification
- No miscalculation at boundary

---

## Actual Result
- Shipping rule applied correctly
- Calculation matches expected behavior
- No discrepancy observed

---

## Status
PASS

---

## Severity
Low

## Priority
Low

---

## Notes
System correctly handles the boundary condition without off-by-one or rounding errors.  
Edge case behavior validated successfully.

---

## Evidence
Screenshot 19

<img width="526" height="626" alt="8  BVA - System applies shipping fee rule as defined" src="https://github.com/user-attachments/assets/7a488b11-1cec-4aaa-914f-b1a253949741" />

---
---

# GroceryMate – Test Execution Report

## Test Case 20 — Free Shipping Applied Above Threshold

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Test Type
Functional Testing

## Test Technique
Equivalence Partitioning (EP)

---

## Test Scenario
Verify that the system applies free shipping when the cart total exceeds the free-shipping threshold.

---

## Preconditions
- User logged in
- Free-shipping threshold configured (e.g., €20)

---

## Test Data
Cart total > €20

---

## Steps to Reproduce
1. Add items to cart so total exceeds €20
2. Open cart page
3. Observe shipping charge

---

## Expected Result
- Shipping cost = €0
- Free-shipping message displayed
- Total equals product total only

---

## Actual Result
- Shipping cost is €0
- Total calculated correctly
- Free shipping applied as expected

---

## Status
PASS

---

## Severity
Low

## Priority
Low

---

## Notes
System correctly applies free-shipping rule when order value exceeds threshold.

---

## Evidence
Screenshot 20

<img width="531" height="617" alt="9  EP - Shipping fee zero above threashold value" src="https://github.com/user-attachments/assets/a0c3603b-1e19-4d7d-b76c-5ea29b68a3a8" />

---
---

# GroceryMate – Test Execution Report

## Test Case 21 — Empty Cart Behavior Validation

---

### Test Environment
System: GroceryMate Webshop  
Environment: Staging  

### Test User
Role: Registered User  
Account Type: Test Account  

---

## Test Type
Functional Testing

## Test Technique
Error Guessing (Edge Case)

---

## Test Scenario
Verify that the system behaves correctly when the shopping cart is empty.

---

## Preconditions
- User logged in
- No items added to cart

---

## Steps to Reproduce
1. Open cart page with no products added
2. Observe page behavior

---

## Expected Result
- Message indicating cart is empty
- No shipping cost displayed
- No product totals shown
- No system errors or crashes

---

## Actual Result
- "No items in cart" message displayed
- No shipping charges applied
- No totals calculated
- Page renders correctly

---

## Status
PASS

---

## Severity
Low

## Priority
Low

---

## Notes
System gracefully handles empty cart edge case without calculation or UI issues.  
Proper empty-state UX implemented.

---

## Evidence
Screenshot 21

<img width="882" height="585" alt="10  Error Guessing for empty cart" src="https://github.com/user-attachments/assets/a3c08aca-9a96-475e-ae76-f5d197fb1280" />

# End of report
