# Moj

Ministry Of Justice ERPNext customizations

## Features
### Iraqi Payroll Print Format
- Explanation: A custom `Print Format` named `Iraqi Payroll Slip`.
- Source: `{baseUrl}/app/print-format/Iraqi%20Payroll%20Slip`
- Usage: any salary slip -> press the print icon.
### Income Tax/Pension Deductions
- Explanation: Automated `Salary Slip` deductions for Iraqi `Income Tax`(ضريبة الدخل) and `Pension Deductions`(استقطاعات التقاعد).
- Source: `{baseUrl}/app/salary-slip/{id}` -> `Earnings & Deductions`.
- Usage: Whenever you submit a salary slip it will automatically add `Deductions` components named ضريبة الدخل and استقطاعات التقاعد.
### Custom Salary Slip Fields
- Explanation: Adds new `Custom Fields` for `Salary Slip`.
- Source: 
    - `{baseUrl}/app/custom-field/Salary Slip-show_employee_details`
    - `{baseUrl}/app/custom-field/Salary Slip-show_remarks`
    - `{baseUrl}/app/custom-field/Salary Slip-show_signature`
    - `{baseUrl}/app/custom-field/Salary Slip-show_deductions`
    - `{baseUrl}/app/custom-field/Salary Slip-show_allowances`
### Absence deductions
- Explanation: Adds new `Salary Slip` `Deduction` only and only if the employee has deductions.
- Source: `{baseUrl}/app/salary-slip/{id}` -> `Earnings & Deductions`.
- Usage: Whenever you submit a salary slip it will automatically add `Deductions` components named استقطاعات الغياب; only if the employee has absences.
- Notes: The component is added only if the employee has absences.