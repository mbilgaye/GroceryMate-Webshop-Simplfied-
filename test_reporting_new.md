# ⭐ Product Rating System

---

## 📌 Scenario 1: Give Minimum Rating (1 Star)

**User Story:**  
As a user of GroceryMate, I am able to give a product a rating of **1 star**.

---

### Test Steps

| Step # | Action | Expected Outcome | Status | URL | Issue |
|--------|--------|-----------------|--------|------|--------|
| 1 | Go to the login page of GroceryMate | Login page appears | OK | https://grocerymate.masterschool.com/ | |
| 2a | Enter username: `asdf@example.com` | Username accepted | OK | | |
| 2b | Enter password: `AsDfGh` | Password accepted | OK | | |
| 3 | Click **Sign In** | User is successfully logged in and redirected to homepage | OK | | |
| 4 | Click **Shop** button | Navigated to store page | OK | `/store` | |
| 5 | Select **Pears** → Click **Add to Cart** | Message displayed: *Item added to cart* | OK | | |
| 6 | Click cart icon | Navigated to checkout page | OK | `/checkout` | |
| 7a | Enter street: `ABC` | Field accepted | OK | | |
| 7b | Enter city: `Berlin` | Field accepted | OK | | |
| 7c | Enter postal code: `12345` | Field accepted | OK | | |
| 7d | Enter card number: `12345` | Field accepted | OK | | |
| 7e | Enter name on card: `Abc` | Field accepted | OK | | |
| 7f | Enter expiration date: `12/2032` | Field accepted | OK | | |
| 7g | Enter CVV: `123` | Field accepted | OK | | |
| 8 | Click **Buy Now** | Redirected to homepage | OK | | |
| 9 | Click **Shop** button | Redirected to store page | OK | `/store` | |
| 10 | Click **Pears** | Redirected to product page | OK | https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47990 | |
| 11 | Select **1 Star rating** | 1 star is highlighted | OK | | |
| 12 | Click **Send** button | Rating visible & message displayed: *You already reviewed this product* | OK | `/store` | |

---

### 📷 Evidence Screenshot

![Product rated to 1](https://github.com/user-attachments/assets/c94bf50c-5b01-4c2a-9d5a-aa7223c9cdcd)

---

---

## 📌 Scenario 2: Give Maximum Rating (5 Star)

**User Story:**  
As a user of GroceryMate, I am able to give a product a rating of **5 star**.

---

### Test Steps

| Step # | Action | Expected Outcome | Status | URL | Issue |
|--------|--------|-----------------|--------|------|--------|
| 1 | Go to the login page of GroceryMate | Login page appears | OK | https://grocerymate.masterschool.com/ | |
| 2a | Enter username: `asdf@example.com` | Username accepted | OK | | |
| 2b | Enter password: `AsDfGh` | Password accepted | OK | | |
| 3 | Click **Sign In** | User is successfully logged in and redirected to homepage | OK | | |
| 4 | Click **Shop** button | Navigated to store page | OK | `/store` | |
| 5 | Select **Nectarines** → Click **Add to Cart** | Message displayed: *Item added to cart* | OK | | |
| 6 | Click cart icon | Navigated to checkout page | OK | `/checkout` | |
| 7a | Enter street: `ABC` | Field accepted | OK | | |
| 7b | Enter city: `Berlin` | Field accepted | OK | | |
| 7c | Enter postal code: `12345` | Field accepted | OK | | |
| 7d | Enter card number: `12345` | Field accepted | OK | | |
| 7e | Enter name on card: `Abc` | Field accepted | OK | | |
| 7f | Enter expiration date: `12/2032` | Field accepted | OK | | |
| 7g | Enter CVV: `123` | Field accepted | OK | | |
| 8 | Click **Buy Now** | Redirected to homepage | OK | | |
| 9 | Click **Shop** button | Redirected to store page | OK | `/store` | |
| 10 | Click **Nectarines** | Redirected to product page | OK | https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47990 | |
| 11 | Select **5 Star rating** | 5 star is highlighted | OK | | |
| 12 | Click **Send** button | Rating visible & message displayed: *You already reviewed this product* | OK | `/store` | |

---

### 📷 Evidence Screenshot

---<img width="777" height="907" alt="1  Boundry Value Rating 5" src="https://github.com/user-attachments/assets/378b080a-e590-4991-aeaf-85bf07dc603e" />

---
---

## 📌 Scenario 3: Verify valid rating submission by logged-in user
**User Story:**  
As a user of GroceryMate, I am able to give a product a rating **between 1 to 5 star**.

---

### Test Steps

| Step # | Action | Expected Outcome | Status | URL | Issue |
|--------|--------|-----------------|--------|------|--------|
| 1 | Go to the login page of GroceryMate | Login page appears | OK | https://grocerymate.masterschool.com/ | |
| 2a | Enter username: `asdf@example.com` | Username accepted | OK | | |
| 2b | Enter password: `AsDfGh` | Password accepted | OK | | |
| 3 | Click **Sign In** | User is successfully logged in and redirected to homepage | OK | | |
| 4 | Click **Shop** button | Navigated to store page | OK | `/store` | |
| 5 | Select **Oranges** → Click **Add to Cart** | Message displayed: *Item added to cart* | OK | | |
| 6 | Click cart icon | Navigated to checkout page | OK | `/checkout` | |
| 7a | Enter street: `ABC` | Field accepted | OK | | |
| 7b | Enter city: `Berlin` | Field accepted | OK | | |
| 7c | Enter postal code: `12345` | Field accepted | OK | | |
| 7d | Enter card number: `12345` | Field accepted | OK | | |
| 7e | Enter name on card: `Abc` | Field accepted | OK | | |
| 7f | Enter expiration date: `12/2032` | Field accepted | OK | | |
| 7g | Enter CVV: `123` | Field accepted | OK | | |
| 8 | Click **Buy Now** | Redirected to homepage | OK | | |
| 9 | Click **Shop** button | Redirected to store page | OK | `/store` | |
| 10 | Click **Oranges** | Redirected to product page | OK | https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47990 | |
| 11 | Select **3 Star rating** | 5 star is highlighted | OK | | |
| 12 | Click **Send** button | Rating visible & message displayed: *You already reviewed this product* | OK | `/store` | |

---

### 📷 Evidence Screenshot
<img width="392" height="907" alt="3  Equivalance Partitioning Rating 4" src="https://github.com/user-attachments/assets/30c0ec04-b259-4f72-b9e4-83bc2eade8cc" />

---
---

## 📌 Scenario 4: Submit Review with Text

**User Story:**  
As a user of GroceryMate, I am able to give a product a **1 star rating with a short review text**.

---

### Test Steps

| Step # | Action | Expected Outcome | Status | URL | Issue |
|--------|--------|-----------------|--------|------|--------|
| 1 | Go to the login page of GroceryMate | Login page appears | OK | https://grocerymate.masterschool.com/ | |
| 2a | Enter username: `asdf@example.com` | Username accepted | OK | | |
| 2b | Enter password: `AsDfGh` | Password accepted | OK | | |
| 3 | Click **Sign In** | User successfully logged in | OK | | |
| 4 | Click **Shop** button | Navigated to store page | OK | `/store` | |
| 5 | Select **Lemon Loaf Cake** → Click **Add to Cart** | Message displayed: *Item added to cart* | OK | | |
| 6 | Click cart icon | Navigated to checkout page | OK | `/checkout` | |
| 7a | Enter street: `ABC` | Field accepted | OK | | |
| 7b | Enter city: `Berlin` | Field accepted | OK | | |
| 7c | Enter postal code: `12345` | Field accepted | OK | | |
| 7d | Enter card number: `12345` | Field accepted | OK | | |
| 7e | Enter name on card: `Abc` | Field accepted | OK | | |
| 7f | Enter expiration date: `12/2032` | Field accepted | OK | | |
| 7g | Enter CVV: `123` | Field accepted | OK | | |
| 8 | Click **Buy Now** | Redirected to homepage | OK | | |
| 9 | Click **Shop** button | Redirected to store page | OK | `/store` | |
| 10 | Click **Lemon Loaf Cake** | Redirected to product page | OK | https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb479f9 | |
| 11 | Select **1 Star rating** | 1 star is highlighted | OK | | |
| 12 | Write comment: `Between good and bad` | Comment text entered successfully | OK | | |
| 13 | Click **Send** button | Rating and review displayed successfully | OK | `/store` | |

---
