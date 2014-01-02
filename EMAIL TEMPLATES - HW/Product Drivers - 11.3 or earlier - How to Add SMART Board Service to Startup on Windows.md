

Inbound email summary: Customer experiencing issue where SMART Board Service does not run on startup. Customer has to manually run connection wizard after each restart.

Steps Taken/Results Summary: Advised to make sure SMART Board Service is checked in msconfig. Provided instructions on adding SMART Board Service to startup folder if they do not have an entry for it in msconfig.

Next steps: n/a

Email Template:

(I understand that in order to establish a connection to your SMART Board® interactive whiteboard, you need to launch the Connection Wizard or Firmware Updater each time you restart your computer. I apologize for any inconvenience this may have caused. I am happy to help.)

 

From your description, it sounds like the SMART Board Service may not be launching at startup. To check for this, please restart or relog onto a computer so that you lose your connection to the SMART Board interactive whiteboard. Open Task Manager (right click on your taskbar and select “Task Manager”). Once Task Manager opens, select the “Processes” tab, and then check if the SMARTBoardService.exe is listed.  If it is not listed this means it is not running.

 

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


(Let us know if your issue persists upon following the above instructions.

                                                                                   

For further reference your support incident number is XXXXXXX.

If you have any further questions or concerns, please contact us again.)


Tags (Do Not Copy):

EMT , smart board service , does not run on startup , connection wizard , flashing green , login , restart 
