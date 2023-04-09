Memory forensics involves acquisition and analysis of a computer's volatile memory (computer's RAM). 
The acquired memory is normally referred to as a memory dump, and can be particularly useful in identifying 
- Running processes
- User credentials
- Network connections
- Registry keys
- Encryption keys
- Browser history
- Clipboard contents, and other valuable information.

## Tools to acquire Memory Dump

    DumpIt — a light-weight command-line utility for Windows.
    FTK Imager — a popular image forensics tool.
    Redline — a memory analysis tool developed by FireEye.
    
    
 To acquire a memory image from offline Windows machines, we can extract it from 
 
    %SystemDrive%/hiberfil.sys
 which contains a compressed memory image from the previous boot that is normally kept to provide faster boot-up times.



## TO BE EDITED
DumpIt to collect a memory dump file for analysis, which can be downloaded from https://raw.githubusercontent.com/thimbleweed/All-In-USB/master/utilities/DumpIt/DumpIt.exe.

    Note: Acquiring a memory dump can be a time-consuming process, so you may use the memory dump that is available for download at the link provided in the next section.

When you have downloaded the tool, go ahead and double-click on the executable file. This will launch a command prompt that will ask you to confirm the memory capture by typing 'y' or 'n'. Type 'y' to confirm, and the tool will immediately initiate the memory capture process:

DumpIt - v1.3.2.20110401 - One click memory memory dumper
  Copyright (c) 2007 - 2011, Matthieu Suiche <http://www.msuiche.net>
  Copyright (c) 2010 - 2011, MoonSols <http://www.moonsols.com>

    Address space size:       19042140160 bytes (  18160 Mb)
    Free space size:         188405813248 bytes ( 179677 Mb)

    * Destination = \??\C:\Users\saadj\Downloads\DESKTOP-ABCDEFG-20230402-184706.raw

	  --> Are you sure you want to continue? [y/n]
		+ Processing...

As a result, the memory dump file will be saved in the same directory where the tool was launched.

    bulb The memory dump file extension can vary depending on the tool used to create the dump. Some common extensions for memory dumps include .raw, .mem, .vmem, and .bin.
