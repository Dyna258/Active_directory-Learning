# 01 Installing the Domain Controller

1. SConfig to:
    Change the hostname
    Change IP Address to static
    Change DNS server to Host's IP address
2. Install the Active Directory Windows Feature

````shell
Install-WindowsFeature AD-Domain-Services -IncludeManagementTools
````