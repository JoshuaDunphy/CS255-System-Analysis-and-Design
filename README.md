# CS 255 Sample Business Requirements Document for an ATM

> **Note**: The following is a sample of the business requirements document for an ATM system. Use this as an example of the types of requirements you should be collecting for each of the categories. It is important to know that this is **not an exhaustive list** of all functionality for an ATM system, but just a sample.

---

## System Components and Design

### Purpose
- This project is for one of our clients, a **banking institution**.  
  The purpose is to make their customer services **easier and more efficient** as well as to provide customers with access to their accounts.

### System Background
- The client asked us to build a **system that enables customers to withdraw, deposit, and check account balances using an ATM card**.
- The system, called an **ATM or automated teller machine**, will provide banking services to customers.
- The system will consist of a **large machine** that is **connected to the central bank via internet**.

---

## Objectives and Goals

The system will provide the user with the following functions:
- Withdraw money
- Deposit money
- Print transactions
- Check balance

---

## Requirements

### Functional Requirements
- **ATM must lock card** after three failed attempts to enter PIN.

### Nonfunctional Requirements
- The time it takes to **connect to the central bank**, retrieve information, and display it to the customer should **not exceed 10 seconds**.
- Updates to the **ATM should be pushed from a central bank system** with the presence of a technician for backup.

---

## Performance Requirements
- **Rationale**: Performance requirements capture the aspects of the system such as the **speed of different functions**, storage capacity, battery (if applicable), and updates.  
  For an ATM, it would be important to have **quick transactions** to avoid user frustration and long lines.  
  Since an ATM deals with **sensitive financial information**, updates should be made in a **very controlled way** to make sure that the updates are verified and that someone is on hand in case there are any issues.

---

# UML Diagrams for ATM Cash Withdrawal

## UML Activity Diagram

```mermaid
flowchart TD
    A[Start] --> B[Verify PIN]
    B -->|Wrong PIN| C[Wrong PIN]
    B -->|Correct PIN| D[Ask for Amount]
    D --> E{Amount Not Available}
    E -->|Yes| F[Dispense Cash]
    E -->|No| G[Amount Not Available]
    F --> H[Generate Receipt]
    H --> I[Print Receipt]
    I --> J[End]