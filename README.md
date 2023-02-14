# X10ManagerDesktop

Copyright (c) February 2006 trekkerphotoart.com

Document Date: February 11, 2023

Document Author: Alan Wagner

X10ManagerDesktop and X10Manager (command line)

Manage Schedules and their Events for X10 Controllers and Devices

Project developed using:
- X10ManagerDesktop
	- Microsoft Visual Studio Community 2017
	- Microsoft .NET Framework Version 4.8
- X10Manager (command line)
	- Microsoft .NET Framework Version 4.0.30319

======================================================

Specifications:

- Supported X10 Controllers:
	- CP290 X10 Home Control Interface
	- CM11A X10 2-Way Computer Interface
	- CM15A X10 ActiveHome Pro

- Operating System:
	- Microsoft Windows 8, 8.1 or 10 (32 bit or 64 bit)
	- Windows Server 2019 (64 bit)
	
	Notes:
		
		1)	Microsoft .Net Framework Version 4.x is needed for X10Manager (command line).
		
		2)	X10 USB ActiveHome (ACPI-compliant) driver is needed for CM15A Controller.
			The driver can be found in compressed zip archive “C:\X10Manager\X10_USBWindows_v6.0.0.210.zip”.
			Usually Windows 8, 8.1 or 10 will plug-n-play the driver as a powered-up CM15A controller
			is connected to a USB port.
			For Windows Server 2019, the driver will have to be installed.

- "Adobe Reader" or "Adobe Acrobat" is needed to read file X10ManagerDesktop_OperationsManual.pdf which contains the "X10ManagerDesktop Operations Manual" document.
  "Adobe Reader" or "Adobe Acrobat" can be found at:
  		
		https://www.adobe.com/accessibility/products/reader.html
		
		https://get2.adobe.com/reader/ 

- Computer Interface:
	- For each CP290 Controller: RS-232 Port (600 baud, 8 data bits, no parity, 1 stop bit, no flow control)
	- For each CM11A Controller: RS-232 Port (4800 baud, 8 data bits, no parity, 1 stop bit, no flow control)
	- For each CM15A Controller: USB Port (1.1, 2, 3)

======================================================

1st Time Quick Start:

1) Extract folder "X10ManagerDesktop_Installer" from X10ManagerDesktop_Installer_Release.zip to "C:\X10ManagerDesktop_Installer"
2) "Run as administrator" ImportCert_X10ManagerDesktop_Installer.cmd
3) Install X10ManagerDesktop_Installer.msi

++++++++++++++++++++++++++++++++++++++++++++++++++++++

Quick Start Notes:

	A) If already running an earlier version:
		1) Backup database BEFORE removing earlier version.
		2) After successful instalation of this version, Restore backup made in step A-1.
	
	B) Refer to section "X10ManagerDesktop Operations Manual" - "Remove Installation" - "Preserve Files and X10 database" 
	   regarding steps for database Backup and Restore.
	
======================================================

Notes:

1)	A normal X10ManagerDesktop and X10Manager (command line) installation will create new folders in the following locations:
	- C:\X10ManagerDesktop_Installer
	- C:\Program Files (x86)\trekkerphotoart.com\X10ManagerDesktop_Installer
	- C:\X10Manager
	Note: Existing folders and their contents will be replaced.
	
2)	"C:\Program Files (x86)\trekkerphotoart.com\X10ManagerDesktop_Installer" contains files needed for operation of X10ManagerDesktop.
	- When a Repair or Remove Installation is performed, this folder and its contents are removed.
	- A Repair Installation will re-create this folder and its contents.
	Note: Do not add or modify files in this location.
	
3)	“C:\X10Manager” contains files needed for operation of both X10ManagerDesktop and X10Manager (command line).
	- When a Repair or Remove Installation is performed, this folder, its subfolders and its contents are removed.
	- With a Repair Installation, the core files and some support command scripts (.cmd) are re-created.
	Note: Before a Repair or Remove is performed, review "Preserve Files and X10 database" section in the "X10ManagerDesktop Operations Manual".

4)	Detailed information regarding Installation, Repairing the Installation, Removing the Installation,
	and Preserving Command Script files and X10 Access database can be found in the "X10ManagerDesktop Operations Manual".
	
5)	X10Manager (command line) and the Access Database (X10Db.mdb) used by X10ManagerDesktop and X10Manager (command line) are typically located at "C:\X10Manager".

6)	The Access Database "X10Db.mdb" must be in the same folder with "X10Manager.exe" and its program support files 
	"X10Manager.exe.config, ParadoxReader.dll, X10Include.dll, X10IncludeCM.dll".
	
7)	Detailed information about X10ManagerDesktop and X10Manager (command line) can be found in "X10ManagerDesktop Operations Manual".

8)	Information regarding installation, setup and operation of X10 Controllers and X10 Modules is not covered in "X10ManagerDesktop Operations Manual".

======================================================

Licensing:

Copyright (c) February 2006 trekkerphotoart.com
This entire project (including and not limited to Documentation, Images, Executables, Libraries and Scripts) is Licensed under the "CREATIVE COMMONS PUBLIC LICENSE (CCPL)".
The "CCPL" can be found in "X10ManagerDesktop Operations Manual", "Licensing" section.

======================================================

Credits:

ParadoxReader.DLL (ParadoxReader) contains source code from, "Code Project", "Paradox database native .NET reader" by Petr Bříza, March 17, 2011, v1.2.
Modifications have been added by Alan Wagner that allow ParadoxReader, as used in X10ManagerDesktop and X10Manager, to read X10 Lighthouse Scene BLOB data.
Original ParadoxReader source code is Licensed under: "The Code Project Open License (CPOL) 1.02"
The "CPOL" can be found in "X10ManagerDesktop Operations Manual", "Appendix", "The Code Project Open License (CPOL) 1.02" section.

======================================================
