# 🔐 Windows Log Analysis with PowerShell

---

## Overview

This project demonstrates how to perform **basic cybersecurity monitoring and log analysis** using PowerShell on Windows systems. 

The goal was to:
- Automate the process of scanning Windows Event Logs
- Extract all **Error-level events** from the Application log
- Export the results into a text file for reporting or further analysis

This project is perfect for:
- Beginner cybersecurity students learning Windows internals
- Anyone interested in log analysis, incident response, or SOC analyst tasks
- Demonstrating PowerShell skills for automation and cybersecurity use cases

---

## Project Goals

✅ Automate security monitoring tasks  
✅ Learn to filter logs by severity  
✅ Practice exporting results to external reports  
✅ Build practical PowerShell skills for cybersecurity

---

## How It Works

The PowerShell script:
- Reads the **Application log** using the `Get-WinEvent` cmdlet
- Filters only events where:
  - `LevelDisplayName` is `"Error"`
- Formats the details into readable text
- Saves the output to `application_errors.txt` in the same folder as the script

---

## Usage

> **Important:** Run PowerShell as Administrator for permission to read system logs.

---

### How to Run the Script

1. Open PowerShell as Administrator:


2. Navigate to your project folder:

```powershell
cd "C:\Users\anjal\OneDrive\Documents\windows-log-analysis"
.\get-application-errors.ps1
