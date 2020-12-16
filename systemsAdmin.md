
## Systems Admin IT Roles and Infrastructure

##### servers

This are softwares that provide services to other s/w or machines

    Tower server
    
    Rack Server
    
    blade server
    
KVM switch

    Keyboard,Mouse and Video switch.-->Attached to the server
    
    Connects multiple computers using one KV&M

Supplementary Reading on KVM

[KVM switching](http://en.wikipedia.org/wiki/KVM_switch)

#### The Cloud Computing World

Data Center--->store Millions/hundreds of servers

Cloud-->Remote connection of data from anywhere

#### IT Infrastructure and Roles

Manage systems H/w and S/w

Preform security,DB and many other tasks as a system Admin

H/w life cycle:

    procurement-->h/w purchased/Reused
    
    Deployment--->setting up h/w
    
    Maintenance--->s/w update and h/w fix issues
    
    Retirement--->s/w unusable / no longer  needed
    
Batch update:

    updating s/w of a computer on a predefined sequence

Troubleshooting

    Documents on your work for ease incase of s/w failure


#### As an Administrator:

Linux->script to record commands

powershell->Start-Transcript

windows->recordMyDesktop

##### as an Admin:::::

    Respect rights of others

    Think before you type

    with great power comes great Responsibility

Rollback:

    reverting to the previous state

#### Readings

[Linux Script](http://manpages.ubuntu.com/manpages/bionic/man1/script.1.html)

[Windows start Transcript](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.host/start-transcript?view=powershell-6)

[Read the scripts](http://manpages.ubuntu.com/manpages/bionic/man1/ansi2txt.1.html)

[script readers](http://manpages.ubuntu.com/manpages/bionic/man1/ansi2html.1.html)

[Record my desktop windows](http://recordmydesktop.sourceforge.net/about.php)


N/B:: Never Test in Production us TEST ENVIRONMENT

Reproduction case:

    creating a road map to retrace the steps that led to the user to unexpected outcome

### IT infrastructure services

#### Types of IT infrastructure services

Amazon EC2

Linode

Windows Azure

Google Compute Engine


Cloud services provided

    IaaS - Amazon EC2 -Linode -Windows Azure -Google Compute Engine
    
    NaaS

    PaaS - Heroku-Windows Azure -Google App Engine

    users -Windows Active Directory -OpenLDAP

    DaaS

#### Readings on IT Infrastructure service:

[IaaS](https://www.techrepublic.com/blog/the-enterprise-cloud/side-by-side-comparisons-of-iaas-service-providers/)

[NaaS](https://en.wikipedia.org/wiki/Network_as_a_service)

[SaaS](http://www.businessinsider.com/the-most-popular-cloud-apps-used-at-work-2015-8)

[PaaS](https://www.techradar.com/best/best-paas-providers)

[DaaS -Amazon](https://aws.amazon.com/cloud-directory/)

[DaaS-JumpCloud](https://aws.amazon.com/cloud-directory/)

[DaaS -Azure](https://azure.microsoft.com/en-us/services/active-directory/)


#### Physical Infrastructure

Server Operating System-Regular os that are optimized for server functionality

[Server Operating System](https://www.pcworld.idg.com.au/article/151491/server_operating_systems/)

Remote Access: Linux

[Open SSH](https://en.wikipedia.org/wiki/OpenSSH)

    sudo apt-get install openssh-client

Remote Access: Windows

[Using Putty](https://en.wikipedia.org/wiki/PuTTY)

[Remote Desktop](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/clients/remote-desktop-clients)

[Windows Remote Management](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/clients/remote-desktop-clients)


#### Network Services

[FTP Clients](https://en.wikipedia.org/wiki/Comparison_of_FTP_client_software)
[PXE boot to online softwares](https://en.wikipedia.org/wiki/Preboot_Execution_Environment)

File Transfer Service (FTS):

    FTP-File Transfer Protocol -->Transfer data through the internet: No Encryption but got Authentication

    SFTP -Secure File Transfer Protocol -->SHH Encryption Authentication and Encryption present

    TFTP - Trivial FTP -->No Encryption/Authentication

Network Time Protocol (NTP):

    keep time for machine synchronization on the internet

Proxy Server:

    Intermediary between company's network and the internet

[Power DNS](https://blog.dnsimple.com/2015/02/top-dns-servers/)

DHCp--->Automatic assignment of IP addresses

[DHCP software](https://blog.dnsimple.com/2015/02/top-dns-servers/)

Troubleshoot Network Issues:

    use nslook up to check for correct addressing

        nslookup www.google.com

    use ping to check configuration

        ping www.google.com

#### Managing Services in Linux:

check NTP service running:

    service ntp status

stop a set date or time:

    sudo date -s "2017-01-01" 00:00:00

    sudo service ntp stop

start

    sudo service ntp start

Restart NTP

    sudo service ntp restart

#### Managing service in Windows

Software update powershell:

check for updates

    Get-Service wuaserv

check services configured to run

    Get-Service wuaserv | Format-List

### Service Configuration Linux
