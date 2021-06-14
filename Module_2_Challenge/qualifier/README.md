# BizOPs Application

Creating new features and enhancement for loan qualifier application. The programm will have the ability to allow a user to save the qualifiying loans to a CSV file so that the results can be shared as a spreadsheet.

---

## Technologies

This project uses python 3.8 with the following packages:

* [sys](https://docs.python.org/3/library/sys.html) - It allows operating on the interpreter as it provides access to variables and functions.
* [fire](https://github.com/google/python-fire) - A simple way to create a CLI in python.
* [questionary](https://pypi.org/project/questionary/) - An interactive interface for user prompts and dialogs

---

## Installation Guide

Before running this application first install the following dependencies.
```python
    pip install fire
    pip install questionary
```
---

## Examples

This prompts the user for loan application information.

``` python
python app.py --credit_score --debt --income --loan_amount --home_value
```
---

## Usage

Example code for applicant's financial information.
``` python
    def get_applicant_info():
    """Prompt dialog to get the applicant's financial information.

    Returns:
        Returns the applicant's financial information.
    """

    credit_score = questionary.text("What's your credit score?").ask()
    debt = questionary.text("What's your current amount of monthly debt?").ask()
    income = questionary.text("What's your total monthly income?").ask()
    loan_amount = questionary.text("What's your desired loan amount?").ask()
    home_value = questionary.text("What's your home value?").ask()

    credit_score = int(credit_score)
    debt = float(debt)
    income = float(income)
    loan_amount = float(loan_amount)
    home_value = float(home_value)

    return credit_score, debt, income, loan_amount, home_value
```

---

## Contributors

Presented by Bina Jariwala

---

## License

none