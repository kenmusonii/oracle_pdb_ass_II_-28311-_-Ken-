
**Name:** Ken MUSONI   
**Student ID:** 28311  
**Course:** Database Development with PL/SQL (INSY 8311)  
**Instructor:** Eric Maniraguha  
**Oracle Version:** 21c Express Edition (XE)  

## Overview

This repository documents navigation on Oracle Pluggable Databases (PDB) management.  
The assignment demonstrates practical skills in:

- Creating and managing Pluggable Databases
- Creating users inside a PDB
- Verifying PDBs via SQL*Plus and Oracle Enterprise Manager (OEM)
- Documenting work professionally on GitHub

## Task 1 — Create a New Pluggable Database

- **PDB Name:** `ke_pdb_28311`  
- **User Created:** `ken_plsqlauca_28311`  

**Steps Taken:**

1. Connected to the root container (`CDB$ROOT`) as SYSDBA in SQL*Plus.  
2. Created the PDB by cloning `PDB$SEED`.  
3. Opened the PDB.  
4. Switched session to the new PDB.  
5. Created the required user and granted `CREATE SESSION` privileges.  

**Evidence:**  
![PDB Creation and User Creation ](Screenshots/PDB&UserCreation.png)  


## Task 2 — Create and Delete a Temporary PDB

- **Temporary PDB Name:** `ke_to_delete_pdb_28311`  

**Steps Taken:**

1. Created the temporary PDB from `PDB$SEED`.  
2. Verified the PDB exists using `SHOW PDBS`.  
3. Opened the temporary PDB.  
4. Closed and deleted it completely using `DROP PLUGGABLE DATABASE ... INCLUDING DATAFILES`.  

**Evidence:**  
![Temporary PDB Creation](screenshots/task2_pdb_creation.png)  
![Temporary PDB Deletion](screenshots/task2_pdb_deletion.png)  

---

## Task 3 — Oracle Enterprise Manager (OEM)

**Notes:**

- Attempted to access OEM via browser (`https://localhost:5500/em`).  
- Encountered port conflicts, so full dashboard PDB view was limited.  
- Verified all PDBs and user creation via SQL*Plus commands instead.

**Evidence:**  
![PDBs Verified in SQLPlus](screenshots/task3_oem_dashboard.png)  

## Challenges Faced

- OEM login failed initially due to port conflict (`ORA-44718`).  
- Resolved by using SQL*Plus commands (`SHOW PDBS`, `SELECT username FROM dba_users`) to verify tasks.  
- Screenshot evidence still clearly demonstrates successful task completion.  



## Integrity Statement

I confirm that this work is entirely my own. All commands, screenshots, and documentation reflect my individual execution without any unauthorized help or collaboration.

