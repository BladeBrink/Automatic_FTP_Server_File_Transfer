# Automatic_FTP_Server_File_Transfer
Automating the process of transferring files from an external FTP server to a clients internal network.

This is a report for project called Automating File Transfer.

Lines 16-21 are imports of required libraries.
Line 24 we are creating a logger, setting its level to info to catch all the exception.
Lines 26-31 prompts the user for various inputs.

Lines 34  function for uploading files from an ftp server to an internal network.
Lines 42-45 connect to the FTP server.
Line 48 the log that the connection is established.
Line 51-55 check if the local directory exists, if not create it.
Line 58 change the working directory on the FTP server.
Line 61 retrieve a list of files in the directory.
Lines 64-67 iterate through the files, download and save to the local directory.
Line 69 iterate through the files, download and save to the local directory.
Lines 70-71 exception, connection error message.
Lines 73-76 moving downloaded files from a local directory to an internal network destination.
Line 77 exception, file move error message.

Lines 81-91 Script scheduled to run every day at 10:30.
Line 95 this function is called to schedule the script to run every day at 10:30 by using schedule library.
Line 96 creates an infinite loop which will run indefinitely.
Line 97 check whether there is any scheduled task pending to run or not. If there is any scheduled task pending, it will run it.
Line 98 will pause the execution of the script for 1 second. This is useful to avoid the infinite loop from consuming too much CPU resources and also it will wait for the scheduled task to be completed before checking again.

Lines 101-102 a block of code that should only be executed when the script is run directly.

A public ftp server was used for the test:
	host = 'ftp.otenet.gr '
	user = 'speedtest'
	password = 'speedtest'
	remote_dir = '/'
