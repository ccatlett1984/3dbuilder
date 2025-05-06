create a folder on your C drive, named "3d_builder"
copy the contents of this archive into that folder

open a powershell prompt, and paste the following commands
(one line at a time, pressing Enter for each)

$filepath = "C:\3d_builder\"

Get-Childitem $filePath -filter *.appx| %{Add-AppxPackage -Path $_.FullName}

Get-Childitem $filePath -filter *.appxbundle | %{Add-AppxPackage -Path $_.FullName}

(You have successfully installed 3d builder, it should now be in your start menu)
