create a folder on your C drive, named "3d_builder"
copy the contents of this archive into that folder

open a powershell prompt, and paste the following commands
(one line at a time, pressing Enter for each)

$filepath = "C:\3d_builder\"

Get-Childitem $filePath -filter *.appx| %{Add-AppxPackage -Path $_.FullName}

Get-Childitem $filePath -filter *.appxbundle | %{Add-AppxPackage -Path $_.FullName}

(You have successfully installed 3d builder, it should now be in your start menu)


If you would like to obtain these files yourself, you may get them from a Windows machine that has the application installed
Path: "C:\Program Files\WindowsApps"

or from the following website:
https://store.rg-adguard.net/

enter: https://apps.microsoft.com/detail/9wzdncrfj3t6?hl=en-us&gl=PH

select "Retail" from the drop-down.


