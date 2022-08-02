> **Blog Post:** [https://blakedrumm.com/blog/scom-dw-grooming-tool/](https://blakedrumm.com/blog/scom-dw-grooming-tool/) \
> **Quick Download:** [https://aka.ms/SCOM-DW-Tool](https://aka.ms/SCOM-DW-Tool)

[![Visits Badge](https://badges.strrl.dev/visits/blakedrumm/SCOM-DW-Grooming-Tool)](https://badges.strrl.dev) \
[![Latest Version](https://img.shields.io/github/v/release/blakedrumm/SCOM-DW-Grooming-Tool)](https://github.com/blakedrumm/SCOM-DW-Grooming-Tool/releases/latest) \
[![Download Count Latest](https://img.shields.io/github/downloads/blakedrumm/SCOM-DW-Grooming-Tool/latest/SCOM-DW-GroomingGUI-EXE-64bit.zip?style=for-the-badge&color=brightgreen)](https://aka.ms/SCOM-DW-Tool)

![SCOM DW Grooming Tool](https://user-images.githubusercontent.com/17127926/176571271-6cd1f5f1-7ab4-40ac-8498-0bc8f5a2089f.png)

## Introduction

This tool can be used to modify the System Center Operations Manager Data Warehouse Grooming retention days, allows you to see grooming history, you can manually run grooming, and you may also export the current configuration so you can keep a backup of your settings. You have the option of resetting the values to Defaults for the typical data sets in the Data Warehouse.

## How to Use

You have multiple ways to run the SCOM DW Grooming GUI Tool:

1. Download and install the MSI: [MSI Download](https://github.com/blakedrumm/SCOM-DW-Grooming-Tool/releases/latest/download/SCOM-DW-GroomingGUI-MSI.zip)
2. Download and run the EXE: [EXE Downloads](https://github.com/blakedrumm/SCOM-DW-Grooming-Tool/releases/latest/download/SCOM-DW-GroomingGUI-EXE-64bit.zip)
3. Download or Copy the Powershell Script: [Powershell Script](https://github.com/blakedrumm/SCOM-DW-Grooming-Tool/releases/latest/download/SCOM-DW-GroomingGUI.ps1)

You will need to provide the Data Warehouse DB Server Name or Address, and the Data Warehouse Database Name. The script may auto detect these variables from the local registry on the machine you are running the script. To get started, you will need to press the **Get Current Settings** button. This will allow the script to gather the information from the Data Warehouse database server. Once you make the changes you can save the change with **Set**.

This script will log some actions to the Application Event Log. Look for the Event Source: `SCOMDWTool`

## More Information

You will get prompted each time you run the script to accept the license agreement, unless you select do not ask me again, when you select this it will save a file to your ProgramData Directory:
```
C:\ProgramData\SCOM-DataWarehouseGUI-AgreedToLicense.log
```

<!-- ![Visits](https://counter.blakedrumm.com/count/tag.svg?url=https://github.com/blakedrumm/SCOM-DW-Grooming-Tool) -->
