# This Powershell script is used to create new users and their shared folders in Active-Directory.

This script has to be used on a Windows Server with Active Directory. It has been tested on :
 - Windows Server 2016

# Usage :

The script needs to be launched using Powershell command line.
It can either be launched with the parameters -File "Path_to_the_csv_file" and -Password or with no parameter :
 - If this first option is chosen, the script will create all users listed in the csv_file.csv. The csv_file should be created, and the informations about the users should be written in the following order and using , as a delimiter :
Firstname,Lastname,Site,PrimaryGroup,SecondaryGroup,Tel2,Mobile,Domain,Email
(e.g. : John,Smith,London,Commercial Department,Trainees,04 73 95 68 73,+33 0 00 00 00 00,bigenterprise,john@bigenterprise.com)
 - If the last option is chosen, then the script will create only one user, and will be asking for each information about it.
