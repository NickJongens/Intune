# Intune
A list of Intune scripts to be used in the Microsoft Endpoint Manager.

# Printers

## Why?
At my workplace, we've found a need to deploy printers via Intune/MEM without using Azure Universal Print. The job count for Azure Universal Print is severly restrictive unless you pay a reasonable sum per month to be able to print. This should not be the case. This also becomes harder if you're not using Microsoft 365 Business Premium licenses as there's no print allocation provided. Maybe you want to use Intune, or maybe you want to include printer deployment into an onboarding process - you should have options!

## More Info!

Deployment, Detection & Removal of TCP/IP Printers. Driver INF, Catalog and INI files are added to a ZIP file under a folder called Driver.
E.g.

Driver\MB5100P6.INF

This unzips & installs the driver, creates a named printer TCP/IP Port and finally, a print queue. The detection script is uploaded to MEM and you can call the uninstall script for printer removal. This allows complete printer management without a centralised print server.

Unfortunately, you cannot deploy secure print/printer defaults to the printer, however some driver vendors allow you to remove colour from the driver by repackaging e.g. Ricoh. Typically, this will require a managed print service.
