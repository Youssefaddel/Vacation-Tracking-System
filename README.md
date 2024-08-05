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
- System administrator: responsible for the smooth running of the system’s technical       resources.


## Use Case Diagram

![5870819388955936277](https://github.com/user-attachments/assets/97b96bd4-13e3-42cc-9f7a-a7f7cea9885a)


## Sequence Diagram

![VTS](https://github.com/user-attachments/assets/15e51728-a8ce-4b9e-bc55-4067e41d6593)




