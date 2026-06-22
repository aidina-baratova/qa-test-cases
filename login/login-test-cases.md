Login Feature - Test Cases
TC001 - Valid login
Precondition: User is on the saucedemo.com login page

Steps:

Enter valid username: standard_user
Enter valid password: secret_sauce
Click the Login button
Expected result: User is redirected to the products page

Status: Pass

TC002 - Invalid password
Precondition: User is on the login page

Steps:

Enter valid username: standard_user
Enter incorrect password: wrongpassword
Click the Login button
Expected result: Error message displayed - "Username and password do not match any user in this service"

Status: Pass

TC003 - Invalid username
Precondition: User is on the login page

Steps:

Enter invalid username: wrongusername
Enter valid password: secret_sauce
Click the Login button
Expected result: Error message displayed - "Username and password do not match any user in this service"

Status: Pass

TC004 - Both fields empty
Precondition: User is on the login page

Steps:

Leave username field empty
Leave password field empty
Click the Login button
Expected result: Error message displayed - "Username is required"

Status: Pass

TC005 - Username empty, password filled
Precondition: User is on the login page

Steps:

Leave username field empty
Enter valid password: secret_sauce
Click the Login button
Expected result: Error message displayed - "Username is required"

Status: Pass

TC006 - Username filled, password empty
Precondition: User is on the login page

Steps:

Enter valid username: standard_user
Leave password field empty
Click the Login button
Expected result: Error message displayed - "Password is required"

Status: Pass

TC007 - Locked out user
Precondition: User is on the login page

Steps:

Enter locked out username: locked_out_user
Enter valid password: secret_sauce
Click the Login button
Expected result: Error message displayed - "Sorry, this user has been locked out"

Status: Pass

TC008 - Login with extra spaces in username
Precondition: User is on the login page

Steps:

Enter username with spaces at the end: standard_user
Enter valid password: secret_sauce
Click the Login button
Expected result: Error message displayed - "Username and password do not match any user in this service"

Status: Pass

TC009 - Password field masking
Precondition: User is on the login page

Steps:

Click on the password field
Type any password: secret_sauce
Observe the characters as they are entered
Expected result: Password characters are masked and displayed as dots - plain text is not visible

Status: Pass

TC010 - Successful logout after login
Precondition: User is on the login page

Steps:

Enter valid username: standard_user
Enter valid password: secret_sauce
Click the Login button
Click the menu icon (three horizontal lines) in the top left corner
Click the Logout button
Expected result: User is logged out and redirected back to the login page

Status: Pass
