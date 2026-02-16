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

## 📌 Scenario 4: Give Out of Range Rating (0 & 6 (Below 0 & above 5) Star)

**User Story:**  
As a user of GroceryMate, I am able not able to give a product rating which is out of the range **1 to 5 star**.

---

### Test Steps

| Step # | Action | Expected Outcome | Status | URL | Issue |
|--------|--------|-----------------|--------|------|--------|
| 1 | Go to the login page of GroceryMate | Login page appears | OK | https://grocerymate.masterschool.com/ | |
| 2a | Enter username: `asdf@example.com` | Username accepted | OK | | |
| 2b | Enter password: `AsDfGh` | Password accepted | OK | | |
| 3 | Click **Sign In** | User is successfully logged in and redirected to homepage | OK | | |
| 4 | Click **Shop** button | Navigated to store page | OK | `/store` | |
| 5 | Select **Fresh Vegetables** → Click **Add to Cart** | Message displayed: *Item added to cart* | OK | | |
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
| 10 | Click **Fresh Vegetables** | Redirected to product page | OK | https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47990 | |
| 11 | Select **0 Star rating** | 1 star is highlighted | OK | | |
| 12 | Click **Send** button | Invalid input for the filed 'Rating'. Please check the input | OK | `/store` | |

---

### 📷 Evidence Screenshot

![4  Error Guessing With Rating Zero](https://github.com/user-attachments/assets/a2acf3fc-9d22-40e6-b417-13aed1a5ff18)


---
---
## 📌 Scenario 5: Submit Review with Text

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
### Evidence Screenshot
<img width="391" height="906" alt="2  Boundry Value Rating 1" src="https://github.com/user-attachments/assets/f0e6e007-ed5c-4dd3-8193-c0fe35b527fa" />

---
--- 


## 📌 Scenario 6: Verify Written Feedback Exceeding Maximum Character Limit of 500 Character

**User Story:**  
As a user of GroceryMate, I am **not able to write feedback exceeding 500 character limit**.

---

### Test Steps

| Step # | Action | Expected Outcome | Status | URL | Issue |
|--------|--------|-----------------|--------|------|--------|
| 1 | Go to the login page of GroceryMate | Login page appears | OK | https://grocerymate.masterschool.com/ | |
| 2a | Enter username: `asdf@example.com` | Username accepted | OK | | |
| 2b | Enter password: `AsDfGh` | Password accepted | OK | | |
| 3 | Click **Sign In** | User successfully logged in | OK | | |
| 4 | Click **Shop** button | Navigated to store page | OK | `/store` | |
| 5 | Select **Sotma Strawberry & Lime Cider** → Click **Add to Cart** | Message displayed: *Item added to cart* | OK | | |
| 6 | Click cart icon | Navigated to checkout page | OK | `/checkout` | |
| 7a | Enter street: `ABC` | Field accepted | OK | | |
| 7b | Enter city: `Berlin` | Field accepted | OK | | |
| 7c | Enter postal code: `12345` | Field accepted | OK | | |
| 7d | Enter card number: `12345` | Field accepted | OK | | |
| 7e | Enter name on card: `Abc` | Field accepted | OK | | |
| 7f | Enter expiration date: `12/2032` | Field accepted | OK | | |
| 7g | Enter CVV: `123` | Field accepted | OK | | |
| 8 | Click **Rating heart symbol** | Message displayed **Item added to favourite** | OK | | |
| 9 | Click **Favourite Icon** button | Redirected to store page | OK | `/store/fav` | |
| 10 | Click **Sotma Strawberry & Lime Cider** | Redirected to product page | OK | (https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47a7b)| |
| 11 | Select **Add a comment** | Write a comment | OK | | |
| 12 | Write comment: `Enter text exceeding 500 characters` | Comment text rejected | OK | | |

---
### 📷 Evidence Screenshot

<img width="772" height="962" alt="3  Rating text not allowed above 500 characters" src="https://github.com/user-attachments/assets/b78820f3-695d-4cba-9f00-9dbf31571143" />

---
---


## 📌 Scenario 7: Verify Age Verification prompt when accessing alcohol strategy
**User Story:**  
As a user of GroceryMate, **the website is generating age verification prompt whn accessing alcohol atrategy**.

---

### Test Steps

| Step # | Action | Expected Outcome | Status | URL | Issue |
|--------|--------|-----------------|--------|------|--------|
| 1 | Go to the login page of GroceryMate | Login page appears | OK | https://grocerymate.masterschool.com/ | |
| 2a | Enter username: `asdf@example.com` | Username accepted | OK | | |
| 2b | Enter password: `AsDfGh` | Password accepted | OK | | |
| 3 | Click **Sign In** | User successfully logged in | OK | | |
| 4 | Age verification prompt appears |  | OK |Entered age 16-02-2008 | Age is exactly 18 years |
| 5 | Click **Submit** | Age is accepted | OK | | |
| 6 | Click **Sign In** | User successfully logged in | OK | | |
| 7 | Click **Shop** button | Navigated to store page | OK | `/store` | |
| 8 | Select **Sotma Strawberry & Lime Cider** → Click **Add to Cart** | Message displayed: *Item added to cart* | OK | | |
| 9 | Click cart icon | Navigated to checkout page | OK | `/checkout` | |
| 10a | Enter street: `ABC` | Field accepted | OK | | |
| 10b | Enter city: `Berlin` | Field accepted | OK | | |
| 10c | Enter postal code: `12345` | Field accepted | OK | | |
| 10d | Enter card number: `12345` | Field accepted | OK | | |
| 10e | Enter name on card: `Abc` | Field accepted | OK | | |
| 10f | Enter expiration date: `12/2032` | Field accepted | OK | | |
| 10g | Enter CVV: `123` | Field accepted | OK | | |
| 8 | Click **Buy Now** | Redirected to homepage | OK | | |

---
### Evidence Screenshot
<img width="1460" height="592" alt="3  Age entered to 18 years" src="https://github.com/user-attachments/assets/4026d372-acd3-46bd-83e5-2fd35e3ca4ce" />

---
---

## 📌 Scenario 8: Verify access grant at minimum allowed age (= 18) 
**User Story:**  
As a user of GroceryMate, **the website is allowing purchase of alochom at exactly age = 18**.

---

### Test Steps

| Step # | Action | Expected Outcome | Status | URL | Issue |
|--------|--------|-----------------|--------|------|--------|
| 1 | Go to the login page of GroceryMate | Login page appears | OK | https://grocerymate.masterschool.com/ | |
| 2a | Enter username: `asdf@example.com` | Username accepted | OK | | |
| 2b | Enter password: `AsDfGh` | Password accepted | OK | | |
| 3 | Click **Sign In** | User successfully logged in | OK | | |
| 4 | Age verification prompt appears |  | OK |Entered age 16-02-2008 | Age is exactly 18 years |
| 5 | Click **Sign In** | User successfully logged in | OK | | |

---
### Evidence Screenshot
<img width="1460" height="592" alt="3  Age entered to 18 years" src="https://github.com/user-attachments/assets/4026d372-acd3-46bd-83e5-2fd35e3ca4ce" />

---
---


## 📌 Scenario 9: Verify access for users above mimimum age (> 18)
**User Story:**  
As a user of GroceryMate, **the website is allowing purchase of alochom above minimum age > 18**.

---

### Test Steps

| Step # | Action | Expected Outcome | Status | URL | Issue |
|--------|--------|-----------------|--------|------|--------|
| 1 | Go to the login page of GroceryMate | Login page appears | OK | https://grocerymate.masterschool.com/ | |
| 2a | Enter username: `asdf@example.com` | Username accepted | OK | | |
| 2b | Enter password: `AsDfGh` | Password accepted | OK | | |
| 3 | Click **Sign In** | User successfully logged in | OK | | |
| 4 | Age verification prompt appears |  | OK |Entered age 16-02-2008 | Age is exactly 18 years |
| 5 | Click **Sign In** | User successfully logged in | OK | | |

---
### Evidence Screenshot
<img width="1460" height="592" alt="3  Age entered to 18 years" src="https://github.com/user-attachments/assets/4026d372-acd3-46bd-83e5-2fd35e3ca4ce" />

---
---


