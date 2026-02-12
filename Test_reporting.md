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
