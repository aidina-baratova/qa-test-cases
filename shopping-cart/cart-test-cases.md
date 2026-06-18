# Shopping Cart - Test Cases
**Test site:** https://www.saucedemo.com

**Precondition for all tests:** User is logged in as 'standard_user' with password 'secret_sauce' and is on the products page.

---

### TC001 - Add single item to cart

**Steps:**
1. Click Add to cart on any product

**Expected result:** Item is added to cart, button changes to Remove, cart icon displays count of 1

**Status:** Pass

---

### TC002 - Add multiple items to cart

**Steps:**
1. Click Add to cart on first product
2. Click Add to cart on second product
3. Click Add to cart on third product

**Expected result:** Cart icon displays count of 3, all three items show Remove button

**Status:** Pass

--- 

### TC003 - Cannot add same item twice

**Steps:**
1. Click Add to cart on any product
2. Observe the button state

**Expected result:** Button changes to Remove - no option to add the same item a second time

**Status:** Pass

---

### TC004 - Remove item from products page

**Steps:**
1. Click Add to cart on any product
2. Click Remove on the same product

**Expected result:** Item is removed from cart, button changes back to Add to cart, cart icon count decreases by 1

**Status:** Pass

---

### TC005 - View cart contents

**Steps:**
1. Add two items to the cart
2. Click the cart icon in the top right corner

**Expected result:** Cart page displays both added items with correct names and prices

**Status:** Pass

---

### TC006 - Remove item from cart page

**Steps:**
1. Add one item to the cart
2. Click the cart icon to go to the cart page
3. Click Remove next to the item

**Expected result:** Item is removed from cart, cart becomes empty, cart icon shows no count

**Status:** Pass

---

### TC007 - Continue shopping from cart

**Steps:**
1. Add one item to the cart
2. Click the cart icon to go to the cart page
3. Click Continue Shopping

**Expected result:** User is returned to the products page, item remains in the cart

**Status:** Pass

---

### TC008 - Checkout with valid details

**Steps:**
1. Add one item to the cart
2. Click the cart icon
3. Click Checkout
4. Enter first name: Test
5. Enter last name: User
6. Enter zip code: 90001
7. Click Continue
8. Review order summary
9. Click Finish

**Expected result:** Order is completed, confirmation message displayed - "Thank you for your order!"

**Status:** Pass

---

### TC009 - Checkout with empty first name

**Steps:**
1. Add one item to the cart
2. Click the cart icon
3. Click Checkout
4. Leave first name empty
5. Enter last name: User
6. Enter zip code: 90001
7. Click Continue

**Expected result:** Error message displayed — [go to saucedemo and check exact message]

**Status:** Pass

---

### TC010 - Checkout with empty zip code

**Steps:**
1. Add one item to the cart
2. Click the cart icon
3. Click Checkout
4. Enter first name: Test
5. Enter last name: User
6. Leave zip code empty
7. Click Continue

**Expected result:** Error message displayed — [go to saucedemo and check exact message]

**Status:** Pass
