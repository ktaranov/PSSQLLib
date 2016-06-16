# Powershell SQL Server Library (PSSQLLib)
[![licence badge]][licence]
[![stars badge]][stars]
[![forks badge]][forks]
[![issues badge]][issues]

PowerShell is very good for retrieving information from SQL Server. The problem is that most of the time we have to create the scripts every time or load them from a previous file. Because I hate to do things twice I created a PowerShell module for SQL Server which enables me to retrieve information from my instances with a few simple commands and is called PSSQLLib.

Is uses the [SQL Server SMO](https://msdn.microsoft.com/en-us/library/cc281947.aspx) for retrieving information from SQL Server and uses the WMI to get information from the host.

**The module is definitely not done and additions can be made. If you have any functionality that could be included please send it to me and I’ll include it in the library.**


## Requirements
The module needs at **least PowerShell version 3.0** installed.

Additionally you need the SQL Server SMO installed. If you’ve got the SQL Server Management Studio installed on the machine your running this module from, then you don’t have to do anything.
If it’s not installed, you can download and install the SQL Server Feature pack. The version for 2014 can be found [here](https://www.microsoft.com/en-us/download/details.aspx?id=42295).


## Features

The library has the following features:

 - Export database objects
 - Export SQL Server objects
 - Get the host harddisk information
 - Get the host hardware
 - Get the host operating system information
 - Get the host uptime
 - Get the SQL Server instance settings
 - Get the SQL Server instance configuration settings
 - Get the SQL Server instance uptime
 - Get the SQL Server login server privileges
 - Get the SQL Server databases
 - Get the SQL Server database files
 - Get the SQL Server database users
 - Get the SQL Server database user privileges
 - Get the SQL Server Agent jobs
 - Get the SQL Server disk latencies

## Installation PSSQLLib
1. Unzip the file.
2. Make a directory (if not already present) named **"PSSQLLib"** in one of the following standard Powershell Module directories:
* $Home\Documents\WindowsPowerShell\Modules (%UserProfile%\Documents\WindowsPowerShell\Modules)
* $Env:ProgramFiles\WindowsPowerShell\Modules (%ProgramFiles%\WindowsPowerShell\Modules)
* $Systemroot\System32\WindowsPowerShell\v1.0\Modules (%systemroot%\System32\WindowsPowerShell\v1.0\Modules)
3. Place both the psd1 and psm1 files in the module directory created earlier.
4. Execute the following command in a PowerShell command screen: `Import-Module PSSQLLib`

To check if the module is imported correctly execute the following command:
`Get-Command -Module PSSQLLib`  or `Get-Module -Name PSSQLLib`

You should be able to see a list of all functions.


## License
MIT


[licence badge]:https://img.shields.io/badge/license-MIT-blue.svg
[stars badge]:https://img.shields.io/github/stars/sanderstad/PSSQLLib.svg
[forks badge]:https://img.shields.io/github/forks/sanderstad/PSSQLLib.svg
[issues badge]:https://img.shields.io/github/issues/sanderstad/PSSQLLib.svg

[licence]:https://github.com/sanderstad/PSSQLLib/blob/master/LICENSE.md
[stars]:https://github.com/sanderstad/PSSQLLib/stargazers
[forks]:https://github.com/sanderstad/PSSQLLib/network
[issues]:https://github.com/sanderstad/PSSQLLib/issues
