# Requirements — GroceryMate Webshop (New Features)

## The Software

GroceryMate is a web-based webshop application with the following existing functionalities:

- Browse product categories
- View product listings and product detail pages
- Add and remove items from the shopping cart
- Proceed to checkout and place orders

---

## New Features

### 1. Product Rating System

#### Vague Requirement

Users should be able to rate products and optionally leave feedback about their experience.

#### Questions

- Who should be allowed to rate products (guest users, logged-in users, or only verified purchasers)?
- How many stars should the rating system support?
- Should users be able to rate the same product more than once?
- Is written feedback optional or mandatory?
- What should happen if the user enters very short or very long feedback?
- Are there any restrictions on content (e.g., profanity, links, scripts)?

#### Detailed Requirement

Logged-in users should be able to rate products using a 5-star rating system with values from 1 to 5.  
The system should allow users to optionally submit written feedback along with the rating.

The system should define whether a user can submit only one rating per product (with the option to edit or delete it) or multiple ratings.  
Written feedback must be validated according to defined minimum and maximum character limits.  
After submission, the rating and feedback should be saved and reflected in the product’s average rating display.

---

### 2. Age Verification for Alcoholic Products

#### Vague Requirement

Users should only be able to access alcoholic products if they are at least 18 years old.

#### Questions

- How should age verification be implemented (Yes/No confirmation, age input, or date of birth)?
- When should the age verification be triggered (category page, product page, or both)?
- What should happen if a user is underage?
- Should the verification persist for the session or longer?
- Can users bypass the restriction by accessing product pages directly via URL?

#### Detailed Requirement

When a user navigates to the alcoholic products category, the system should display an age verification modal before showing any products.  
The user must verify that they are at least 18 years old in order to proceed.

If the user is underage, access to alcoholic products must be blocked and a clear restriction message should be displayed.  
The system should enforce the age restriction not only on category pages but also on direct product URLs and add-to-cart actions.

The duration of verification persistence (session-based, cookie-based, or profile-based) must be clearly defined.

---

### 3. Shipping Cost Changes

#### Vague Requirement

The webshop should support free shipping above a certain order value and apply a shipping fee below that value.

#### Questions

- What is the free-shipping threshold amount?
- Is free shipping applied when the order total is exactly equal to the threshold?
- What shipping fee should be applied below the threshold?
- Should the threshold be calculated before or after discounts?
- Should taxes be included in the threshold calculation?
- How should shipping costs update when cart contents change?

#### Detailed Requirement

The system should define a free-shipping threshold amount.  
Orders with a total value above the defined threshold should receive free shipping, while orders below the threshold should have a shipping fee applied.

The shipping cost should be recalculated dynamically whenever the cart contents change (adding/removing items or updating quantities).  
Shipping costs must be displayed consistently on the cart page, checkout summary, and order confirmation page.

The rules for threshold calculation (discounts, taxes, rounding) must be clearly defined and applied consistently.

---


