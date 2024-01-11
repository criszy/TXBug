# Dataset - TXBugs

This is the dataset for the ICSE'24 paper **Understanding Transaction Bugs in Database Systems**. See
[paper](http://www.tcse.cn/~cuiziyu20/papers/2024-icse-txbug.pdf) to learn more details.
It can be used to replicate and reproduce the paper's study, as well as to serve as a bug benchmark for future work on combating transaction bugs in database management systems.

An archived version of the artifact is available on Zenodo. See https://doi.org/10.5281/zenodo.10460740.

## Overview

This dataset contains 140 transaction bugs (TXBugs) collected from six widely-used DBMSs, i.e., MySQL, PostgreSQL, SQLite, MariaDB, CockroachDB, and TiDB.

## Detailed Description

This document contains in total 150 classification labels and around 1400 lines of clear and concise bug descriptions including transaction test cases, bug manifestations, root causes, bug impacts and fixes. The transaction test cases include initial database building statements, transaction statements, and the statement execution order for triggering TXBugs:
- Database: Indicate the database management system where the bug occurred.
- Bug ID: Indicate the issue where the bug was identified.
  Considering the issue (https://bugs.mysql.com/bug.php?id=103672), we record *103672* in this column.
- Bug URL: Indicate the location where the bug was reported. 
- Bug Report Description: Group of 8 columns that indicate the important information in bug report.
- Triggering Description: Indicate the necessary steps to trigger the bug.
- Isolation Level: Indicate the isolation level where the bug occurred.
- #Initial Table: Indicate the number of initial tables in a transaction test case.
- #Initial Data: Group of 5 columns that indicate the number of rows of data in a table.
- Transaction Mode: Indicate the transaction mode where the bug occurred.
- Transactions: Group of 11 columns that indicate the number and types of transactions in a transaction test case, and the number of SQL statements in a transaction.
- SQL Statements: Group of 24 columns that indicate the types of SQL statements in a transaction test case.
- Extra Triggering Conditions: Group of 5 columns that indicate the types of extra triggering conditions.
- Data Properties: Group of 7 columns that indicate types of data properties.
- Deterministic: Indicate whether the bug can be triggered deterministically.
- Manifestation: Indicate the types of failure symptoms.
- Transaction Semantic Violation: Indicate the types of transaction semantic violations.
- Priority: Indicate the priority levels.
- Fixed: Indicate whether the bug was fixed and why the bug was not fixed.
- Fixing Information: Group of 8 columns that indicate the fixing information of a fixed bug.
- Confirmed Duration: Indicate the duration of an unfixed bug.
- Detection Capability of Existing Approaches: Group of 3 columns that indicate whether existing approaches can detect the studied TXBug.