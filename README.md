# 🔐 Windows Log Analysis with PowerShell

## Overview
This project demonstrates basic cybersecurity analysis using PowerShell to inspect Windows event logs. I built a script that extracts **Error-level events** from the Application log and saves the results to a text file for further investigation.

---

## How It Works

✅ The PowerShell script:
- Searches the **Windows Application log**
- Filters only events where `LevelDisplayName` equals `"Error"`
- Saves the results into `application_errors.txt`

Run it like this in PowerShell (as Administrator):

```powershell
.\get-application-errors.ps1
