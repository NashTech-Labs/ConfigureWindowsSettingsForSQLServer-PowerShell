Using this template we can configure settings to optimize our SQL Server on Windows by the help of powershell scripts.

*Configure-Windows-Firewall-SQL-Ports.ps1* is used to to Configure Firewall Rules for SQL Server using PowerShell.

*Grant-SQL-Server-Account-Lock-Pages-in-Memory-and-Volume-Maintenance-Tasks.ps1* is used to Grant SQL Server account access to Lock Pages in Memory and Perform Volume Maintenance Tasks .

## Change Processor Scheduling

### To set Processor Scheduling to Programs:

```Set-ItemProperty HKLM:\SYSTEM\CurrentControlSet\Control\PriorityControl -Name Win32PrioritySeparation -Value 2 ```

### To Set Processor Scheduling to Background Services:

```Set-ItemProperty HKLM:\SYSTEM\CurrentControlSet\Control\PriorityControl -Name Win32PrioritySeparation -Value 18```