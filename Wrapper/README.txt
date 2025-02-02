File: README.TXT for 'Sophia Script Wrapper v2.0' created by https://benchtweakgaming.com/2020/10/10/windows-10-debloat-tool/
Created for farag2 Windows 10 Sophia Script: https://github.com/farag2/Windows-10-Sophia-Script

INTRODUCTION
------------
Please read this document to understand how to use this program.

BenchTweakGaming.com now works with the farag team.

This program create a PowerShell script file that you can run to tweak/'Debloat' Windows 10 based on farag2 
Windows 10 Sophia Script. It serves as a front-end GUI for the Sophia script (Wrapper).

The options are arranged in different tabs and there is a Default preset in the menu so you can debloat a 
set of options. You can choose the Default preset first and then add your own choices. You can also create your own 
Sophia script to share and open it up. There are ToolTips balloon message popups for detailed info for each item.

After choosing your options you can directly run the PowerShell script from the program after creating your script. 
To do so, open up 'Sophia.ps1' preset, this also gets the path for files to run directly, then fill in your combobox 
choices, click the ‘Output PowerShell’ button and then click ‘Run Powershell’ button. The “Run PowerShell” button 
creates a PowerShell script called ‘Sophia_edited.ps1’ in the same directory and runs it.

OR save the PowerShell script as 'Sophia.ps1' with the farag2 Sophia files (see heading FILES below) 
and run it using the following commands.

Launch PowerShell (Run as administrator) and navigate to where your script is.

1. Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process -Force
2. ./Sophia.ps1

FILES
-----
There needs to be 6 files for this program to run properly. The txt files are stored in a folder 'Config'.

►Sophia Script Wrapper.exe : The GUI program.
►data.txt : Contains the options (function names) to select from (usually only 2 options that something is Enable or Disable or ‘LeaveAlone’).
Notice the sections ‘#region Xxx’ and how a semi colon separate the function commands. The last command option in each section does not have a semi colon.
Add or substract from the set.
►dataltsc.txt : LTSC version of data.txt
►default.txt : Contains Default preset to debloat. Click this preset from Option menu in program.
►tooltip.txt : Contains ToolTips for each combobox item. In English.
►README.txt : This documentation.

INSTRUCTIONS
------------
UNZIP all the files and open the 'Sophia.ps1' file to import your preset and to get the path for files to run.
If you do not open 'Sophia.ps1' then you can not run directly the PowerShell script you create and must run 
your script manually via PowerShell command line in console.

►Sophia.ps1 :			farag2 Original Windows PowerShell Script.
►Sophia.psd1 :			farag2 Windows PowerShell Data File
►Sophia.psm1 :			farag2 Windows PowerShell Script Module
►Functions.ps1 :		farag2 Windows PowerShell Script to run functions with tab autocompletion

The 'Localizations' folder contains folders that are localized language files for prompts during the PowerShell 
execution each with a PowerShell Data File 'Sophia.psd1'.

►cn-CN
►de-DE
►en-US
►es-ES
►fr-FR
►hu-HU
►it-IT
►ru-RU
►tr-TR
►uk-UA