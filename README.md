Payroll Processing System
A COBOL-based Payroll Processing System designed to calculate employee pay and generate payroll reports using VSAM and sequential file processing.

System Overview
This system processes employee payroll data by: 
1. Reading employee records from a VSAM KSDS file
2. Calculating gross pay and deductions
3. Generating a payroll report in a sequential file

Program Components
1. PAYROLL.CBL
Main COBOL program that:

Reads employee records from VSAM
Calculates gross pay (Hours Worked * Hourly Rate)
Deducts taxes (20%) and insurance (5%)
Calculates net pay
Writes results to the output file

2. PAYROLL.JCL
JCL job that:

Compiles the COBOL program
Executes the program
Manages dataset allocations
Handles VSAM and sequential file I/O

3. PAYROLL.INPUT
Sample input data file containing employee records
