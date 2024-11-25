# Creating-a-Wim-file
Creating a Wim file from a active computer
How to create a Wim file to be set for export to other computers.

Step 1: Get everything before you will need to start witch is a external hard drive or flash drive with enougth storage to have the file stored.

Step 2: Use a clean computer so theres minimal amount or absolutly zero duplicated programs and files.

Step 3: You should do a Sysprep on the computer as a saftey measure just in case if something goes wrong to make sure everything goes as smooth it can go.

Step 4: After the Sysprep start by typing "Control Panel" in the Windows search bar, then get to "System and Security"

Step 5: Once you get here then select "Backup and Restore (Windows 7)" yes it says Windows 7 it works with Windows 10 and 11 so dont worry.

Step 6: Select "Create a system image" after that make sure your external hard drive or flash drive is connected.

Step 7: Boot the computer in Windows PE and once at Command line enter the following commands.

Here are the commands in order.

DISM /image:C:\ /optimize-image /boot     
DISM /Capture-Image /ImageFile:"D:\Images\image.wim" /CaptureDir:C:\ /Name:image

After you have completed this process you can boot up windows normally check your files and make sure your .wim file is there you are then done.
