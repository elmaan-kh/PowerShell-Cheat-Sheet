
# PowerShell Cheat Sheet

The following content provides a cheat sheet for PowerShell

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
In Classwork 1 I have learned basic commands for output, service management, and command history. `Write-Host` and `Write-Output` helped with displaying messages, `Get-Service` with filtering services, and `$host.version` showed PowerShell host details. I also learned to work with command history using `Get-History` and `Invoke-History`.

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
- <img width="422" alt="image" src="https://github.com/user-attachments/assets/316f6636-1bd1-42cf-a43b-1492fbc366fd">


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
- <img width="436" alt="image" src="https://github.com/user-attachments/assets/6b723bd4-c87c-4522-a435-c1dc158cb64f">


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
- <img width="674" alt="image" src="https://github.com/user-attachments/assets/8781db57-0152-462a-95c9-b0446c801078">


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
- <img width="602" alt="image" src="https://github.com/user-attachments/assets/c2d528e8-78b8-42f2-b9e4-0548074dbc61">


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
- <img width="568" alt="image" src="https://github.com/user-attachments/assets/ddacdbe5-2287-421a-9fea-03a0b7311ff5">


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
- <img width="283" alt="image" src="https://github.com/user-attachments/assets/b7104a1c-7e62-433b-9c46-94ccb00f4d99">
- <img width="302" alt="image" src="https://github.com/user-attachments/assets/e82ff83c-1b5f-40df-9ee2-1f83b6dec456">



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
- <img width="511" alt="image" src="https://github.com/user-attachments/assets/2ab7f9a9-3f09-4bc0-97ae-5e1a70bf10bd">


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
- <img width="484" alt="image" src="https://github.com/user-attachments/assets/2d2f463b-0b3c-43c0-a789-39362666713c">


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
- <img width="850" alt="image" src="https://github.com/user-attachments/assets/592c4b38-94c1-4cbb-86ab-61059fe139ea">


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
- <img width="521" alt="image" src="https://github.com/user-attachments/assets/8eedd241-a79a-4f6f-aa29-129391b1a062">


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
- <img width="932" alt="image" src="https://github.com/user-attachments/assets/482ac88e-257a-4fe0-b453-2a366fd3a60a">


### Summary:
In Classwork 2, I learned important commands for managing system processes, services, event logs, and network adapters. `Get-Help` provided guidance, while `Set-ExecutionPolicy` modified script execution rules. I also learned to export data to CSV with `Export-CSV`, filter output with `Select-Object`, and manipulate processes and services with `Get-Process`, `Stop-Process`, and `Get-Service`. WMI and event logs were explored with `Get-WmiObject` and `Get-EventLog`.

---

## Classwork 3
*No commands to include*

### Summary:
Although there were no new commands that I got to use, this classwork focused on handling CSV files, exploring Export-CSV and Import-CSV for data export and conversion, and comparing plain text vs. CSV-formatted outputs. It also introduced service management with Stop-Service and Restart-Service.

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
- <img width="914" alt="image" src="https://github.com/user-attachments/assets/3ea54fe4-4b61-4949-ad58-780019761850">


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
- <img width="914" alt="image" src="https://github.com/user-attachments/assets/9e4202eb-200c-4bc6-80e0-158aed3219b0">


### Summary:
In Classwork 4, I covered `Get-ADComputer`, which is used to retrieve Active Directory computer details, and `ForEach-Object`, which allows you to iterate over a collection of objects in a pipeline to perform actions on each object.

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
- <img width="588" alt="image" src="https://github.com/user-attachments/assets/76d7fc74-2986-45ba-9c65-0d2a6a84201b">


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
- <img width="890" alt="image" src="https://github.com/user-attachments/assets/14607456-d0ae-4f97-8616-00c8d5b5d46d">


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
- <img width="707" alt="image" src="https://github.com/user-attachments/assets/561ac418-3050-4701-923c-da311dcb1dd0">


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
- <img width="931" alt="image" src="https://github.com/user-attachments/assets/4ca37611-d576-43fb-8a54-d1655a59c619">


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
- <img width="898" alt="image" src="https://github.com/user-attachments/assets/3340196c-35fd-44f8-9e10-366d71242510">


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
- <img width="923" alt="image" src="https://github.com/user-attachments/assets/e066c9ed-231a-40ad-ac62-7a013b2d1214">


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
- <img width="771" alt="image" src="https://github.com/user-attachments/assets/d847538d-aec3-42ed-becb-2210d436d17d">


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
- <img width="736" alt="image" src="https://github.com/user-attachments/assets/52acb26f-fe47-4dc8-be61-dd3887583e41">


### Summary:
In Classwork 5, I focused on enabling and using PowerShell Remoting. Commands like `Invoke-Command`, `New-PSSession`, and `Enter-PSSession` were used for remote command execution, while `Get-Module` and `Import-Module` helped manage modules. I also learned to retrieve network adapter information remotely with `Get-RemoteNetAdapter` and close remote sessions with `Remove-PSSession`.

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
- <img width="893" alt="image" src="https://github.com/user-attachments/assets/742e2c31-02b8-4784-96b6-3fa6e5fa2047">


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
- <img width="897" alt="image" src="https://github.com/user-attachments/assets/a4e3bf41-fd34-4be7-abce-6c8636480f61">


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
- <img width="896" alt="image" src="https://github.com/user-attachments/assets/81ac5a8b-4321-4061-9941-c85f63dec1cb">


### Summary:
For Classwork 6, I focused on CIM commands, like `Get-CimClass`, `Get-CimInstance`, and `Where-Object` to retrieve and filter data from CIM classes, which are used for querying system information similar to WMI.

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
- <img width="706" alt="image" src="https://github.com/user-attachments/assets/44b4a013-95c0-4855-99c5-bd5583e187c4">


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
- <img width="927" alt="image" src="https://github.com/user-attachments/assets/e5ac6d9d-4281-4604-ae4d-893679a508cd">


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
- <img width="665" alt="image" src="https://github.com/user-attachments/assets/b03c1667-2256-4ab3-bce1-7dee6a1b636b">
- <img width="353" alt="image" src="https://github.com/user-attachments/assets/ba74f1c3-e03d-448c-8a44-5155763ec791">



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
- <img width="665" alt="image" src="https://github.com/user-attachments/assets/b03c1667-2256-4ab3-bce1-7dee6a1b636b">
- <img width="353" alt="image" src="https://github.com/user-attachments/assets/ba74f1c3-e03d-448c-8a44-5155763ec791">


### Summary:
Classwork 8 focused on user input with `Read-Host` and output redirection with `Out-File`.

---

## Classwork 9
*No commands to include*

### Summary:
Even though there were no new commands that I learned here, Classwork 9 focused on playing around with the Task Scheduler and using it to create tasks that we can use and observe through PowerShell.

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
- <img width="930" alt="image" src="https://github.com/user-attachments/assets/d4bed060-50aa-4960-a1e4-04fc81adafd5">


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
- <img width="855" alt="image" src="https://github.com/user-attachments/assets/32649b86-c4b7-4792-9c9b-1abef6f9d73d">


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
- <img width="806" alt="image" src="https://github.com/user-attachments/assets/0f01569e-6924-41fc-9dff-bd813750638e">


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
- <img width="920" alt="image" src="https://github.com/user-attachments/assets/c4e75aae-5a01-4345-bf0a-0a8b8d59fa63">


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
- <img width="847" alt="image" src="https://github.com/user-attachments/assets/1a3d228a-417f-41dd-817e-983982f71ba2">


### Summary:
Lastly, Classwork 10 covered file and printer management using `New-Item`, `New-SmbShare`, `Get-SmbShare`, `Get-Printer`, and `Test-Path` to work with directories, network shares, printers, and file paths.

---


