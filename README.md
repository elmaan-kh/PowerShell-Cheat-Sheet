
# PowerShell Cheat Sheet

This repository serves as a cheat sheet for all the PowerShell cmdlets learned during the course. It includes a summary of cmdlets, descriptions, syntax, and practical examples.

### Table of Contents
1. [Classwork 1](#classwork-1)
2. [Classwork 2](#classwork-2)
3. [Classwork 3](#classwork-3)
4. [Classwork 4](#classwork-4)
5. [Classwork 5](#classwork-5)
6. [Classwork 6](#classwork-6)
7. [Classwork 7](#classwork-7)
8. [Classwork 8](#classwork-8)
9. [Classwork 10](#classwork-10)

---

## Classwork 1

### Cmdlets Documented:
#### **Write-Host**
- **Description:** Displays a message to the console.
- **Syntax:**
    ```powershell
    Write-Host "Message"
    ```
- **Example:**
    ```powershell
    Write-Host "This is a message"
    ```
- <img width="718" alt="image" src="https://github.com/user-attachments/assets/79ff695c-71d6-4ad4-9100-14b3c8729eb6">

#### **Get-Service | Where-Object {$_.Status -eq "Stopped"}**
- **Description:** Filters services that are stopped.
- **Syntax:**
    ```powershell
    Get-Service | Where-Object {$_.Status -eq "Stopped"}
    ```
- **Example:**
    ```powershell
    Get-Service | Where-Object {$_.Status -eq "Stopped"}
    ```
- <img width="539" alt="image" src="https://github.com/user-attachments/assets/789e5ea3-6848-44d2-b780-550492a3290f">

#### **$host.version**
- **Description:** Displays the version of the current PowerShell host.
- **Syntax:**
    ```powershell
    $host.version
    ```
- **Example:**
    ```powershell
    $host.version
    ```
- <img width="329" alt="image" src="https://github.com/user-attachments/assets/63e032df-c152-461b-83a9-2af56922be52">

#### **Get-History**
- **Description:** Retrieves the history of commands used in the session.
- **Syntax:**
    ```powershell
    Get-History
    ```
- **Example:**
    ```powershell
    Get-History
    ```
- <img width="549" alt="image" src="https://github.com/user-attachments/assets/c70d653d-4815-4c06-ae45-9fb6a486c082">

#### **Invoke-History 3**
- **Description:** Executes a command from the history list by its ID.
- **Syntax:**
    ```powershell
    Invoke-History <ID>
    ```
- **Example:**
    ```powershell
    Invoke-History 3
    ```
- <img width="348" alt="image" src="https://github.com/user-attachments/assets/a5e32a50-dced-4ac3-aeaa-bc1c31a98908">

#### **Write-Output "This is a sentence"**
- **Description:** Outputs a string to the pipeline.
- **Syntax:**
    ```powershell
    Write-Output "This is a sentence"
    ```
- **Example:**
    ```powershell
    Write-Output "This is a sentence"
    ```
- <img width="562" alt="image" src="https://github.com/user-attachments/assets/e9279a7a-e121-4252-a877-3a29778f3a68">

### Summary:
Classwork 1 focused on basic cmdlets for output, service management, and command history. `Write-Host` and `Write-Output` helped with displaying messages, `Get-Service` with filtering services, and `$host.version` showed PowerShell host details. Additionally, you learned to work with command history using `Get-History` and `Invoke-History`.

---

## Classwork 2

### Cmdlets Documented:
#### **Get-Help**
- **Description:** Provides help documentation for cmdlets.
- **Syntax:**
    ```powershell
    Get-Help <CmdletName>
    ```
- **Example:**
    ```powershell
    Get-Help Get-Service
    ```
- **Screenshot**

#### **Set-ExecutionPolicy**
- **Description:** Changes the user preference for script execution policies.
- **Syntax:**
    ```powershell
    Set-ExecutionPolicy <Policy>
    ```
- **Example:**
    ```powershell
    Set-ExecutionPolicy RemoteSigned
    ```
- **Screenshot**

#### **Export-CSV**
- **Description:** Exports data to a CSV file.
- **Syntax:**
    ```powershell
    Export-CSV -Path <FilePath> -NoTypeInformation
    ```
- **Example:**
    ```powershell
    Get-Service | Export-CSV -Path "C:\services.csv" -NoTypeInformation
    ```
- **Screenshot**

#### **Select-Object**
- **Description:** Selects specific properties of an object.
- **Syntax:**
    ```powershell
    Select-Object -Property <Property1>, <Property2>
    ```
- **Example:**
    ```powershell
    Get-Service | Select-Object -Property Name, Status
    ```
- **Screenshot**

#### **Get-Process**
- **Description:** Retrieves a list of all running processes.
- **Syntax:**
    ```powershell
    Get-Process
    ```
- **Example:**
    ```powershell
    Get-Process
    ```
- **Screenshot**

#### **Stop-Process**
- **Description:** Stops a process by its ID or name.
- **Syntax:**
    ```powershell
    Stop-Process -Name <ProcessName>
    ```
- **Example:**
    ```powershell
    Stop-Process -Name "notepad"
    ```
- **Screenshot**

#### **Get-Service**
- **Description:** Retrieves information about services on the system.
- **Syntax:**
    ```powershell
    Get-Service
    ```
- **Example:**
    ```powershell
    Get-Service
    ```
- **Screenshot**

#### **Get-WmiObject**
- **Description:** Retrieves WMI objects.
- **Syntax:**
    ```powershell
    Get-WmiObject -Class <ClassName>
    ```
- **Example:**
    ```powershell
    Get-WmiObject -Class Win32_OperatingSystem
    ```
- **Screenshot**

#### **Get-EventLog**
- **Description:** Retrieves event log data.
- **Syntax:**
    ```powershell
    Get-EventLog -LogName <LogName>
    ```
- **Example:**
    ```powershell
    Get-EventLog -LogName Application
    ```
- **Screenshot**

#### **Get-Content**
- **Description:** Retrieves the content of a file.
- **Syntax:**
    ```powershell
    Get-Content -Path <FilePath>
    ```
- **Example:**
    ```powershell
    Get-Content -Path "C:\temp\file.txt"
    ```
- **Screenshot**

#### **Get-NetAdapter**
- **Description:** Retrieves network adapter information.
- **Syntax:**
    ```powershell
    Get-NetAdapter
    ```
- **Example:**
    ```powershell
    Get-NetAdapter
    ```
- **Screenshot**

### Summary:
Classwork 2 introduced essential cmdlets for managing system processes, services, event logs, and network adapters. `Get-Help` provided guidance, while `Set-ExecutionPolicy` modified script execution rules. You also learned to export data to CSV with `Export-CSV`, filter output with `Select-Object`, and manipulate processes and services with `Get-Process`, `Stop-Process`, and `Get-Service`. WMI and event logs were explored with `Get-WmiObject` and `Get-EventLog`.

---

## Classwork 3
*No commands to include*

### Summary:
Classwork 3 did not include any specific commands.

---

## Classwork 4

### Cmdlets Documented:
#### **Get-ADComputer**
- **Description:** Retrieves information about Active Directory computers.
- **Syntax:**
    ```powershell
    Get-ADComputer -Identity <ComputerName>
    ```
- **Example:**
    ```powershell
    Get-ADComputer -Identity "Computer01"
    ```
- **Screenshot**

#### **ForEach-Object**
- **Description:** Performs an action for each object in a pipeline.
- **Syntax:**
    ```powershell
    ForEach-Object {<ScriptBlock>}
    ```
- **Example:**
    ```powershell
    Get-Service | ForEach-Object { $_.Name }
    ```
- **Screenshot**

### Summary:
Classwork 4 covered `Get-ADComputer`, which is used to retrieve Active Directory computer details, and `ForEach-Object`, which allows you to iterate over a collection of objects in a pipeline to perform actions on each object.

---

## Classwork 5

### Cmdlets Documented:
#### **Enable PS-Remoting**
- **Description:** Enables PowerShell Remoting on the system.
- **Syntax:**
    ```powershell
    Enable-PSRemoting -Force
    ```
- **Example:**
    ```powershell
    Enable-PSRemoting -Force
    ```
- **Screenshot**

#### **Invoke-Command**
- **Description:** Runs a command on a remote system.
- **Syntax:**
    ```powershell
    Invoke-Command -ScriptBlock {<Command>} -ComputerName <ComputerName>
    ```
- **Example:**
    ```powershell
    Invoke-Command -ScriptBlock { Get-Process } -ComputerName "Server01"
    ```
- **Screenshot**

#### **New-PSSession**
- **Description:** Creates a new PowerShell session to a remote system.
- **Syntax:**
    ```powershell
    New-PSSession -ComputerName <ComputerName>
    ```
- **Example:**
    ```powershell
    New-PSSession -ComputerName "Server01"
    ```
- **Screenshot**

#### **Get-Module**
- **Description:** Retrieves information about modules in the session.
- **Syntax:**
    ```powershell
    Get-Module
    ```
- **Example:**
    ```powershell
    Get-Module
    ```
- **Screenshot**

#### **Import-Module**
- **Description:** Imports a module into the current session.
- **Syntax:**
    ```powershell
    Import-Module <ModuleName>
    ```
- **Example:**
    ```powershell
    Import-Module ActiveDirectory
    ```
- **Screenshot**

#### **Get-RemoteNetAdapter**
- **Description:** Retrieves network adapter information from a remote system.
- **Syntax:**
    ```powershell
    Get-RemoteNetAdapter -ComputerName <ComputerName>
    ```
- **Example:**
    ```powershell
    Get-RemoteNetAdapter -ComputerName "Server01"
    ```
- **Screenshot**

#### **Remove-PSSession**
- **Description:** Closes an established remote session.
- **Syntax:**
    ```powershell
    Remove-PSSession -Session <Session>
    ```
- **Example:**
    ```powershell
    Remove-PSSession -Session $session
    ```
- **Screenshot**

#### **Enter-PSSession**
- **Description:** Starts an interactive remote PowerShell session.
- **Syntax:**
    ```powershell
    Enter-PSSession -ComputerName <ComputerName>
    ```
- **Example:**
    ```powershell
    Enter-PSSession -ComputerName "Server01"
    ```
- **Screenshot**

### Summary:
Classwork 5 focused on enabling and using PowerShell Remoting. Cmdlets such as `Invoke-Command`, `New-PSSession`, and `Enter-PSSession` were used for remote command execution, while `Get-Module` and `Import-Module` helped manage modules. You also learned to retrieve network adapter information remotely with `Get-RemoteNetAdapter` and close remote sessions with `Remove-PSSession`.

---

## Classwork 6

### Cmdlets Documented:
#### **Get-CimClass**
- **Description:** Retrieves a list of CIM (Common Information Model) classes.
- **Syntax:**
    ```powershell
    Get-CimClass
    ```
- **Example:**
    ```powershell
    Get-CimClass
    ```
- **Screenshot**

#### **Where-Object**
- **Description:** Filters objects in a pipeline based on a condition.
- **Syntax:**
    ```powershell
    Where-Object { <Condition> }
    ```
- **Example:**
    ```powershell
    Get-CimInstance -ClassName Win32_OperatingSystem | Where-Object { $_.Version -eq "10.0.18363" }
    ```
- **Screenshot**

#### **Get-CimInstance**
- **Description:** Retrieves CIM instances (like WMI).
- **Syntax:**
    ```powershell
    Get-CimInstance -ClassName <ClassName>
    ```
- **Example:**
    ```powershell
    Get-CimInstance -ClassName Win32_OperatingSystem
    ```
- **Screenshot**

### Summary:
Classwork 6 focused on CIM cmdlets, like `Get-CimClass`, `Get-CimInstance`, and `Where-Object` to retrieve and filter data from CIM classes, which are used for querying system information similar to WMI.

---

## Classwork 7

### Cmdlets Documented:
#### **Get-Variable**
- **Description:** Retrieves the values of PowerShell variables.
- **Syntax:**
    ```powershell
    Get-Variable
    ```
- **Example:**
    ```powershell
    Get-Variable
    ```
- **Screenshot**

#### **Remove-Variable**
- **Description:** Removes a variable from the session.
- **Syntax:**
    ```powershell
    Remove-Variable -Name <VariableName>
    ```
- **Example:**
    ```powershell
    Remove-Variable -Name "MyVar"
    ```
- **Screenshot**

### Summary:
Classwork 7 introduced variable management using `Get-Variable` and `Remove-Variable` to retrieve and delete variables in the session.

---

## Classwork 8

### Cmdlets Documented:
#### **Read-Host**
- **Description:** Prompts the user for input.
- **Syntax:**
    ```powershell
    Read-Host "Enter your input"
    ```
- **Example:**
    ```powershell
    Read-Host "Enter your name"
    ```
- **Screenshot**

#### **Out-File**
- **Description:** Sends output to a file.
- **Syntax:**
    ```powershell
    Out-File -FilePath <FilePath>
    ```
- **Example:**
    ```powershell
    "This is a test" | Out-File -FilePath "C:\test.txt"
    ```
- **Screenshot**

### Summary:
Classwork 8 focused on user input with `Read-Host` and output redirection with `Out-File`.

---

## Classwork 9
*No commands to include*

### Summary:
Classwork 9 did not include any specific commands.

---

## Classwork 10

### Cmdlets Documented:
#### **New-Item**
- **Description:** Creates a new item, such as a file or directory.
- **Syntax:**
    ```powershell
    New-Item -Path <Path> -ItemType <ItemType>
    ```
- **Example:**
    ```powershell
    New-Item -Path "C:\test" -ItemType Directory
    ```
- **Screenshot**

#### **New-SmbShare**
- **Description:** Creates a new SMB share.
- **Syntax:**
    ```powershell
    New-SmbShare -Name <ShareName> -Path <SharePath>
    ```
- **Example:**
    ```powershell
    New-SmbShare -Name "SharedFolder" -Path "C:\Shared"
    ```
- **Screenshot**

#### **Get-SmbShare**
- **Description:** Retrieves information about SMB shares.
- **Syntax:**
    ```powershell
    Get-SmbShare
    ```
- **Example:**
    ```powershell
    Get-SmbShare
    ```
- **Screenshot**

#### **Get-Printer**
- **Description:** Retrieves information about installed printers.
- **Syntax:**
    ```powershell
    Get-Printer
    ```
- **Example:**
    ```powershell
    Get-Printer
    ```
- **Screenshot**

#### **Test-Path**
- **Description:** Checks if a path exists.
- **Syntax:**
    ```powershell
    Test-Path <Path>
    ```
- **Example:**
    ```powershell
    Test-Path "C:\test"
    ```
- **Screenshot**

### Summary:
Classwork 10 covered file and printer management using `New-Item`, `New-SmbShare`, `Get-SmbShare`, `Get-Printer`, and `Test-Path` to work with directories, network shares, printers, and file paths.

---


