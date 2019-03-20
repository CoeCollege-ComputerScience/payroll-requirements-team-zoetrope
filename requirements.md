
# General Requirements
* The user can view information about the current pay period.
* The user can request a report to be generated for the current pay period.
* The system can handle an arbitrary amount of employees (dynamically allocated memory).
* The system can receive correctly formatted documents and translate that to payroll information.
* Users can input employee information directly into the system manually.
* Users can type employees' information by keyboard.
* System will support English for the first release.
* System can handle arbitrary amount of money when input.
* System can handle an arbitrary amount of users.
* There are three general types of users: admins, departmental head, and employees.
* The system complies with all federal U.S. business laws.
* The system complies with all state business laws.
* The System complies with all international business laws.

# Payment information
* User can request payment in check or direct deposit.
* As a user, I can be paid either hourly or salaried.
* The system uses U.S. currency.
* Hourly workers will clock in and out according to a set schedule, and the system will calculate their pay according to their actual work times.
* Employees can request changes to their set schedule.
* Employees are not paid during regular time off (e.g. sick days), but they are paid during Paid Time Off.
* Employees are able to request an advance on pay. Admins must approve.
* Schedule changes need approval of managers.
* The system will calculate overtime pay for hourly workers, including weekend pay.
* Weekend pay is 1.5x pay, overtime is 1.5x pay, and weekend overtime is 2x pay.
* Managers can suspend employees.
* Suspended employees receive no payment.
* System can calculate and deduct taxes.
* Management can add bonuses into employee pay.
* Payers can be company account, employees account, customer account, the bank account of departments
* Payee can be company account, employees account, customer account, the bank account of departments

# Screens – what screens are needed (we don't need to put these in our final list, since GUI specification is beyond the perview of this assignment)
* Login: Login based on access rights (watch one's own, watch everyone or can edit/add data)
* Home(for managers ?): showing a list of employees and their basic payroll information
* Past employees' data (if needed)
* Show: showing individual status in detail
* Add: Add employees' data (admin only)
* Edit: Edit or Update employees' data (admin only)
* User interface has a blue and grey color scheme.
* Business-themed interface

# Admin user requirements
* Admin users can set system user types (change an account from employee to admin and vice versa)
* Admin users can search for employees by:
  * name
  * id
  * hire date
* Admin users can edit employee information
* Admin users can remove employees from the system
* Admin users can add employees to the system, with the following information:
  * name
  * address
  * id
  * resident status (U.S. citizen, J1 visa, etc.)
  * position and department
  * hire date
  * salary/hourly wage
  * payment type (hourly vs salary)
  * if hourly:
    * set schedule
  * payment schedule (weekly, biweekly, monthly)
* Admin users can request employee reports (see employee report requests)
* admin users can request company reports
  * company reports calculate total employee payments
* Admin users can request departmental report
  * departmental reports calculate the employee payments for a given department

# Department head user requirements
* department head users can request personal payment reports
* department head users can request departmental payment reports

# regular employee user requirements
* employee user can change personal information
  * address
  * payment method (direct deposit vs. check)
  * etc.
* employee users can request a report of their own payment:
  * can request a history of past payments
  * can request a report of current pay period

# Login & Registration
* System can handle first-time users
  * System prompts user to enter company email or id
  * system prompts user to set initial password
  * System prompts user to re-enter and match password
  * System prompts user to enter information (id, name, address, etc.)
  * System sets default user type to basic employee
* Password requirements:
  * minimum length of 10 characters
  * must have a lower case letter, upper case letter, number, and special character
  * passwords must be updated every month
    * on successful login, if over a month since last change, prompts user to change password
* on successful login, system enables appropriate privileges for that login session
* if login not successful or user forgets password, system prompts user to contact an admin
  * or, redirects user to email to reset password with a web link

# Security
* The system tracks each login
  * system records the IP and account of every login event
  * if the IP is not previously recorded, the system sends the account email an alert including:
    * the IP of the login
    * the time of the login

# Data storage/retention
* The system stores monthly company payment reports indefinitely
* The system stores employee payment reports and information for up to five years after termination/retirement
* The system stores information in a external database.


# Reports & Status
* Any reports can printed or downloaded as a PDF
* The system can generate personal reports for any user, which contain:
  * gross total income for current pay period
  * federal tax rate and federal tax deductions
  * estimated income tax deduction
  * current payment period status: not yet generated, generated and processing, dispensed
  * projected net income after tax reductions
  * Total medical coverage cost for the pay period
  * Deductions for insurance for the pay period
  * Deductions for retirement for the pay period
  * hours of work, if user is hourly paid
* The system can generate personal reports for any past pay period
* The system will generate unofficial reports in real time for each type of employees, which contain:
  * The unofficial report can be printed as PDF document
  * The unofficial report can be download as PDF document
* Admin users can generate company reports that contain:
  * total gross employee pay
  * number of employees per department
  * total expected federal tax and local income tax
  * total gross employee pay per department
  * total man-hours of work by hourly employees
* Admin users can generate reports that adhere to all governmental regulations that can be sent to IRS
* Departmental heads and admin users can generate departmental reports, containing:
  * a departments total number of employees
  * personal reports for each departmental employee
  * total man-hours of work by hourly workers for a department
  * tax information for each departmental employee
* System can process and produce 20,000 records per minute.

# The following seem a little extraneous and/or difficult to understand, or redundant

* The official report can be generated
    * The format options can be chosen ( add format options here)
    * Need permission of some departments (?)
    * charge money for this report (?)
* The reports for the departments
  * This is in the screen for departments(such as: financial department
  * Empoyess basic information and name in this department
  * For each empoyees, the payment status (refer to the unofficail report for each employee)
  * The payments status for departments accounts ( The provision refer to the report for each employee)
  * For each payment, show the status in the work flow and send the status to admin
  * Once the status of payments change, send and notify the admin
  * Give authorization for departments in the work flow
  * ex. Financial department have authorization to send money from company bank account
  * Certain positions have authorization to press the approved button for the payment in processing status, at

* The reports for the admin
  * This is in the screen for admin (such as: CEO)
  * get notified when the status in work flow changed
  * be available for each emplyee's, each departments payment status
  * have authorization to send money from company bank account (?)
  * Have authorization to approve or disapprove a payment (?)

* The reports for the bank
  * This is in the account page for bank
  * choose the time period the report going to be generated
  * choose the items on the reports( departments, emplyees, customers ...)
  * format options ( add format options here for the bank)

* The reports for the government
  * This is in the account page of the department of government
  * choose the time period the reprot going to be generate
  * choose the items on the report ( departments, employees, customers ...)
  * format options (add format otions here for the department of government)

## Regulation


* Follow the private policy for the country
  * User private policy
    * According to government policy, before shipping, build the limitation of authorization of our stuff to access the customer's data
  * Company data private policy
    * Build the limitation for ANY user in this payroll system to UPLOAD data to the cloud, COPY data
    * Build the limitation for any history record that can not be edit and changed permanently

## Search system
* Build in search options (searched by payment history, by employee, by department etc)
* Build in searched by wrong words, searched by initial.. (aka, error input forgiveness)
* Different search system in terms of different users (Backup probably want to generate database history)

## User instruction in terms of interface
* Build the instructions of the system of account number for each type of user
* Build in user instruction after they sign up and first time use the payroll system (probably with cute arrow)
* Build in online html instructions with vividely screenshots (in case user searched by google for solution)
* If possiblee, build the short vedio for the instruction
