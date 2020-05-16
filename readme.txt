PS3 OFW 4.82 NAND/NOR Downgrader v1.0

Courtesy of:
W (Javascript, Research & Testing)
esc0rtd3w (Debugging, Research & Testing)
bguerville (ROP Chaining/Javascript & Debugging)
Habib (ROP Chaining & Debugging)

More Info at: http://www.psx-place.com


######################################################################################################
BRICK WARNING!!!
You have to make sure the correct flsh.hex file is on the flash drive and in the far right USB slot!

4.82 flsh.hex MD5: 8e156c99101bf36ec3edb832982ae46d
######################################################################################################


=================================================================================================================
PLEASE READ FIRST:
It's essential not to flood the browser memory with junk before running the exploit. The reason for this is that due to javascript core memory usage limitations we are scanning several times a small range of browser memory (a few Mb) to find some essential data in RAM, if the memory is flooded then the range to scan becomes much larger & the probabilities that our data is found in the smaller range decrease dramatically....

So in short, never use the browser or set a homepage you cancel before running the exploit!
If you need to, set the homepage to 'blank', close the browser then reopen it to start the flash writer.

Usage Tips:
1) Try using a LAN connection or a solid WiFi connection during exploitation. A weak signal can cause problems.
2) If the exploit takes more than 5 minutes to work, reload page, browser, or restart console and try again.
3) If you are using a LAN connection and experience network issues, make sure all cables to router are in working order.
=================================================================================================================


Steps:

1. Setup a small Web server on pc or smartphone. A custom miniweb application has been created by Aldo, and supplied to host files if you would like to use it. Don't come to us for explanations about how to run a http server though. Google it.

2. Extract the files from release to your http server root folder.

3. Copy the "flsh.hex" file from release folder to root of flash drive.

4. Put a FAT32 USB key in port closest to BD Drive (/dev_usb000).

5. DOUBLE-CHECK your flash drive on XMB to make sure it shows up under Music, Photos, Videos, etc.

6. Open the ps3 browser, press start & write the ip address of your server (and the port if not 80) & the name of the appropriate file ie
nand-4.82.html for NAND consoles (Phat Models Axx/Bxx/Cxx/Exx/Gxx) or nor-482.html for NOR consoles (Phat Models Hxx/Jxx/Kxx/Lxx/Mxx/Pxx/Qxx & Slim Models 2xxx (minver 3.56 or lower ONLY, check with minverchk.pup).
For example: http://192.168.0.100/nor-482.html on NOR consoles.

7. Click on the button and wait for PS3 to power down. DO NOT STOP THE PROCESS ONCE STARTED!!

8. Once PS3 has powered down, reboot console and install CFW matching OFW version. If installing through XMB does not work, boot to recovery and install.




***********************
HISTORY
***********************
v1.0.0
- Initial Release. Supports Direct OFW to CFW patching for All Phat and 2xxx Slim (minver 3.56 Dec 2010 and lower)
