# Automation_Cypress_Test

Test Overview Scenerio..

1) Login -  To ensure that users can successfully log in to the web application.
Steps go - Visit the web application's login page.
Enter a specific email and password.
Click the login button.

After The Login..

2) Add Package -  To verify that a user can manually add a new package with specified FirstName_LastName and dimensions.
Steps go - Navigate to the "Package Types" section (assuming this is the prerequisite step).
Click on the "Add Manually" button.
Provide the name and dimensions of the package.
Create the package.

Logout- To confirm that users can successfully log out of the web application.
Steps go - Click on the logout button. This step ensures that the test environment is in a known state (logged out) before proceeding to the next test case.


# now again the Login -  To ensure that users can successfully log in to the web application. 

3) Delete Package- To validate that a user can delete a recently added package.
Steps go - Log in again (as logging out is a prerequisite).
Locate and select the recently added package.
Delete the selected package.
Separation of Test Cases: This test case is separate from "Add Package" to focus on package deletion functionality.
Explicit Waits: Use cy.wait as needed to ensure elements are ready for interaction.
Hardcoded Values: Maintain the use of hardcoded values for consistency and accuracy.

Design Decisions and Approach:-
a) Separation of Test Cases: The "Add Package" and "Delete Package" actions are seperated into two different test cases.
b) Explicit Waits: cy.wait are introduced for explicit waits between certain actions.
c) Repetition of Login and Logout: log in and log out is done for both test cases,that ensures each test starts with a known state (logged in) and ends in a known state (logged out).


