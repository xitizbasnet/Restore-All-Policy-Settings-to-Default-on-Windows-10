# Restore-All-Policy-Settings-to-Default-on-Windows-10
Restore All Policy Settings to Default on Windows 10 

...............................

So your computers has a message saying “some settings are managed by your organization message” or “some of these settings are hidden or managed by your organization” This is very common and normally means you or someone who uses the computer have setting policies in place to block certain features of windows 10. This is normally to do with windows updates, privacy settings and telemetry. Either you have used group policy editor to block these features, or registry tweaks to block or disable these features or software like ADP or Shutup 10 or any other type of privacy software. I will show you step by step on how to reset these settings with a simple command.

...............................

1. Open command prompt with admin permission


...............................

2. Execute these commands then restart the computer

RD /S /Q “%WinDir%\System32\GroupPolicy”


RD /S /Q “%WinDir%\System32\GroupPolicyUsers”

gpupdate.exe /force


...............................
