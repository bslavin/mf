# Introduction

MyFuture builds a financial picture for your specific retirement based on your current and future circumstances. MyFuture gives you the tools to model your financial picture in an ever changing economy. Knowing when you can retire with a lifestyle you can afford is now possible with MyFuture. Version 1.x is a prototype. Version 2.x will not use Excel, but will execute on Windows, Mac and Linux.

## Simple Financial Model
MyFuture is a Microsoft Excel spreadsheet program that uses Excel’s extensive library of tools. A MyFuture user needs to define their financial world, describing income, expenses, investments and debt. With these inputs, the program will generate your future financial picture.

## Inputs
“MyWorld”, an Excel sheet, describes all the current and future financial events in your lifetime. 

There are two sections to MyWorld

### Defined Dates

Defined dates are used to simplify entering your current and future financial circumstances. There are significant dates in your financial landscape including such dates as when you retire, when you turn 65 or 70 and when you pass away. These significant dates are defined in this section of MyWorld.
### Description Types

There are four description types in MyWorld. These description types provide you the necessary elements to completely describe your current and future financial situation.

- Income Income entries describe income from such things as jobs, investments, and Social Security
- Expenses Expense entries describe ongoing, short term and onetime expenses. Expenses entries describe such things as food, clothing, heath care, tuition, and home repairs. Debt expenses are not included in this entry.
- Investments Investment entries describe your investments ranging from savings accounts, 401Ks, and real estate.
- Debt Debt entries describe your debt ranging from credit card, mortgages and term loans.

## Outputs
MyFuture produces two outputs. “MyForecast Summary” shows you a year by year summary of your income, expenses, net cash flow, investments, debts and net worth. “MyForecast Details” shows details the details of each entry in MyWorld by year with a more detailed summary than MyForecast Summary.

## Program Execution
To start MyFuture, type “Shift” + “Ctrl” + “M”. The program will begin execution and provide status updates in the Excel Status Bar. During the processing, the program will not update the screen except at the Excel Status Bar. 

Not all versions of Excel have been tested and at least one version does not show the update in the Status Bar even though the processing is taking place. Processing can take from a few seconds to up to one minute. MyFuture outputs both warning and error messages. MyFuture will continue processing after a warning message, but will stop processing after an error message.

MyFuture is an Excel Macro written in VBA. For security reasons, Excel will more than likely block execution of the macro in MyFuture. Excel macros can have hidden viruses that can damage your computer. MyFuture is not dangerous to your computer. Excel should give you the option to enable the macro in MyFuture. Do not enable all macros; just enable the macro MyFuture.

## Sheet MyWorld
Defined Dates Defined Dates must be in columns A and B. Entries must start in row 2. Column A is used for your user friendly definitions. Your user friendly definitions help building the Description types more intuitive. Defined dates should start with a letter and can be anything but “Description” as this is a reserved word. Column B is used for the Actual Date and should be in the format of mm/dd/yyyy. Typical dates that are significant to your financial model are
- Start date
- Birth of a child
- A child entering college
- Retirement
- The beginning of Social Security
- Medicate start date
- IRA mandatory contribution date
- Estimate date of your death and death of your spouse

## Description Types
There are four description types in MyWorld. These description types provide you the necessary elements to completely describe your current financial situation. They also provide you the means to create a model for your future. The description types may be fully described in a single entry or in multiple entries. For example, salary for a job could be described in a single entry with a specific start date, end date, amount and percent change. The description of a stock portfolio could be described with multiple entries since you might change at retirement from putting money into the stock portfolio to removing money from the stock portfolio. This change is best modeled using multiple entries. There are examples of single and multiple entry types MyFuture.

## Income 

Income entries describe income from such things as jobs and Social Security. Each column of the entry is described below.


- Description – This is a short description. For multiple entries, the short description must be identical for each entry.
- Type – This must be “Income”.
- Start – This is the start date. If the start date is not a Defined Date, the value must
be January 1st of a year in the format “1/1/yyyy.” If the start date is a Defined Date, the program will shift the date to the nearest January 1st. If the start date is a second entry or beyond of a multiple entry description, the start date must be the exact end date of the previous entry or one day afterwards.
- End–Thisistheenddate.IftheenddateisnotaDefinedDate,thevaluemustbe December 31st of a year in the format “12/31/yyyy.” If the end date is a Defined Date, the program will shift the date to the nearest December 31st.
- Amount – This is that yearly amount of the income. This should be a positive whole number.
- % Change – This is the percent increase or decrease of the amount. For example, you might have a positive percent change if you expect steady increases in salary. On the other hand, if you work hourly, and expect to cut back your hours over a many years, you might have a negative percent change. This should be a percentage from -99.99% to 99.99%.
- Investment Withdrawal ($) – This is only used for type Investment. o Investment Withdrawal (%) – This is only used for type Investment. o Investment Contribution ($) – This is only used for type Investment. o Debt Pay Down ($) – This is only used for type Debt.
- Investment Growth Tax – This is only used for type Investment.
- Investment Withdrawal Tax – This is only used for type Investment.
- Income Tax – This is the percent of income tax you expect to pay on this income
entry. This can be left blank if the income is not taxed or it should be a percentage from 0.01% to 99.99%.

## Expenses 

Expense entries describe ongoing, short term and onetime expenses. Expenses entries describe such things as food, clothing, heath care, tuition, and home repairs. Debt expenses are not included in this entry.
- Description – Same as “Income.”
- Type – This must be “Expense.”
- Start – Same as “Income.”
- End – Same as “Income.”
- Amount – This is that yearly amount of the expense. This should be a positive whole
number.
- % Change – This is the percent increase or decrease of the amount. This is where
you account for inflation of the specific types of expenses. This is also where you can account for a change in your spending habits. For example, you might cut back or increase vacation expenses when you retire. This should be a percentage from - 99.99% to 99.99%.
- Investment Withdrawal ($) – This is only used for type Investment. o Investment Withdrawal (%) – This is only used for type Investment.

- Investment Contribution ($) – This is only used for type Investment. o Debt Pay Down ($) – This is only used for type Debt.
- Investment Growth Tax – This is only used for type Investment.
- Investment Withdrawal Tax – This is only used for type Investment. o Income Tax – This is only used for type Income.

## Investments 

Investment entries describe your investments ranging from savings accounts, 401Ks, and real estate.

- Description – Same as “Income.”
- Type – This must be “Investment.”
- Start – Same as “Income.”
- End – Same as “Income.”
- Amount – This is the current value of the investment. This should be a positive
whole number.
- % Change – This is the percent increase or decrease of the investment for the year.
The percent change does not include any contributions you make during the year or any distributions you take during the year. This percent change is only for the growth or decline in value of the investment you expect for the year. This should be a percentage from -99.99% to 99.99%.
- Investment Withdrawal ($) – This is the yearly amount, in dollars, you want to use for cash flow during the year. It is not required to set this value, but if you want to use some of the investment for cash flow, you can either use this dollar amount or the percent amount described below. You cannot use both. This money can be taxed by filling in either Investment Growth Tax or Investment Withdrawal Tax. MyForecast Detail shows this as income. This should be a positive whole number.
- Investment Withdrawal (%) – This is the yearly amount, in percent of current amount, you want to use for cash flow during the year. It is not required to set this value, but if you want to use some of the investment for cash flow, you can either use this percent amount or the dollar amount described above. You cannot use both. This money can be taxed by filling in either Investment Growth Tax or Investment Withdrawal Tax. MyForecast Detail shows this as income. This should be a percentage from -99.99% to 99.99%.
- Investment Contribution ($) – This is the yearly amount, in dollars, that you want to put into this investment. MyForecast Detail shows the contribution as an expense. This should be a positive whole number. The program calculates the growth on the investment before adding in this contribution.
-  Debt Pay Down ($) – This is only used for type Debt.
- Investment Growth Tax – This is the tax rate for growth of the investment as in a
simple savings account. This can be left blank if the growth is not taxed or it should
be a percentage from 0.01% to 99.99%.
-  Investment Withdrawal Tax – This is the tax rate for a withdrawal of the investment
as in an IRA. This can be left blank if the withdrawal is not taxed or it should be a
percentage from 0.01% to 99.99%.
-  Income Tax – This is only used for type Income.


## Debt Debt entries describe your debt ranging from credit card, mortgages and term loans.
- Description – Same as “Income.” o Type – This must be “Debt.”
- Start – Same as “Income.”
- End – Same as “Income.”
- Amount – This is the current amount of the debt. This should be a positive whole number.
- % Change – This is the interest rate of the debt. This should be a percentage from 0.01% to 99.99%.
- Investment Withdrawal ($) – This is only used for type Investment.
- Investment Withdrawal (%) – This is only used for type Investment.
- Investment Contribution ($) – This is only used for type Investment.
- Debt Pay Down ($) – This is the yearly amount, in dollars, you want to use for debt
pay down during the year. It is not required to set this value, but the debt will grow forever unless you do set a pay down amount greater than the amount the debt grows from interest charges. Debt Pay Down should be a positive number.
- Investment Growth Tax – This is only used for type Investment.
- Investment Withdrawal Tax – This is only used for type Investment. o Income Tax – This is only used for type Income.

## Sheet MyForecast Summary
The summary sheet shows you what your model in MyWorld produces for each year. The columns are taken from MyForecast Detail. See the MyForecast Detail description for what each column represents. Negative numbers, shown as red numbers in parenthesis, should be understood and analyzed by looking into MyForecast Detail.
Though some negative numbers in Net Cash Flow are reasonable, too large of negatives indicate a model that does not produce long term financial stability. Cumulative Net Cash Flow sums up the current and past cash flows. If this column goes negative, it shows that the previous positive cash flows are not sufficient to offset the current negative cash flow.

If there are years of positive Net Cash Flow numbers before some negatives and if the sum of the positives are greater than the sum of the negatives, this can be a viable financial future assuming the positives are saved to be used for the years of negatives. If, however, the past positives don’t cover the future negatives, the model is not showing a viable financial future.

As with Net Cash Flow, some negative numbers in Net Worth might be reasonable, too large of negatives indicate a model that does not produce long term financial stability. Large positive numbers in Net Cash Flow might be reasonable, but too many large positive numbers would suggest that some cash flow should be moved to an investment via Investment Contribution in MyWorld.


## Sheet MyForecast Detail
This sheet shows all the details of your MyWorld model. Columns A and B show a summary of the details. Below is an example of a single year’s summary entry.