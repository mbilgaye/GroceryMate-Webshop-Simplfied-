# Test Plan — GroceryMate Webshop Enhancements

---

## 1. Analyze the Product

### Objective
The primary objective of the product is to enhance the existing GroceryMate webshop by introducing new customer-facing features while ensuring that existing core shopping and checkout functionalities continue to work correctly.

### User Base
The product will be used by:
- Guest users browsing products
- Registered and logged-in customers
- Users purchasing both regular and age-restricted (alcoholic) products

The platform is intended for adult users, with age verification enforced for alcoholic products.

### Hardware and Software Specifications

#### Hardware Requirements
- Devices: Desktop PCs, laptops, smartphones, tablets
- Minimum specifications:
  - Desktop/Laptop: 4GB RAM, 2GHz processor
  - Mobile: Standard Android and iOS devices

#### Software Requirements
- Operating Systems: Windows, macOS, Android, iOS
- Browsers: Chrome, Firefox, Safari, Edge
- Dependencies:
  - Backend services
  - Pricing and shipping calculation services
  - Payment and checkout services

### Product Functionality
The product allows users to:
- Browse and search products
- Add and remove items from the basket
- Rate products using a star rating and optional review
- View alcoholic products only after age verification
- Receive dynamic shipping cost calculation based on cart total
- Complete checkout with accurate order totals

---

## 2. Design the Test Strategy

### Scope of Testing

#### In Scope
- Product rating system
- Age verification for alcoholic products
- Shipping cost calculation and threshold logic
- Integration of new features with:
  - Product listing and detail pages
  - Basket and checkout flow
- Negative, boundary, and basic security testing
- UI and usability validation

#### Out of Scope
- Full performance benchmarking
- Penetration testing
- Backend database testing not affecting UI behavior
- Payment gateway certification

### Type of Testing
- Functional Testing
- Integration Testing
- Regression Testing
- Security Testing (basic input and bypass validation)
- Usability Testing

### Risks and Issues

| Risk | Mitigation |
|---|---|
| Undefined business rules (threshold logic, rating eligibility) | Confirm rules with stakeholders before execution |
| Test data unavailability | Prepare mock products and cart configurations |
| Late feature changes | Allocate buffer time for regression testing |

---

## 3. Define Test Objectives

### Objectives
- **Functionality:** Ensure all new features work according to defined requirements.
- **GUI:** Verify correct display of ratings, shipping costs, and age-verification messages.
- **Security:** Prevent underage access and bypass attempts.
- **Usability:** Ensure clear messaging and smooth user experience.

### Expected Outcomes
- Product ratings are submitted, stored, and displayed correctly.
- Alcoholic products are accessible only after successful age verification.
- Shipping costs are calculated and displayed accurately across all screens.
- Existing webshop functionality remains unaffected.

---

## 4. Define Test Criteria

### Suspension Criteria
Testing will be suspended if:
- Critical defects block checkout or pricing calculations
- Underage users can access alcoholic products
- Test environment becomes unavailable

### Exit Criteria
- All planned test cases executed
- At least 95% execution rate achieved
- At least 90% pass rate achieved
- No open critical or high-severity defects
- Regression tests completed successfully
- Stakeholder sign-off obtained

---

## 5. Resource Planning

### Human Resources
- QA Engineer: Test design, execution, defect reporting
- Developers: Defect fixing and technical support
- Product Owner / Stakeholder: Requirement clarification and acceptance

### Hardware
- Desktop and laptop systems
- Mobile devices or emulators

### Software
- Supported browsers and operating systems
- Test management and defect tracking tools

---

## 6. Plan Test Environment

### Test Environments
- Development (DEV)
- Testing / QA (TEST)
- Acceptance (ACC)
- Production (PROD)

Testing will primarily be conducted in the TEST environment using real browsers and devices.

---

## 7. Schedule and Estimation

| Activity | Environment | Responsible | Estimated Effort |
|---|---|---|---|
| Test Planning | All | QA Engineer | 16 hours |
| Test Case Design | All | QA Engineer | 32 hours |
| Integration Testing | TEST | QA Engineer | 24 hours |
| System Testing | TEST | QA Engineer | 40 hours |
| Regression Testing | TEST | QA Engineer | 24 hours |
| UAT Support | ACC | QA / Stakeholders | 20 hours |

---

## 8. Determine Test Deliverables

- Test Plan Document
- Test Cases and Test Checklists
- Test Data
- Defect Reports
- Test Summary Report
- UAT Sign-off Document
