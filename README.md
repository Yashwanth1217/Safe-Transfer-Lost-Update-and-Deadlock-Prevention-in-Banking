# Safe-Transfer-Lost-Update-and-Deadlock-Prevention-in-Banking
SafeTransfer: Lost-Update and Deadlock Prevention in Banking. A DBMS course end project on Oracle 10g using PL/SQL stored procedures, an audit trigger and row-level locking to demonstrate ACID, lost updates and deadlocks.
# SafeTransfer: Lost-Update and Deadlock Prevention in Banking

A DBMS course end project (A9512 - Database Management Systems),
Vardhaman College of Engineering, Hyderabad.

SafeTransfer is a small banking database built on Oracle 10g. Deposits,
withdrawals and fund transfers are PL/SQL stored procedures that commit or
roll back as one unit, a trigger writes every balance change to an audit
table, and constraints reject invalid data. Two SQL*Plus sessions are used to
reproduce a lost update and a deadlock (ORA-00060), which are then fixed with
SELECT ... FOR UPDATE row locking and ordered locking of accounts.

Topics covered: ACID, transactions, schedules and serializability, stored
procedures, triggers, cursors, lock-based concurrency control, deadlock
handling.

## Files
- sql/01_setup.sql        - tables, constraints, sequences, trigger, sample data
- sql/02_procedures.sql   - deposit, withdraw, transfer_funds, mini_statement
- report/                 - project report (LaTeX source and PDF)

## Team
J. Sai Deekshith (25881A0546), T. Sai Purnanand (25881A0549),
G. Yashwanth (25881A0562)
Course Instructor: Ms. Shaik Shahanaz, Assistant Professor, CSE
