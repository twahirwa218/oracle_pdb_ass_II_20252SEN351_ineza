# Oracle PDB Assignment II

## Overview of Tasks

This repository contains my submission for Assignment II, covering:
1. Creating a new Pluggable Database (PDB)
2. Creating and deleting a temporary PDB
3. Accessing Oracle Enterprise Manager (OEM)
4. Documentation and reporting on GitHub

## Oracle Environment Used

- **Oracle Database**: Oracle Database 21c Express Edition (XE)
- **Tool**: Oracle SQL Developer 23.1
- **Operating System**: Windows
- **OEM Access**: https://localhost:5500/em

## Explanation of Each Task

### Task 1: Create a New Pluggable Database
I created a PDB named `in_pdb_20252SEN351` using the `CREATE PLUGGABLE DATABASE` command.
The PDB was opened in READ WRITE mode and its state was saved for automatic startup.
A user named `ineza_plsqlauca_20252SEN351` was created inside the PDB with CONNECT,
RESOURCE, DBA, and UNLIMITED TABLESPACE privileges.

### Task 2: Create and Delete a Temporary PDB
I created a temporary PDB named `in_to_delete_pdb_20252SEN351`, verified its existence,
then closed and dropped it using `DROP PLUGGABLE DATABASE ... INCLUDING DATAFILES`.
I confirmed the deletion by querying `v$pdbs`, which returned no rows.

### Task 3: Oracle Enterprise Manager (OEM)
I accessed OEM at https://localhost:5500/em using the SYS user with SYSDBA role.
The dashboard reflected my Oracle environment, including the CDB and PDBs.

### Task 4: Documentation & Reporting
This README and the accompanying screenshots in the `screenshots/` folder
document all tasks.

## Challenges Faced and How They Were Solved

- **Challenge**: Initially could not connect to the database due to missing Oracle services.
  - **Solution**: Installed Oracle Database XE and verified the Windows services were running.
- **Challenge**: [Add any other challenges you faced]
  - **Solution**: [How you solved them]

## Integrity Statement

I declare that this submission is my own work. All commands were executed by me,
and all screenshots are from my own Oracle environment.

## Submission Details

- **Repository Link**: https://github.com/twahirwa218/oracle_pdb_ass_II_20252SEN351_ineza
- **PDB Name Created**: in_pdb_20252SEN351
- **Issues Encountered**: [Yes/No]
