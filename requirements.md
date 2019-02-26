# General Requirements
* The user can view information about the current pay period.
* The user can request a report to be generated for the current pay period.
* The system can handle an arbitrary amount of employees (dynamically allocated memory).
* The system can receive correctly formatted documents and translate that to payroll information.
* Users can input employee information directly into the system manually.
* Users can type employees' information by keyboard.
* System will support English for the first release.
* System can handle arbitrary amount of money when input.
* There is a flexible number of users.

# Payment information
* User can request payment in check or direct deposit.
* As a user, I can be paid either hourly or salaried.
* The system uses U.S. currency.
* Hourly workers will clock in and out according to a set schedule, and the system will calculate their pay according to their actual work times.
* Employees can change their set schedule.
* Employees are not paid during regular time off (e.g. sick days), but they are paid during Paid Time Off.
* Employees are able to request an advance on pay. Admins must approve.
* Schedule changes need approval of managers.
* The system will calculate overtime pay for hourly workers, including weekend pay.
* Managers can suspend employees.
* Suspended employees receive no payment.
* System can handle taxes and bonuses.
* Payers can be company account, employees account, customer account, the bank account of departments
* Payee can be company account, employees account, customer account, the bank account of departments

# Screens – what screens are needed
* Login: Login based on access rights (watch one's own, watch everyone or can edit/add data)
* Home(for managers ?): showing a list of employees and their basic payroll information
* Past employees' data (if needed)
* Show: showing individual status in detail
* Add: Add employees' data (admin only)
* Edit: Edit or Update employees' data (admin only)
* User interface has a blue and grey color scheme.
* Business-themed interface

# Menus/Navigation – what menus will screens have
* Admin users can
  * Search by name
  * Search by date
  * Search by id
  * click to see each employees' detailed information
    * edit employees' data
    * delete employee's data
  * add employees and their data
    * name
    * id
    * position
    * date of payment
    * rate
    * regular hours
    * overtime
    * tax(?)
    * gross
  * change status (maybe for those who quit a company)
* Employee
  * can watch one's own
  * can request a report

# Login & Registration
* Registration for first time user
  * Clarify the account number system for each user
  * Input ID or company email
  * Set the password
    * declare the password requirements ( ex. must contain lower case, upper case, minimum digits etc.)
    * check the initial setting of password is whether qualified, if not, the page returned to "set the password"
    * detect the initial setting of password, report "where is the password invalid" on the returned page
  * Confirm the password ( Send the activation link to the input email)
  * fill the form for user information (refer to different types of user informatiom)
  * declare user types by user input
    * Customers
    * Employee
    * department
    * admin
* login
  * Users can login as watcher
  * Admin users can login as admin
  * Only account ID and password matched, the login is succesfull

* Password
  * Passwords for admin should change every week/month
  * Change password
    * must login in successfully with old password first
    * set the new password ( procedure here is same with first time set the password)
    * Confirm the password
  * Find back password
    * User input the related email account
    * send the activation link to that email
    * The activation link get to the password ressint page under that user's ID
* Forget User ID
 * prompt the user to input related emial and reset ID
 * If email doesn't work, input other informations ( ex. Employee ID, name, etc)
 * If the other informations still doesnt' work, display the option 'contact the administrator'
   * display the administrator's name and contact information

# Security
* Keep track the login device
 * For each user, keep track the login device by IP address
 * If a new device logged into system, sent an alert email to user's email account
   * Include user name
   * Include that login time and position
   * Include the new device's IP address (  ? )

# Data Storage
* Store the information on each employee for up to five years after termination/retirement
      * name
      * id
      * position
      * date of payment
      * rate
      * regular hours
      * overtime
      * taxes
      * gross
* Store system-generated reports indefinitely
* Backup data should be stored in an external database at a separate location. (?)


# User types
* The system will deal with different types of user
  * Customer
  * Empoyees
  * department
  * admin
* the system will deal with different access rights
  * admin
  * watcher(normal employee?)
* the system will deal with different time workers  
  * full-time workers
  * part-time workers
* the system will deal with different residence information
  * U.S.
  * J1 VISA
  * other

#Reports & Status
* The system will generate unofficial reports in real time for each type of employees
  * The total amount of payment supposed to be received
  * Payer
  * Payee bank account (or check number)
  * Status
    * The total amount of payment received before tax  (by day/ by hour/ by week/ by month/ by season / by year)
    * The total amount of payment in the processing (by day/ by hour/ by week/ by month/ by season / by year)
    * The total amount of payment newly generated (by day/ by hour/ by week/ by month/ by season / by year)
    * current status (generated / processing / received) for each payment
    * For the payments in processing and generated, display the information (tax & calculated based & amoubt for each unit time)
    * Display the tax amount for each payment (before taxed/ after taxed)
  * History status record
    * For each payment, the time when it changing status (generated/ processing/ received)
    * How long does this payment take from being generated to received
    * Display the detail information for all received payments (tax & calculated based * amount for each unit time)
    * Display the tax amount for each payment (before taxed/ after taxed)
  * tax information
    * tax type ( ex. federal government)
    * tax amount
    * tax returned status
    * tax returned amount
  * The unofficial report can be printed as PDF document
  * The unofficial report can be download as PDF document


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

# Regulation
* If position is in a state of U.S
  * Follow the minimum wage policy of this state for the empolyees
  * Follow the maximum charge amount policy of this state for the payments

* Follow the private policy for the country
  * User private policy
    * According to government policy, before shipping, build the limitation of authorization of our stuff to access the customer's data
  * Company data private policy
    * Build the limitation for ANY user in this payroll system to UPLOAD data to the cloud, COPY data
    * Build the limitation for any history record that can not be edit and changed permanently

# Search system
* Build in search options (searched by payment history, by employee, by department etc)
* Build in searched by wrong words, searched by initial.. (aka, error input forgiveness)
* Different search system in terms of different users (Backup probably want to generate database history)

#User instruction in terms of interface
* Build the instructions of the system of account number for each type of user
* Build in user instruction after they sign up and first time use the payroll system (probably with cute arrow)
* Build in online html instructions with vividely screenshots (in case user searched by google for solution)
* If possiblee, build the short vedio for the instruction
