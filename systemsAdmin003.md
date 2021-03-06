### Directory services

### Directory services

Contains a lookup services that provides mapping between network resources and their network addresses

Directory service: ---> Useful for organizing data and making it searchable for an organization

DAP-->Directory Access Protocol:

DSP-->Directory Service Protocol

DISP-->Directory Information Shadowing Protocol

DOP-->Directory Operational Bindings Management Protocol

LDAP-->Lightweight Directory Access Protocol

implementation:

    Microsoft Active Directory: AD

    OpenLDAP--covers windows,Unix

#### Instaling and configuring Active Directory

Powershell

    C:\Qwiklabs\ADSetup\active_directory_install.ps1

    configure with --> C:\Qwiklabs\ADSetup\configure_active_directory.ps1

#### Centralized Management

Central service that provides all instructions to all of the different parts of my IT infrastructure

Directory services:

    provide centralized authentication, Authorzation and accounting , also known as AAA

Role based Access Control (RBAC)

Configuration management frameworks:

    chef

    SCCM

    Puppet

[Role-based access control](https://en.wikipedia.org/wiki/Role-based_access_control)

[Chef](https://www.chef.io/chef/)

[Puppet](https://puppet.com/)

[System Control Center Configuration Manager](https://docs.microsoft.com/en-us/sccm/core/understand/introduction)


#### LDAP(Lightweight Directory Access Protocol)

used to access information in directory services like over a network

    OpenLDAP--mostly used

    Active Directory -also uses it

[LDAP Format](https://en.wikipedia.org/wiki/LDAP_Data_Interchange_Format)

LDAP Binding

    authenticate a client to a directory server

components of LDP

    Common Name

    Uncommon Name

    Distinguished Name

LDAP Authentication:


    Anonymous

    Simple

    SASL: Simple Authentication & Security Layer

        uses Kerberos:

            Network authentication protocol that's used to authenticate user identity,secure the transfer of user credential and more

[Kerbros extended Reading](https://technet.microsoft.com/en-us/library/cc780469(v=ws.10).aspx)

### Active Directory

Native Directory service for Microsoft Windows

Also a central Repo for Group Policy Object GPOs--manage configuration of windows machine

Tools used:

    ADAC-->Active Directory Administrative Center

OU---> type of container (Organizational unit)

Domain Controllers:

    provide several services on network

    Hold replica of AD Database

    serves as DNS Server to provide name resolution and service discovery to clients

FSMO-->Flexible single-master operations

[Active Directory supplementary reading](https://technet.microsoft.com/en-us/library/cc961936.aspx)

#### Managing Active Directory:

User SAM account--->Security Account Manager.(Stores the user name and password in windows db)

[Group scope in windows](https://technet.microsoft.com/en-us/library/cc961936.aspx)

[Security principles](https://technet.microsoft.com/en-us/library/cc780957%28v=ws.10%29.aspx?f=255&MSPPError=-2147217396)

#### Managing AD user passwords

click on the user from the respective domain and reset password

make sure the unlock checkbox is checked .

Allow also the user t change password on next Login

[Supplementary Reading for EFS](https://technet.microsoft.com/en-us/library/cc962100.aspx)

#### Joining an Active directory Domain

change from WorkGroup on windows settings in PC's Property

add from command prompt:

    Add-Computer -DomainName 'example.com'-Server 'dc1'

Functional Level-Desc features it support

    Get-AdForest

    Get-AdDomain

[Forest and Domain Functional Levels](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/active-directory-functional-levels)


#### Group policy

GPO-Group object policy:

    set of policies and preferences that can be applied to a group of objects in the directory

    Groups all the users and must follow the set policy

security Filtering

WMI Filters

policies: Settings that are reapplied every minute  and aren't meant to be changed even by local administrators

Group policy:  a template setting

Windows Registry:

    hierarchical db of settings that windows, and many windows application use for storing configuration data.

#### Group policy inheritance and Precedence.

Tool:

Group Policy Management Console (GPMC):

WMI--->Windows Management Instrumentation

Can run GPMC.MSE from command line

RSOP----> adding all group policies together for specific machine and apply precedence

#### Group policy Troubleshooting

DNS Records--Established computer connection to the DNS server

     _ldap._tcp.dc._msdcs.DOMAIN.NAME

     on cmd ps--> Resolve-DNSName -Type SRV -Name _ldap._tcp.dc._msdcs.example.com

Fast Logon Optimization:---->Changes application
 
update-->

    gpupdate/force

    gpupdate/force/sync----Logout everyone on the computer

[Force Group policy resync](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/windows-time-service/how-the-windows-time-service-works)

[Manually force a domain](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-xp/bb491016(v=technet.10))

[Troubleshoot AD Replica](https://msdn.microsoft.com/en-us/library/bb727055.aspx)

[GPO control on sccope](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2008-R2-and-2008/cc772166(v=ws.11))

[Controling GPO](https://technet.microsoft.com/en-us/library/jj134176(v=ws.11).aspx)

[GP Result command](https://technet.microsoft.com/en-us/library/cc733160(v=ws.11.).aspx)

[Create WMI](https://technet.microsoft.com/en-us/library/cc770562(v=ws.11).aspx)


#### Mobile Device Management

controls Profile and policies

Remote wipe:

    A factory reset that you can trigger from your central MDM, rather than having to do it in person on the device

Enterprise Mobility management  (EMM):--> Creating a distributing the policies across different Mobile OS

#### Supplementary Reading for MDM:

[IoS MDM payload list ](https://support.apple.com/guide/mdm/payload-list-mdm5370d089/web)

[Android settings](https://support.google.com/a/answer/6328708#apply)

[ios intro to Profile Manager](https://support.apple.com/guide/server/intro-to-profile-manager-apd0e2214c6/mac)

[ios MDM settings payload](https://support.apple.com/guide/mdm/payload-list-mdm5370d089/web)

[Android get started with Google Mobile Management](https://support.google.com/a/answer/7396025)

[Apply settings for Mobile Devices](https://support.google.com/a/answer/7396025)


### OpenLDAP (Lightweight Directory Access Protocol)

Free opensource Manager for Directory

LDAP Data Interchange Fomart:

    you can auth, Add or Remove Users,Groups

    used on All Os

you ca work from:

    command Line
    php LDAP Admin--(Web UI to manage)

Installing:

    sudo apt -get install slapd ldap-utils

    sudo dpkg-reconfigure slapd ----> to reconfigure our setting

[Installing OpenLDAP and PHPAdmin for ubuntu ](https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-openldap-and-phpldapadmin-on-ubuntu-16-04)

[OpenLDAP org ](https://www.openldap.org/doc/admin24/slapdconf2.html)

#### Managing OpenLDAP

Using CommandLine to manage. You need LDIF Files.

    ldapadd-->Takes the input of LDIF file and adds the context of the file

    ldapmodify-->modify an existing object

    ldapdelete-->remove object that the LDIF file refers to

    ldapsearch-->search for entries in your directory db

[Data interchange format ](https://en.wikipedia.org/wiki/LDAP_Data_Interchange_Format)

[using LDIF files to make changes to an OpenLDAP system](https://www.digitalocean.com/community/tutorials/how-to-use-ldif-files-to-make-changes-to-an-openldap-system)
