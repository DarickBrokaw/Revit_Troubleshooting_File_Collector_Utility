Readme: Revit Troubleshooting File Collector Utility

Note: Many of the files gathered are user account specific. Make sure to run this utility on the Windows user account experiencing the issue.

	Usage:
1.	Extract the ZIP file into a folder
2.	Open the folder for the version that you are troubleshooting e.g. 2018.
3.	Double click on the Windows Batch BAT File. E.g. Collector_2018.bat
	Note: If you receive a SmartScreen warning, you can bypass this by clicking More info, and then Run Anyway.
4.	The data will be gathered and Zipped into the following path:
    C:\Autodesk\DiagnosticData
5.  The folder containing the ZIP should open automatically.

Note: If the folder does not open autotomatically, you can browse to the C:\Autodesk\DiagnosticData folder to manually ZIP the files.

Configurable options:
If you need to adjust the folder which the collected data will be written to e.g. due to permission restrictions, open the Variables folder within the version folder and edit the Path.txt file. 

Note: If the path specified in the Path.txt folder does not exist the utility will attempt to create it.

		The following items	are gathered by this utility:
	Revit related items:
		Background Process	Registry keys associated with the Revit Boost::Interprocess are exported for review of the settings defined.
		Cloud Rendering Log These contain information useful for troubleshooting issues with cloud rendering.
		Generative Design	refinery-server-log.txt is gathered with logging information from Generative Design feature.
		Journals			Journal files record actions taken in Revit and provide more information than is seen through the user interface.
		Profile.xml			The Profile.xml file contains information about the customized workspace setup when Revit 2021 and later is first launched.
		Reset Backups		Collect backup items created through reset workflow.
		Revit Add-ins		A directory listing from the Add-in folders.
		Revit.exe.config	If 	Revit is installed in default location The Revit.exe.config file provides information on how Revit will operate. Sometimes this can be modified by 3rd party applications leading to unexpected behavior when applying product updates.
		Revit.ini			The Revit.ini file stores information on user changes made within Revit.
		Revit Registry keys Revit user and system based Registry keys.
		UIState.dat 		The UIState.dat file is a binary file that contains information on UI customization e.g. changes to the Quick Access Toolbar.

		Revit Licensing:
		Revit Licensing Log	e.g. RVT2018ENUAdlm.log.

		Revit Cloud Worksharing Related items:
		A360.log			The A360.log is similar to the Webservices.log.
		Communicator Logs 	This log contains information on Communicator (Depricated).
		Collaboration Cache Directory This shows the names of the files in the Collaboration Cache folder.
		PAC Log				The Personal Accelerator log has information on the PAC activity and can be used in troubleshooting the Collaboration for Revit service.
		PAC Settings		The Personal Accelerator Settings file has information on PAC configuration.
		PAC Activity.json	The Personal Acceloerator Activity.json has information on dumps related to exceeding the cache limits.
		Webservice.log		The Webservices.log contains information on Revit web communications such as logging into an A360 account.

		Revit Server Related items:
		ApplicationHost.config This file stores IIS configuration information and can help in troubleshooting Revit Server.
		DataStorageService.config Model and Local service This file has information on the project and cache paths setup in Revit Server.
		Revit Server Logs	If the utility is run on a Revit Server, then it will gather the Revit Server logs, these contain information on the activity of the server.
		RSN.ini 			This file is used to define the host servers on a Revit Server Network.
		Web.config 			Model and Local service The Web.config stores configuration information for the Revit Server Application within IIS.

	Navisworks related items:
		Navisworks Add-ins		A directory listing from the Add-in folders.

	Autodesk General items:
		Autodesk Install Logs These are logs created when installing software or updates.
		CER data			The Customer Error Reporting system is used primarily for reporting crashes.
		Desktop Connector Logs	The Desktop Connector facilitates certain linking workflows for cloud workshared models, this gathers log information on the utility.
		LoginState.xml		Shows info about logged in user, if user is logged into Revit.

	Windows Related Items:
		DxDiag export		This has information regarding the DirectX graphics system.
		Event Logs		The Windows event logs contain information on the system outside of the Revit application, and can provide insight into system issues.
		FIPS Compliance	Registry keys associated with the Windows FIPS compliance setting this setting can impact applications and cloud services which are not FIPS compliant.
		Fonts				List of Windows installed Fonts.
		Installed Hotfixes	Windows hotfixes can sometimes cause changes in software behavior, this gathers info about installed hotfixes.
		Installed Programs	CSV file created with information on programs installed and versions. This can be used when checking for conflicts with specific applications or versions.
		Localization		Windows Localization settings.
		Network proxy info	This gathers information reported by Windows on Internet Proxies, which can be important for troubleshooting connectivity issues.
		NFO			The NFO file has system information including a list of startup programs, hardware, drivers, and environmental variables.
		Windows Hosts file	This file has information on system level overrides that can affect network communication.