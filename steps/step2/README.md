# 01 Installing the Domain Controller

1. SConfig to:
    Change the hostname
    Change IP Address to static
    Change DNS server to Host's IP address
2. Install the Active Directory Windows Feature

````shell
Install-WindowsFeature AD-Domain-Services -IncludeManagementTools
````



```

This is done to the new workstation you are joining to the domain

get-netipaddress - get's the ip address information to see the interface that ipv4 is on
get-DNSClientServerAddress - gets the client serer ip address informaiton.
Set-DNSClientServerAddress - Sets the client server ip address - for this we set it to the DNS server of the Domain controller.

```

``` 
powershell to join pc to domain:

Add-computer -domainname xyz.com -credential -force -restart

```