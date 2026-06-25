# Wazuh SIEM Security Lab - Commands

This document contains the important commands used during the setup and
verification of the **Wazuh SIEM Security Lab**.

------------------------------------------------------------------------

## 1. Update Ubuntu

``` bash
sudo apt update && sudo apt upgrade -y
```

------------------------------------------------------------------------

## 2. Check Wazuh Manager Status

``` bash
sudo systemctl status wazuh-manager --no-pager
```

------------------------------------------------------------------------

## 3. Check Wazuh Indexer Status

``` bash
sudo systemctl status wazuh-indexer --no-pager
```

------------------------------------------------------------------------

## 4. Check Wazuh Dashboard Status

``` bash
sudo systemctl status wazuh-dashboard --no-pager
```

------------------------------------------------------------------------

## 5. List Registered Agents

``` bash
sudo /var/ossec/bin/agent_control -l
```

------------------------------------------------------------------------

## 6. Check Wazuh Agent Service (Windows)

``` powershell
Get-Service WazuhSvc
```

------------------------------------------------------------------------

## 7. Check Sysmon Service

``` powershell
Get-Service Sysmon64
```

------------------------------------------------------------------------

## 8. View Recent Sysmon Events

``` powershell
Get-WinEvent -LogName "Microsoft-Windows-Sysmon/Operational" -MaxEvents 10
```

------------------------------------------------------------------------

## Expected Result

-   Wazuh Manager: **Active (running)**
-   Wazuh Indexer: **Active (running)**
-   Wazuh Dashboard: **Active (running)**
-   Windows Wazuh Agent: **Running**
-   Sysmon: **Running**
-   Agent visible in Wazuh Dashboard
-   Vulnerabilities detected successfully
