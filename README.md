# chocolatey_packages
Project to share some Chocolatey Packages

The packages folder structure:
- tools
  - chocolateybeforemodify.ps1
  - chocolateyinstall.ps1 (update field DEFAULTAPP and CHANGE)
  - chocolateyunistall.ps1 (update field DEFAULTAPP and CHANGE)
- _todo
- {packagename}.nuspec (update field DEFAULTAPP and CHANGE)
- readme.md

The software executable must be saved in the tools folder.

#Pack

To pack you need run:
- choco pack {packagename}.nuspec

#Push

To send the new package to you Chocolatey server run:
- choco push {packagename}.nupkg --source http://{serverIP}/chocolatey --force --api-key={yourapikey}

#Install Chocolatey Server
The follow page show the needed steps to install Chocolatey Server:
- https://chocolatey.org/docs/how-to-set-up-chocolatey-server
