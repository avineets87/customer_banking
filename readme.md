# Customer Banking

## Overview
Creating a customer banking system that allows users to calculate and track interest earned on savings and CD accounts. By running this application, users will be able to enter their savings and CD account information, see the interest earned, and view the updated balances after a specified number of months.

### Sample Output

``` text
(dev) (base) avineetsharma@Avineets-MacBook-Air customer_banking % conda activate dev
(dev) (dev) avineetsharma@Avineets-MacBook-Air customer_banking % python customer_banking.py 
Hey User, please enter your savings balance: 10000
Hey User, please enter your savings interest rate: 5
Hey User, please enter the savings maturity duration in months: 24
Okay! Here is your interest earned in your saving account 1,000.00 and updated savings account balance 11,000.00
Hey User, please enter your cd balance: 10000
Hey User, please enter your cd interest rate: 10
Hey User, please enter the cd maturity duration in months: 24
Alright! Here is your interest earned in your CD account 2,000.00 and updated savings account balance 12,000.00
```

### Implementation Details

#### Create the Savings Account Function

Open the `savings_account.py` file, and do the following:

1.  Imports the `Account` class from the `Accounts.py` file.
    
2.  In the `create_savings_account` function do the following:
    
    -   Create an instance of the `Account` class and pass in the balance and interest parameters.
        
    -   Calculate interest earned.
  
        
    -   Update the savings account balance by adding the interest earned.
        

        
    -   Pass the updated balance to the set balance method using the instance of the `Account` class.
        
    -   Pass the interest earned to the set interest method using the instance of the `Account` class.
        
    -   Return the updated balance and interest earned.
        

#### Create the CD Account Function

Open the `cd_account.py` file, and do the following:

1.  Import the `Account` class from the `Accounts.py` file.
    
2.  In the `create_cd_account` function, do the following:
    
    -   Create an instance of the `Account` class and pass in the parameters.
        
    -   Calculate interest earned.
        
    -   Update the savings account balance by adding the interest earned.
        
    -   Pass the updated balance to the set balance method using the instance of the `Account` class.
        
    -   Pass the interest earned to the set interest method using the instance of the `Account` class.
        
    -   Return the updated balance and interest earned.
        

#### Create the Main Function

Open the `customer_banking.py` file, and do the following:

1.  Import the `create_cd_account` and `create_savings_account` functions from the appropriate files.
    
2.  In the `main` function, do the following:
    
    -   Prompt the user to set the savings balance, interest rate, and months for the savings account.
       
        
    -   Call the `create_savings_account` function and pass in the variables from the user.
        
    -   Print out the interest earned and updated savings account balance with interest earned for the given months.
        
    -   Prompt the user to set the CD balance, interest rate, and months for the CD account.
        
    -   Call the `create_cd_account` function and pass the variables to the function used to prompt the user from the user.
        
    -   Print out the interest earned and updated CD account balance with interest earned for the given months.
        
    -   Call the main function.
