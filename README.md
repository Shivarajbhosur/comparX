# comparX
Uses Beyond Compare for PASS/FAIL and runs:  AFTER-only CSV comparison Root-level mixed-file comparison with digit-start reconstruction  Prompts to generate reports only on failures.  To generate reports for all files: &amp; "C:\Clients\SSAB.OX\baseline\CompareX.ps1" SG02\P02070-HPPL486P -PromptOnFail $false -GenerateReportOn All


<#
Tool Name : CompareX
Author      : Shivaraj Hosur Sangu
email: shivaraj.hosur@ensono.com
Description :
    Compares baseline vs generated output files
    - AFTER CSV comparison
    - Root-level mixed file comparison
    - Generates HTML and Word reports
#>

# ==============================================================
# CompareX.ps1  (UPDATED: Beyond Compare used for PASS/FAIL)
# Runs BOTH comparisons:
# 1) AFTER-only CSV comparison
# 2) Root-level mixed files comparison (digit-start reconstruction)
# Adds interactive prompt to generate report ONLY on failures.
# below commad for generate report for all even failed files
#PS C:\Clients\SSAB.OX\baseline> & "C:\Clients\SSAB.OX\baseline\CompareX.ps1" SG02\P02070-HPPL486P -PromptOnFail $false -GenerateReportOn All
# ==============================================================

command: PS C:\Users\shosur\git\validation-agent> compare-x -BaselineName "P50015-HPPL231P"
