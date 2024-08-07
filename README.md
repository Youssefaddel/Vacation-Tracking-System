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
- Allow managers to directly award personal leave time.


## Non-Functional Requirements

- Security:
  - All user data must be encrypted during transmission and storage.
    
- Usability:
  - The user interface should be easy to navigate.

- Maintainability:
  - The system should allow for easy updates and maintenance


## Constraints

- Technological:
  -The system must be built using the existing company technology stack: Java Spring Boot, Angular, and PostgreSQL.
  
- Time:
  -The project must be completed within 6 months.
  
- Resource:
  -The system must be able to integrate with existing HR and email systems without additional staffing resources.

  
## Actors

- Employee: Requests vacation time.
- Manager: Approves or rejects vacation requests.
- HR Staff: Oversees the system and manages employee records.
- System administrator: responsible for the smooth running of the system’s technical resources.


## Use Case Diagram

![5870819388955936277](https://github.com/user-attachments/assets/809f9bc7-48e1-4c8f-9ea5-39c89d526753)


## ERD Diagram

![Database ER diagram (crow's foot)](https://github.com/user-attachments/assets/c39e1613-fcd0-4ad2-a762-90302834ee4a)


## Flowchart

![Flowchart (2)](https://github.com/user-attachments/assets/71fe66a5-2630-47c9-a502-09c0dba0646b)


## Sequence Diagram

![VTS (1)](https://github.com/user-attachments/assets/01ce3e74-3fa8-4514-a881-2ca52304cbd2)


## Pseudocode

```
BEGIN
    Authenticate Employee
    IF authentication fails THEN
        DISPLAY "Error: Authentication Failed"
        END
    ENDIF

    Employee SELECTS VTS Link

    RETRIEVE Employee Vacation Status

    Employee Create New Request
    IF Employee does NOT want to create a new request THEN
        END
    ENDIF

    Employee SELECTS "Vacation Category"
    PROMPT Employee for Dates and Time

    Employee ENTERS Details
    Employee SUBMITS Request

    VALIDATE Request
    IF validation fails THEN
        DISPLAY "Error"
        PROMPT Employee to Correct or Cancel
        GOTO "Employee ENTERS Details"
    ENDIF

    SET Request Status to "Pending Approval"
    SEND Email Notification to Manager

    Manager REVIEWS Request
    IF Manager APPROVES Request THEN
        SET Request Status to "Approved"
        SEND Approval Notification to Employee
    ELSE
        SEND Disapproval Notification to Employee
    ENDIF

END

```



