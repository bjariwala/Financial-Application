## Save the qualifying loans as a new CSV file

## Software that can prompt the user to save the qualifying loans as a new CSV file. As a user, I need the ability to save the qualifying loans to a CSV file so that I can share the results as a spreadsheet.
---

Create new features and enhancements for a loan qualifier application. Specifically, you'll do the following:

- Create a GitHub repository.
- Translate new business requirements to code for adding a function to save loans.
- Organize your code for the changes to the fileio module.
- Update the CLI to add additional dialogs for loan output.
- Write new tests for the functionality to save loans.
- Update the documentation to reflect your new functions and operations.

##Instructions

- Create the Project Repository
- Software Requirements: Translate Business Requirements to Code
- System Design: Organize Your Code
- Usability: Update the CLI
- Testing and Debugging: Write New Tests
- Documentation: Update All of the Docs


## Create the Project Repository
In this section, you'll create the GitHub repository for your project. Use the starter code provided to initialize your repository. Don't forget the README.md! You'll need to update this as you develop your code.

- Create a new GitHub repository.
- Add your README.md file and .gitignore.
- Commit your project files.

## Software Requirements: Translate Business Requirements to Code
- In this section, you'll translate the high-level business requirements into functional code.
- In app.py, write a function named save_csv() that uses the csv library to save the qualifying data as a file.

## Systems Design: Organize Your Code
Now that you have the save_csv() code working, the next step is to refine the systems design.
- Integrate your new save_csv() function into the existing loan qualifier application.
- Update the function and module docstrings for the new feature.

## Usability: Update the CLI
To improve the usability for the not-so-technical users, so that they can access and save their qualifying loans to a CSV. You'll need to add a new save dialog to the existing CLI, by completing the following steps:
- In app.py, create a new function named save_qualifying_loans() that accepts the list of qualifying loans.
- Inside the new save_qualifying_loans() function, create the user dialog to prompt the user for whether or not they would like to save their qualifying loans. Use Questionary to prompt the user with .confirm().ask().
- Inside the save_qualifying_loans() function, create the user dialog for the save CSV function. Use Questionary to prompt the user and ask for the output file path.

## Test and Debug: Write New Tests

- Create a new test called test_save_csv to ensure that the fileio code can successfully write to a CSV file at a particular path.

## Extension
Add test_filters to test that your filters properly remove institutions that specific input should eliminate. Try to test each individual filter!

---
## Contributors
Presented by Bina Jariwala 

---
## License
none

---
