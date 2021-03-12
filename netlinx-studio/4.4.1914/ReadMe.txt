Release Notes: NetLinx Studio 4
Version......: V4.4
Build........: 1914
Date.........: 10/18/2019

----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
         What's New for NetLinx Studio - Version 4.4 (October 2019 Hotfix)        
----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
BUG FIX: Fix crash when sending firmware via ICSP

----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
         What's New for NetLinx Studio - Version 4.4 (August 2019 Hotfix)        
----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
BUG FIX: Fix loading of large firmware files.

NEW FEATURE: Changed text editor write technology to support fonts with ligatures
and improve text rendering.

NEW FEATURE: Add ability to use spaces for indentation. See Editor-Display and 
Indentations under Preferences (1)

UPDATE: Added ability to select font weight. (2)

Notes:
(1) Only new indentations are affected after updating this option. Opened documents
    must be reloaded (closed & re-opened) for this to take affect.
(2) Not all font weights are supported. This is a limitation within the text renderer
    and Windows, not within Studio itself.

----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
         What's New for NetLinx Studio - Version 4.4 (May 2018 Hotfix)        
----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
BUG FIX: Increase the length of total characters sent from Control a Device dialog
From 120 to 1024.

Note: The maximum length of a single line in 1024 characters. Attempting to
      create a line greater than this will result in a second line and will be 
      sent as a separate string/command. 




----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
         What's New for NetLinx Studio - Version 4.4 (April 2018 Hotfix)        
----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
NEW FEATURE: Added NetLinx String Expressions to the notifications and diagnostics
view. Visit the Preference dialog for settings.

NEW FEATURE: Added the option to copy the value of the selected line which
excludes the line number and timestamp in the context menu of Notifications and
Diagnostics.

UPDATE: The URL list will now display more detailed information regarding 
authenticated connections and their state (Authentication Pending, Authentication
Failed, or Credentials required but not found)

UPDATE: Change parameter names of functions in Netlinx.axi to allow autocomplete
to be more descriptive.

FEATURE REQUEST: Add ability to cancel, retry or continue a batch file transfer when a
touch panel is locked by TPD4 or TPD5.

FEATURE REQUEST: Add ability to change font and size for all output bar windows and debugger.

BUG FIX: Problem when certain CUSTOM_EVENT messages are displayed in the
notification tab resulting in a crash has been corrected.

BUG FIX: Display the proper context menu when tabs are reordered in the output bar

BUG FIX: Correct an issue where displaying multiple topics to choose from when pressing 
F1 with a highlighted keyword could cause NetLinx Studio to freeze. This fix also prevents 
the help window from being the topmost window with NetLinx Studio.

----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
                   What's New for NetLinx Studio - Version 4.4
----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
NEW FEATURE: Ability to connect NetLinx Studio via TLS/SSL to AMX Controllers that
have ICSP security enhancement firmware (V1.5 and greater).  Please visit the 
Communications Settings dialog for more information.

NEW FEATURE: Added a "Certificate Manager" to manage the AMX Controller's public
and private keys via Certificates.  Option is located under the "Tools" menu.

FEATURE REQUEST: Added a "Bulk Firmware Transfer" mode-less dialog that has the 
ability to send a KIT Firmware file to multiple devices sequentially with one click 
of a button. This feature is located in the context menu for the Online Tree and 
under the "Tools-Firmware Transfers-Bulk Firmware Transfer..." menu item.

FEATURE REQUEST: Added a "Communications Settings" button to the Firmware Transfer
dialog so the user can change the communication settings without closing and then
revisiting the dialog with a different Communication settings.

FEATURE REQUEST: Added the ability to display a "Date Stamp" in the Notifications
and Diagnostics display logs.  Visit the Preference Dialog for settings.

FEATURE REQUEST: Added a "Emulate Custom Event" dialog so the user can emulate
a Custom Event message from a device.  This feature is locate under the 
"Diagnostics" menu item.

FEATURE REQUEST: Added the ability to change all the Connection Settings within
the File Transfer dialog to the current Active System's connection setting.

FEATURE REQUEST: Added the ability to change multi-selected File Transfer items 
connection settings within the File Transfer dialog via the Communications 
Settings dialog.  

FEATURE REQUEST: When saving your File Transfer Dialog list of items to an .FTL
file, you now have the ability to select to save the file names as 
"Relative Path" instead of the fully qualified file name.  The relative path
files names are relative to the directory where the .FTL file is saved by 
the user. 

UPDATE: Updated NetLinx.AXI file with the following new functions:
               AUTHENTICATE
               AUTHENTICATE_CERTIFICATE
               SSH_CLIENT_CLOSE
               SSH_CLIENT_OPEN
               TLS_CLIENT_CLOSE
               TLS_CLIENT_OPEN
Please visit the NetLinx Studio Keyword Help file for additional details.

UPDATE: In the Network Connections dialog, when you Edit or create a New IP
entry, that entry will now be selected within the dialog.

UPDATE: When Importing an Exported AXW file and you have duplicate files within a
System, the program will continue to load the Workspace after the Warning Messages
instead of stopping the loading process.

BUG FIX: The problem with launching the Keyword Help file locking up the program
has been corrected.

BUG FIX: Reoccurring problem with the Workspace Tree not showing the proper
Device Mappings for various files within the Tree is now corrected.

BUG FIX: Problems launching the TPDesign5 application from the Workspace Tree
has been corrected.

BUG FIX: Problems with the editor not code folding the WAIT sections of NetLinx
code has been corrected.

BUG FIX: Ability to drag-and-drop Driver Design Files (.xdd) into the Workspace 
tree.  They will be loaded into the Module folder.

BUG FIX: Problems with the Export/Import Preferences file have been corrected.

BUG FIX: Misbehaving Asynchronous Notifications messages from unwanted devices 
when turning on the Notification Messages data stream has been corrected.
 
BUG FIX: When selecting files from the "Add" dialog within the File Transfer 
dialog, the File Tree is sorted the same way as the Workspace listing within
the application.

BUG FIX: The ability to "Verify TKN on NetLinx Master" is now working when the 
Workspace does not have the Main.axs source code file, but only a TKN file in
the Workspace.


----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
                   What's New for NetLinx Studio - Version 4.3
----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
FEATURE REQUEST: Import/Export IP Address lists from the Network tab of the
Communications dialog.

FEATURE REQUEST: Transfer a single file to multiple masters via the 
"File Transfer-Add Individual Files" dialog.

FEATURE REQUEST: Communications dialog enhancements:
  - Display last tab visited upon activation of the dialog.
  - Sort last selected column when visiting the Network tab.

FEATURE REQUEST: Default the System Number for the NetLinx Notifications Options
dialog to the connected System.

FEATURE REQUEST: Added the "Enable _WC Preprocessor" (Wide Character Preprocessing) 
command to the Configuration file used by the NLRC.EXE program (NetLinx Compiler 
Command Line Program). For more Information,  please read the RunNetLinxCompiler.doc 
file located in C:\Program Files (x86)\Common Files\AMXShare\RunNetLinxCompiler. 

UPDATE: New Online Tree icons with more descriptive appearance.

UPDATE: Added the ability to code-fold on WAIT code blocks.

BUG FIX: Expanded the virtual viewing of the NetLinx Diagnostics/Notification
panes to more than 200 characters per line.

BUG FIX: Various Find/Replace Regular Expression reported problems. 

----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
                  Known Issues with NetLinx Studio - Version 4.3
----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
The NetLinx compiler does not recognize UNC (Universal Naming Convention). The
compiler cannot resolve the network resource or shared file when linked via a 
UNC path (as an example): 

             \\Server\Volume\File

As a workaround, map a drive letter to the Network drive, re-assign/open via that 
drive letter so that it can be recognized by the NetLinx compiler.



----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
                   What's New for NetLinx Studio - Version 4.2
----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
UPDATE: New Installer program for NetLinx Studio application.

UPDATE: Defaulted the file filter for the "Add to User Interface" folder to be
TP4/TP5 Files (*.tp4;*.tp5).

UPDATE: In support of the new "Listview Buttons and Dynamic Data Feeds" enhancements
for the Modero G5 Touch Panels, the NetLinx.AXI and NetLinx Studio Keyword Help 
files have been updated. Please visit the NetLinx Studio Keyword Help file for 
additional information and examples.

UPDATE: Added back in the Port Assignment in the Status Bar for IP connections.

FEATURE REQUEST: For HTTP Firmware File Transfers, the user now has the ability
to select which NIC is used for transfer when they have more than one NIC installed 
on their PC.

FEATURE REQUEST: Share Communications IP Connection History with the TELNET 
Communications selection dialog.

FEATURE REQUEST: Added the ability to override the Code Wizard's code insertion
process by allowing the user to insert generated code at the current cursor 
location.


BUG FIX: Problems with creating the temporary files needed for the TELNET
session have been corrected.

BUG FIX: Removed the Device ID Range check when the user selects to transfer
Firmware Files via the Online Tree menu option.

BUG FIX: Corrected some missing preferences when the user selected the Exports 
Preferences option.

BUG FIX: DIPSwitch program installation problems on Windows 7/8 Platforms have
been corrected.

BUG FIX: The problem of missing TKN files when Exporting the Workspace has 
been corrected.

BUG FIX: In the Online Tree context menu for Device IDs from 1 to 256, the 
user now has the ability to select either an AxLink or NetLinx type 
Firmware Transfer.

BUG FIX: Various irritating File Transfer Dialog problems have been corrected.


----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
                   What's New for NetLinx Studio - Version 4.1
----------------------------------------------------------------------------------
----------------------------------------------------------------------------------
FEATURE REQUEST: File Transfer -- When selecting to "Receive" Non-System, JAR or
XDD files from the master, the user will now be presented with a directory listing 
of these files that are located on the master to select.

FEATURE REQUEST: Increased the maximum Token/Variable limit from 100,000 to 
200,000 for the NetLinx Compiler.

FEATURE REQUEST: After stopping a debug session, leave the Debug Output Window
displayed.  Please visit the NetLinx Compiler Preference page for options.

FEATURE REQUEST: When starting a debug session, have the option to whether or not 
to display the Main.AXS file in the editor.  Please visit the NetLinx Compiler 
Preference page for options.

FEATURE REQUEST: Auto-start scanning for master controllers when activating the 
"Listen for Masters" dialog.

UPDATED FEATURE: Updated the Help Menu link for the official release of AMX-PI2 on 
the AMX web site.
 


BUG: Display correct error message when user enters an invalid Host Name in the 
Network Address dialog.

BUG: Corrected sporadic "Ping Master before Connect" problems for IPv4 and
IPv6 communications.

BUG: Updated the Apple Link for downloading the latest Bonjour Services required
for the Zero-Config tab.

BUG: Reactivated all Diagnostic menu items when a connection is using a Virtual
NetLinx Master.

BUG: Activated code folding on the CUSTOM_EVENT programming block.

BUG: Corrected the Total Event Count calculation when using the Code Wizard to
generate a range of events.

BUG/FEATURE REQUEST: Changed the command line parameters when using a Configuration
file with the NLRC.EXE program (NetLinx Compiler Command Line Program). Please 
visit the C:\Program Files (x86)\Common Files\AMXShare\RunNetLinxCompiler 
directory for more information.


---------------------------------------------------------------------------------
---------------------      Discontinued V3.X Features     -----------------------
---------------------------------------------------------------------------------
The following features will no longer be supported with NetLinx Studio V4.0:

 * File Transfers for G3 Panels (TPD files).
 * File Transfers for Mio Keypads (KPD Files).
 * File Transfers to Axcent Masters (TOK Files).
 * The Axcess Compiler will be not be installed.



---------------------------------------------------------------------------------
---------------------        V3.4 vs V4.X APW Items       -----------------------
---------------------------------------------------------------------------------
With the V4.0 release of NetLinx Studio, the program will now handle the USB 
connections and IPv6 protocols that are available with the new NX-x200 series 
masters, along with the new file transfer capabilities. The APW that is saved by
NetLinx Studio V4.x has been adjusted to handle these new settings. 

All V3.x transport settings will be read in and “preserved” in a V4.x APW file. 
Any USB/IPv6 transport settings saved in V4.x will NOT be seen if you open the
APW file in V3.x of NetLinx Studio, but you will see your original V3.x settings.

Consequently, reading a V4.x APW file with a NetLinx Studio V3.x application will 
have some side-effects.  Any Master Directory settings specified for your 
Non-System file transfers will be lost if you saved the V4.x APW file back to 
a V3.x APW file.  

Since NetLinx Studio V4.x has discontinued support for Axcent Masters along with
KPD, TPD, and TOK file transfers, the V4.x APW will NOT attempt to keep this 
items within your APW file.  The user will be warned about what is being removed 
and will have the option of canceling the opening of the V3.x APW file.

It is recommended that the user should do a “Save As Workspace…” when they have 
read in a V3.x APW to preserve a copy in the event of any problems.



---------------------------------------------------------------------------------
--------      Known Issues with the USB Gadget Driver Installation       --------
---------------------------------------------------------------------------------
As you can connect to the front USB port of the new NX-x200 series master 
controllers to use as the "program port", the USB driver may not load properly.
Therefore, the master may not show up in the USB tab of the Communication Settings
dialog.

Please read the USBGadgetDriverInstallationNotes.docx file located in:

   C:\Program Files (x86)\AMX Control Disc\NetLinx Studio 4\USBGadgetDriver

for additional information on installing the USB driver required to communicate 
with the NX-x200 Series Controllers via the USB Program Port.



