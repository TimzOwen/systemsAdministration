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
