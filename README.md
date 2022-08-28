# Intune
A list of Intune scripts to be used in the Microsoft Endpoint Manager.

# Printers 
Deployment, Detection & Removal of TCP/IP Printers. Driver INF, Catalog and INI files are added to a ZIP file under a folder called Driver.
E.g.

Driver\MB5100P6.INF

This unzips & installs the driver, creates a named printer TCP/IP Port and finally, a print queue. The detection script is uploaded to MEM and you can call the uninstall script for printer removal. This allows complete printer management without a centralised print server.

Unfortunately, you cannot deploy secure print/printer defaults to the printer, however some driver vendors allow you to remove colour from the driver by repackaging e.g. Ricoh. Typically, this will require a managed print service.
