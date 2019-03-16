# Business Requirements
* (What the customer hopes to achieve with project)     
* The customers will be able to manage their payroll with ease with the system

# User Requirements (stakeholder requirements)
* (How the project will be used by end users)  m
* The user can view information about the current pay period.  m
* The user can request a report to be generated for the current pay period.    m
* Users can input employee information directly into the system manually.  s  implementation must, but not must individual user
* Users can type employees' information by keyboard.    c
* User can request payment in check or direct deposit.  c
* As a user, I can be paid either hourly or salaried.   w    
* Hourly workers will clock in and out according to a set schedule, and the system will calculate their pay according to their actual work times.   w
* Employees can change their set schedule.   w
* Managers can suspend employees.    c
* Admin users can     m
  * Search by name
  * Search by date
  * Search by id
  * click to see each employees' detailed information    m
    * edit employees' data
    * delete employee's data
  * add employees' data   s
    * name
    * id
    * position
    * date of payment
    * rate
    * regular hours
    * overtime
    * tax(?)
    * gross
  * change status (maybe for those who quit a company)  s
* Employee     m
  * can watch one's own     include manager's 
  * can request a report

* Admin users can login as admin      m  user types are must
* the system will deal with different access rights     m
  * admin
  * watcher(normal employee?)
* the system will deal with different time workers     w
  * full-time workers
  * part-time workers
* the system will deal with different residence information   c
  * U.S.
  * J1 VISA
  * other

# Functional Requirements
* (Detailed statements of the projects desired capabilities)
* The system can receive correctly formatted documents and translate that to payroll information.   m
* System will support English for the first release.    m
* The system uses U.S. currency.     m
* Schedule changes need approval of managers.   could because of vocation
* The system will calculate overtime pay for hourly workers, including weekend pay.  w
* Suspended employees receive no payment.      c
* System can handle taxes and bonuses.    m
* System can handle the amount of health insurance.   m
* The system can have pages(screens) below      w
  * Login: Login based on access rights (watch one's own, watch everyone or can edit/add data)
  * Home(for managers ?): showing a list of employees and their basic payroll information
  * Past employees' data (if needed)
  * Show: showing individual status in detail
  * Add: Add employees' data (admin only)
  * Edit: Edit or Update employees' data (admin only)
* Passwords for admin should change every week/month    s
* Build in search options (searched by payment history, by employee, by department etc) m                   
* Build in searched by wrong words, searched by initial.. (aka, error input forgiveness)  c
* Different search system in terms of different users (Backup probably want to generate database history)     m
* Build in user instruction after they sign up and first time use the payroll system (probably with cute arrow)   w
* Build in online html instructions with vividely screenshots (in case user searched by google for solution)  w
* If possiblee, build the short vedio for the instruction    w
* According to government policy, before shipping, build the limitation of authorization of our stuff to access the customer's data   w
* Payroll work flow is standard bi-weekly pay   m

# Nonfunctional Requirements
* (Are statements about quality of application (performance, etc))
* System can handle arbitrary amount of money when input.   m                 
* The system can handle an arbitrary amount of employees (dynamically allocated memory).   m
* System can generate at least 300 hundreds payrolls per second in the first release.  
* SQL is used as production database.    m
* Only command line (Unix and Windows) can be used as the platform.   m 


# Implementation Requirements
* (Temporary features to implement (migration scripts, etc))     
* SQL is used as development database.   m
