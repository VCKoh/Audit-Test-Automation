# Word 2016 Audit

based on
* _DISA Microsoft Word 2016 Security Technical Implementation Guide V1R1 2016-11-14_

## Overview

The `Word2016Audit`-Module benchmarks the current Microsoft Word 2016 settings with current hardening standards from DISA.

## Requirements

Please make sure that following requirements are fulfilled:

* **Microsoft Word 2016**
* **ATAPHtmlReport Module:** This module is used for the html report generation and is [included](../ATAPHtmlReport) in the Audit Test Automation Package. Follow the instructions at the link to install the module.

### Loading the Word 2016 Audit module

You only need to import the module when you haven't installed it.

1. Download the release zip and export the modules in a location you can easily access with PowerShell
2. Navigate to the location with PowerShell and import the modules with `Import-Module`. For example:
```Powershell
cd .\Desktop\
Import-Module -Name .\Audit-Test-Automation\Word2016Audit -Verbose
```
3. Generate a report with `Get-Word2016HtmlReport` For example:
```PowerShell
Get-Word2016HtmlReport -Path "reports/report.html"
```

## Sample report

You can find a sample report in the [Sample](Sample) folder.