# wutKraken
howdy_wurld - Overview of content

Welcome to a collection of some various, somewhat simple scripts.  I mainline with PowerShell but learned more heavily from MS SQL and Python Scripting.  I try to keep an object based approach for sake of explanation and debugging.

The below script is mainly used for me to update podcast files with the correct file sizes, before I push the updated .xml rss feed out.
https://github.com/botsama/getFileAttrb_pwrShl

For software removal and deployment, I have a registry script that crawls around both registry trees for the sake of auditing and removing old software.  Helpful if you have an existing VM or server image you wish to clean up old installs from and to push new installs onto.
https://github.com/botsama/uninstallSoftware_pwrShl

I do not currently have many Python script examples but I did make one to build queries up for me to run against a firewall dataset I imported into a MSSQL database.  Honestly, this would better be served in PowerShell to then also actually run the query with <b>Invoke-Sqlcmd</b>.  I am working on a similar method and should get around to doing this in PowerShell.
I like to do remix scripts.  I feel it helps me learn and get a better grasp of things I am trying to do.
https://github.com/botsama/firewallProc-BuildMSSQLQueries_python

For creating local service account users, I run windows commands and evaluate the results to see if that user already exists.  Little bit of logic checking to make use of <b>If</b> and <b>Else</b> conditions.  Do nothing if command returns that user already exists.
https://github.com/botsama/serviceAccount_pwrShl

More registry querying.  I am showing my age a little bit since I don't know how often an actual ODBC / DSN connection is used, since they tend to be defined in some sort of application config.  However this may be of use if checking for exisiting applications with database connectors.
https://github.com/botsama/odbcGetConf_pwrShl/blob/master/getOdbc.ps1

Say you have a certain list of file extensions you want to generate an output file for with the SHA256 value for each file.  This script will collect all matching file extensions, generate a SHA256 for each of them (in the same local file folder) and <b>process all matching results in the list, until the loop<b> has completed.
https://github.com/botsama/hashFile_val/blob/master/getHashFile.ps1

In the event of looking to collect event logs and other machine details, please enjoy the below log collection script.  A few people gave me positive feedback for this one and I appreciate it.  You would never know I spent some time doing SysAdmin roles when reading this script.
https://github.com/botsama/logCollection_pwrShl


Early 2019 comments below:
Most all of the Powershell scripts have been demoed live back in November for the 24 hour #ExtraLife charity stream. Powershell Spooktacular is where I showed these being used on a VM lab. I talk and present the final hour and 20 minutes or so.
https://www.twitch.tv/videos/332624318

Direct links for video of just Powershell Spooktacular:

Video:
http://ftbliss.link/beepBoop/yeehAw/24hrCharity_event001/017_pic0oPowershellSpooktacular_thugCrowd_hardChats.avi 

Audio:
http://ftbliss.link/beepBoop/yeehAw/24hr_audioOnly_event001/017_pic0oPowershellSpooktacularthugCrowd_hardChats.mp3

Shout out to https://thugcrowd.com Tons of incredible and kind people to be found there.
