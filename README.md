# Creating-a-Wim-file

Creating a Wim file from a active computer

How to create a Wim file to be set for export to other computers.

Step 1: Get everything before you will need to start witch is a external hard drive or flash drive with enougth storage to have the file stored.

Step 2: Use a clean computer so theres minimal amount or absolutly zero duplicated programs and files.

Step 3: Do a Sysprep on the computer so you can get a generalized image of the computer.

Step 4: Boot the computer in Windows PE and once at Command line enter the following commands.

Here are the commands in order.

DISM /image:C:\ /optimize-image /boot     
DISM /Capture-Image /ImageFile:"D:\Images\image.wim" /CaptureDir:C:\ /Name:image

After you have completed this process you can boot up windows normally check your files and make sure your .wim file is there you are then done.
