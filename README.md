# ADUser-IDChange

This PowerShell script serves as a user-friendly gateway for multiple departments to access Active Directory functionalities. Designed to streamline user searches and potentially modify user details, this tool accommodates various departments, particularly HR, enabling efficient handling of employee ID and number assignments. By providing an intuitive graphical interface, it empowers users to swiftly search for specific employees based on names, view their details in a structured format, and, if needed, make modifications like updating employee IDs and numbers. This setup aims to optimize HR workflows, granting them direct control over crucial employee information within the Active Directory environment without extensive technical involvement.


User Search: Allows users to search for Active Directory users based on first and last names.
User Details Display: Presents a user-friendly interface displaying user details in a ListView.
User Detail Modification: Provides the functionality to potentially modify user details such as Employee ID and Employee Number.
Key Components:
Find-ADUser Function:

Forms the basis for entering user search criteria (first and last names).
Provides a graphical interface for user input and cancellation options.
Offers the option to display a "No user found" label.
Show-ADUserListView Function:

Generates a graphical interface displaying user details in a ListView format.
Fetches and showcases user data such as User, Employee ID, and E-Number.
Enables potential modification of user details through button interactions.
Set-ADUserDetails Function:

Allows the modification of specific user details like Employee ID and Employee Number.
Locates the user based on CN and updates provided user details.
Search-ADUsers Function:

Facilitates the search for AD users based on provided first and last names.
Constructs filters for searching AD users based on the input criteria.
Get-EmployeeDetails Function:

Offers an interface for entering Employee ID and Employee Number.
Returns entered details or null if the action is canceled.
Main Logic:

Handles user interaction loops for continuous searching until canceled.
Authenticates and establishes connections with Active Directory.
Utilizes various functions to prompt users for input, search AD users, display user details, and potentially modify user information.
Overall Functionality:
Input: Prompts users for first and last names for searching AD users.
Search: Queries Active Directory for users matching the entered criteria.
Display: Presents found user details in a ListView format.
Modification: Provides potential options for modifying user details based on user interactions.
