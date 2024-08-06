# Vacation-Tracking-System

## Vision

VTS will empower individual employees to manage their vacation time, sick leave, and personal time off efficiently, without extensive knowledge of company policies. It will streamline the process and reduce the time required for approval.

## Functional Requirements

- Implement a rules-based system for:
  - validating
  - verifying leave time requests
- Enable manager approval (Optional)
- Provide access to previous calendar year requests and allow requests up to a year and a half in advance.
- use e-mail notifications to:
  -  Request manager approval (Notify the manager)
  -  Status changes (Notify the employee)
- Keep activity logs for all transactions.
- Enables the HR and System Administrator to override all actions restricted by rules with logging those overrides.
- Provide a Web service interface for querying an employee’s vacation request summary.
- Interface with HR department legacy systems for employee information retrieval and updates.
- Allow managers to directly award personal leave time (within system-set limits).


## Actors

- Employee: Requests vacation time.
- Manager: Approves or rejects vacation requests.
- HR Staff: Oversees the system and manages employee records.
- System administrator: responsible for the smooth running of the system’s technical resources.


## Use Case Diagram

![5870819388955936277](https://github.com/user-attachments/assets/809f9bc7-48e1-4c8f-9ea5-39c89d526753)


## Sequence Diagram

-Actors:
  -Employee
  -Internal Portal
  -System (VTS)
  -Manager

![VTS (1)](https://github.com/user-attachments/assets/01ce3e74-3fa8-4514-a881-2ca52304cbd2)


## ERD Diagram

![Database ER diagram (crow's foot)](https://github.com/user-attachments/assets/c39e1613-fcd0-4ad2-a762-90302834ee4a)



