taskkill /f /im Origin.exe

taskkill /f /im OriginWebHelperService.exe


robocopy %ProgramData%/Origin/LocalContent %temp%\Origin/LocalContent /mir /e /copyall /sec



cd C:/ProgramData/

	rmdir /s /q Origin

robocopy %Temp%\Origin %ProgramData%/Origin /mir /e /copyall /sec /move



cd %AppData%

	rmdir /s/q Origin

cd .. 

cd Local

	rmdir /s/q Origin
PAUSE


