# Business Requirements
* (What the customer hopes to achieve with project)
* The customers will be able to manage their payroll with ease with the system

# User Requirements (stakeholder requirements)
* (How the project will be used by end users)
* The user can view information about the current pay period.
* The user can request a report to be generated for the current pay period.
* Users can input employee information directly into the system manually.
* Users can type employees' information by keyboard.
* User can request payment in check or direct deposit.
* As a user, I can be paid either hourly or salaried.
* Hourly workers will clock in and out according to a set schedule, and the system will calculate their pay according to their actual work times.
* Employees can change their set schedule.
* Managers can suspend employees.
* Admin users can
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
* Employee
  * can watch one's own
  * can request a report
* Users can login as watcher
* Admin users can login as admin
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

# Functional Requirements
* (Detailed statements of the projects desired capabilities)
* The system can receive correctly formatted documents and translate that to payroll information.
* System will support English for the first release.
* The system uses U.S. currency.
* Schedule changes need approval of managers.
* The system will calculate overtime pay for hourly workers, including weekend pay.
* Suspended employees receive no payment.
* System can handle taxes and bonuses.
* The system can have pages(screens) below
  * Login: Login based on access rights (watch one's own, watch everyone or can edit/add data)
  * Home(for managers ?): showing a list of employees and their basic payroll information
  * Past employees' data (if needed)
  * Show: showing individual status in detail
  * Add: Add employees' data (admin only)
  * Edit: Edit or Update employees' data (admin only)
* Passwords for admin should change every week/month
* Build in search options (searched by payment history, by employee, by department etc)
* Build in searched by wrong words, searched by initial.. (aka, error input forgiveness)
* Different search system in terms of different users (Backup probably want to generate database history)
* Build in user instruction after they sign up and first time use the payroll system (probably with cute arrow)
* Build in online html instructions with vividely screenshots (in case user searched by google for solution)
* If possiblee, build the short vedio for the instruction
* According to government policy, before shipping, build the limitation of authorization of our stuff to access the customer's data

# Nonfunctional Requirements
* (Are statements about quality of application (performance, etc))
* System can handle arbitrary amount of money when input.
* The system can handle an arbitrary amount of employees (dynamically allocated memory).

# Implementation Requirements
* (Temporary features to implement (migration scripts, etc))
