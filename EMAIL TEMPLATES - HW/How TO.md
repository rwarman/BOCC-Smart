This is a general document on how to perform certain tasks related to troubleshooting that may be addressed in the troubleshooting tree, however no specific instructions are given on achieving the tasks.

HOW TO UNINSTALL/RE-INSTALL DEVICES FROM THE DEVICE MANAGER 

Membership in the local Administrators group, or equivalent, is the minimum required to complete this procedure. 

Applies To: Windows 7

Uninstall a device

Generally, you do not need to use Device Manager to uninstall a Plug and Play device. Simply disconnect the Plug and Play device from your computer. You might have to restart your computer, however, depending on the type of device.

For more information, see the instructions provided by the manufacturer of your device.

To uninstall a device

1.Open Device Manager.

2.Double-click the type of device that you want to uninstall.

3.Right-click the specific device you want, and then click Uninstall. You can also double-click the device, and then on the Driver tab, click Uninstall.

4.In the Confirm Device Removal page, select Delete the driver software for this device if you also want to remove the device driver package from the driver store.

The Delete the driver software for this device option removes the package from the driver store. It does not remove the currently installed driver for any other operational devices that use the same driver. If you remove the driver from the store, and the device is connected to the computer again, Windows must search for a copy of the driver package in the standard search locations, including possibly prompting the user for media. 

5.Click OK to complete the uninstall process.

When the uninstall process is complete, unplug the device from the computer.

If you are prompted to restart the computer, the removal is not completed and the device might continue to function until the computer is restarted.

To reinstall a Plug and Play device

1.Open Device Manager.

2.Follow the instructions in the preceding procedure to uninstall the device.

3.If you are prompted to restart the computer, follow these steps:

Plug in the device and then restart the computer. The device will be detected and reinstalled after Windows restarts.

Follow any instructions on-screen to complete installation.

If you are not prompted to restart the computer, follow these steps:

In Device Manager, in the Action menu, click Scan for hardware changes.

Follow the instructions on the screen.

NOTE:

Scan for hardware changes will not reinstall a Plug and Play device if a driver is already installed on the computer. If the device has not been uninstalled, Scan for hardware changes will not detect the connection of the device as a change. You must uninstall a Plug and Play device for Windows to start an installation when you connect the device again.

Reinstall a non-Plug and Play device

Reinstall a device only if it is working improperly or it has stopped working altogether. Before you reinstall a device, try to restart your computer and check the device to determine whether it is functioning properly. If it is not, try reinstalling the device.

To reinstall a non-Plug and Play device

1. Open your Windows Device Manager:

Windows XP: 
Start > Control Panel > System > Hardware > Device Manager

Windows Vista/7: 
Start > Control Panel > Device Manager

Windows 8: 
Press the “Windows Key” and “c” on your keyboard > click on Settings > click on Control Panel > Select "Device Manager" from the list
 
Once the Device Manager opens, do you see a yellow exclamation or question mark that says unknown USB device?  If so, we will need to manually install the SMART Devices drivers.

Right click on the “unknown device” and select update driver software. When is says “cannot find hardware, would you like to automatically search or manual search”, select manual search and browse to this location on your computer
 
Windows 32bit:
C:\Program Files>SMART Technologies>Education Software>Drivers
 
Windows 64bit:
C:\Program Files(x86)>SMART Technologies>Education Software> Drivers
 
Follow the prompts to finish installing the drivers. The Windows Device Manager should now properly detect the SMART Device.


HOW TO CHECK ADMINISTRATIVE PRIVILEGES

WINDOWS:

To check if you are logged into Windows 7 as a user with administrative rights, please: 
 
1.open menu Start -> Control Panel

2.open User accounts

3.click "Manage another account"

There will be all user accounts listed on the page. Each account has assigned some status (Administrator, Standard user, etc.). Please make sure that you are logged into Windows under an account with the status "Administrator".

MAC:

1.Log on to your Mac computer with your username and password.

2.Go to the Apple menu in the upper-left corner of the Mac desktop and select "System Preferences" from the drop-down menu.

3.Click on the "Accounts" control panel underneath the "System" heading.

4.Highlight your username from the list of accounts on the left side of the window.

5.Look under the "Password" tab on the right side of the window to find a checkbox labeled "Allow user to administer this computer." If the box is checked, you are currently an administrator on the computer. If it is unchecked, you account has only standard permissions.

HOW TO GRANT ADMINISTRATIVE PRIVILEGES (FOLDER LOCATIONS)

If you add Total Control (we require read and write permissions) to SMART Technologies specific folder locations and registry locations, then your users will be able to properly use their SMART products. 


If you give Full Control to the following locations, and all their contents and subdirectories, then you would have the appropriate permissions:


In the Windows Registry:

 

HKEY_LOCAL_MACHINE\SOFTWARE\SMART Technologies


HKEY_LOCAL_MACHINE\SOFTWARE\SMART Technologies Inc.

 

HKEY_CURRENT_USER\Software\SMART Technologies

 

If your UAC is on, and your computer has a 32 bit processor:

HKey_CURRENT_USER\Software\Classes\VirtualStore\Machine\Software\SMART Technologies\


On 64-bit computers:

HKEY_LOCAL_MACHINE\Software\Wow6432Node\SMART Technologies


HKEY_LOCAL_MACHINE\Software\Wow6432Node\SMART Technologie Inc.


HKEY_CURRENT_USER\Software\WoW6432Node\SMART Technologies.


 If your UAC is on, and your computer has a 64 bit processor:

HKey_CURRENT_USER\Software\Classes\VirtualStore\Machine\Software\Wow6432Node \SMART Technologies\

 

 

Folder Locations:

 

*note: for 64-bit computers change to Program Files(x86)

 

C:\Program Files\Common Files\SMART Technologies

 

C:\Program Files\SMART Technologies

 

MyDocuments\SMART Notebook

 

(XP)

C:\Documents and Settings\<user name>\Application Data\SMART Technologies

 

(Vista/7/8)

C:\Users\<user name>\AppData\Roaming\SMART Technologies\

 

(XP)

C:\Documents and Settings\All Users\Application Data\SMART Technologies

 

(Vista/7)

C:\ProgramData\SMART Technologies

 

(XP)

C:\Documents and Settings\<user name>\Local Settings\Application Data\SMART Technologies Inc

 

(Vista/7/8)

C:\Users\<user name>\AppData\Local\SMART Technologies Inc.\


Finally, ensure you add Full Control to the Windows Temp folder and the User's Temp folder:


C:\WINDOWS\Temp


(XP)

C:\Documents and Settings\<user name>\Local Settings\Temp


(Vista/7/8)

C:\Users\<user name>\AppData\Local\Temp


LOCATING THE SYSTEM PROFILER/SYSTEM INFORMATION ON A MAC 

Apple provides Mac OS X with an all-in-one hardware and software display tool, aptly named Apple System Profiler, which you can find it by clicking on MAC Hard drive (HD) >Applications folder > Utilities. You can also reach the Profiler through the Apple menu. Just click About This Mac and then click the More Info button.

The System Profiler major headings include Hardware, Network and Software. If you wish to see what devices are connected i.e. SMART Boards, Document Cameras etc under Hardware, Click on USB and you will see the connected items.


LOCATE AND START/STOP THE SMART BOARD SERVICE

Windows:
Start > Programs > SMART Technologies > SMART Tools > SMART Settings > About Software and Product Support > Tools > Diagnostics > Service > Start or Stop
 
(On Windows 8, you can open SMART Settings by pressing the “Windows key” and “Q” on your keyboard to bring up a search window. Type “SMART Settings” and select it from the search results.)

MAC:
To Start or Stop the SMART service in the Diagnostics menu from: Finder > Applications > SMART Technologies > SMART Settings (or Control Panel) > About Software and Product Support > Tools > Diagnostics > Service > Start or Stop

PROCEDURE TO GET AND RUN THE SOFTWARE CLEAN UP UTILITY

WIN: https://basecamp.com/1764439/projects/2145113-email-templates/documents/4396026-general-software

MAC: https://basecamp.com/1764439/projects/2145113-email-templates/documents/3651767-general-software

TURNING OFF THE SECURITY SOFTWARE/FIREWALLS

Windows:

1.Open Windows Firewall by clicking the Start button Picture of the Start button, clicking Control Panel, clicking Security, and then clicking Windows Firewall.

2.Click Turn Windows Firewall on or off. Administrator permission required If you are prompted for an administrator password or confirmation, type the password or provide confirmation.

3.Click Off (not recommended), and then click OK.

Mac:

1.Open up System Preferences, which is the icon in your dock with the gears (usually near the far right) or by clicking on the apple menu from the toolbar and selecting system preferences.

2.Click on "Security", which is in the top line of icons.

3.Go to the Firewall tab.

4.Click the small padlock icon in the bottom left-hand corner. Enter your password when prompted.
How to Turn Your Computers Firewall On and Off for Beginners
5.Hit the Stop button to turn the firewall off. If you want to turn it back on later, you can come right back to the same place and hit the Start button.


ADDING SMART BOARD SERVICE TO THE START-UP FOLDER

You can add SMART Board Service to your startup items using msconfig. (Type msconfig in your Windows 7 start menu, then open it from the search results.) Once in msconfig, click on the startup tab and expand the Command column. Look for the entry that ends in "SMARTBoardService.exe -d". If the box next to this entry is unchecked please check it and then restart the computer. Please test to see if the issue is resolved once your computer has restarted.

 

If your startup tab in msconfig does not contain an entry for the  SMART Board Service you can add it to startup using the process below.

 

First navigate on your computer to your SMART Technologies folder:

 

32-bit Windows:

C > Program Files > SMART Technologies > Education Software

 

64-bit Windows:

C > Program Files (x86)> SMART Technologies > Education Software

 

Look for the executable file named “SMARTBoardService”. It has an icon with the wrench and screwdriver, not the logfile with the same name. You’ll want to right click on it and choose “create shortcut”. You can now drag this shortcut to your Startup folder. To open your startup folder, click Start > All Programs (or Programs), and locate the folder named “Startup”. Right click on it and choose open. Right click on the shortcut after you have moved it to the startup folder. Click on the Shortcut tab and locate the Target field. You will need to add a space after the end quote at the end of the file path and then type "-d" without quotation marks. Your entry should look like the following:


"C:\Program Files\SMART Technologies\Education Software\SMARTBoardService.exe" -d


After you finish this process please restart your computer and test to see if the issue has resolved. 

IDENTIFYING USB 3.0 PORTS ON YOUR COMPUTER

Easy way to identify a USB  port is to peer inside and check what colour the connecting part inside is.

 

USB 3.0 are coloured Blue.

USB 2.0 are coloured Grey

IDENTIFYING USB 2.0 PORTS ON YOUR COMPUTER

 Windows XP

    On the Start menu, right-click on My Computer.
    From the shortcut menu, click Manage.
    Click Device Manager.
    Double-click Universal Serial Bus controllers.
    Look for any USB controllers labeled as "Enhanced" or "High Speed". These will be the USB 2.0 ports on the computer. USB controllers without these designations are USB 1.0.

 

 

Windows Vista

    On the Start menu, right-click on Computer.
    From the shortcut menu, click Manage.
    Click Device Manager.
    Double-click Universal Serial Bus controllers.
    Look for any USB controllers labeled as "Enhanced" or "High Speed". These will be the USB 2.0 ports on the computer. USB controllers without these designations are USB 1.0.

 
If you have a Mac running OS X v10.6.x Snow Leopard or later

All Macs supported to use Mac OS X v10.6.x Snow Leopard or later have at least one built-in USB 2.0 port.


If you have a Mac running OS X v10.5.x Leopard or earlier

    Click the Apple menu and choose "About this Mac".
    Click the More Info button. System Profiler should open.
    Select USB from the left column.
    Look in the right column under USB Device Tree. If you see USB High-Speed Bus in any of the left-most entries, your Mac has USB 2.0 ports. See this example:

    If you see only USB Bus in the left-most entries, your Mac has USB 1.1, and does not have USB 2.0 ports. See this example:

 

______________________________________________________________

Tags (DO NOT COPY): EMT