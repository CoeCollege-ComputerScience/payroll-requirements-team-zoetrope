# General Requirements
* The user can view information about the current pay period.
* The user can request a report to be generated for the current pay period.
* The system can handle an arbitrary amount of employees (dynamically allocated memory).
* The system can receive correctly formatted documents and translate that to payroll information.
* Users can input employee information directly into the system manually.

# Payment information
* User can request payment in check or direct deposit.
* As a user, I can be paid either hourly or salaried.
* The system uses U.S. currency.
* Hourly workers will clock in and out according to a set schedule, and the system will calculate their pay according to their actual work times.
* Employees can change their set schedule.
* Schedule changes need approval of managers.
* The system will calculate overtime pay for hourly workers, including weekend pay.
* Managers can suspend employees.
* Suspended employees receive no payment.

# Screens – what screens are needed
* Login: Login based on access rights (watch one's own, watch everyone or can edit/add data)
* Home(for managers ?): showing a list of employees and their basic payroll information
* Past employees' data (if needed)
* Show: showing individual status in detail
* Add: Add employees' data (admin only)
* Edit: Edit or Update employees' data (admin only)

# Menus/Navigation – what menus will screens have
* Admin(?)
  * Search by name
  * Search by date
  * Search by id
  * click to see each employees' detailed information
    * edit employees' data
    * delete employee's data
  * add employees' data
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
* Employee(?)
  * watch one's own
  * request a report

# Login
* Passwords for admin should change every week/month
* Login as watcher
* Login as admin


# User types
* access rights
  * admin
  * watcher(normal employee?)
* time  
  * full-time workers
  * part-time workers
* Residence
  * U.S.
  * J1 VISA
  * other

#Search system
* Build in search options (searched by payment history, by employee, by department etc)
* Build in searched by wrong words, searched by initial.. (aka, error input forgiveness)
* Different search system interms of different users (Backup probably want to generate database history)

# User instruction in terms of interface
* Build in user instruction after they sign up and first time use the payroll system (probably with cute arrow)
* Build in online html instructions with vividely screenshots (in case user searched by google for solution)
* If possiblee, build the short vedio for the instruction

# User private policy
* According to government policy, before shipping, build the limitation of authorization of our stuff to access the customer's data 






