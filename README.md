# active_directory
- Howto install AD on Server 2022 core

1. use `sconfig` to:
    - Change hostname
    - Change Static IP Address to DC
    - Change DNS to local IP

2. Install the Active Directory Windows Feature

 ````shell
 Install-WindowsFeature AD-Domain-Services -IncludeManagementTools
 ````
````shell
Import-Module AddsDeployment
Install-ADDSForest
````

3. Change DNS to local IP Address again

