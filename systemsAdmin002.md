

#### Software service:

    services that employees use to enable them to deliver tasks at work

#### Platform service:

    provide a platform for developers to code,build and manage software application

#### Configuring Communication Services

Instant Communication:

    IRC-Internet Channel Relay.(Client-server Model) - 1990s

paid option:

    HipChat

    Slack

Communication protocol:

    Open IM protocol

        XMPP--->Extensible messaging and Presence protocol

            -used in IoT and internet communication

            pidgin and padium-->s/ws usign XMPP

[Paid Chat communication services](https://zapier.com/blog/best-team-chat-app/)

[Open IM chat application](https://jabber.at/p/clients/?os=any)

#### Configuring email services

A Record---> used for Hostname

MX Record--->Email exchange record

##### Email protocols

    POP3

        post Office protocol

        Download email from an email server onto local device

        only to be viewed on one server and device

    IMAP

        Internet Message Access protocol

        Download from email server onto  multiple devices

    SMTP

        Simple Mail Transfer Protocol

        Used for sending emails
        
[Steps to set up your email server](https://www.digitalocean.com/community/tutorials/why-you-may-not-want-to-run-your-own-mail-server)

[Different types of Email  protocols](https://blog.servermania.com/what-protocols-send-receive-email-with-the-mail-server/)

#### Configuring user productivity


#### Configuring user productivity

Always review terms for each s/w you provide for your team and their licence.

#### Configuring security services

Ensure well encryption for any data being used

HTTP-S---make sure your URLs has the Secure part if the web communication browsing capability

TLS------>Transport Layer Security (keep communication secure over a network)

SSL ---->Secure Socket Layer Protocol(Secure communication between web and client server)

### File Services

[File services handling](https://www.cloudwards.net/comparison/)

Network File Storage

    FAT32
    
    NFS-->Network File System
    
        ->Enables Files to be shared over a network
        
        -> Can access Files using the NFS Server and Connection
        
    Samba --->file software that Works for Windows
    
          ---SMB is a n implementation of samba
          
    NAS-->Network Attached Storage
    
        ->Computers designed specific for File storage and Ops

[SMB Reading](https://technet.microsoft.com/en-us/library/hh831795(v=ws.11).aspx)

[NFS server software](http://www.linuxfromscratch.org/blfs/view/cvs/basicnet/nfs-utils.html)

[Mobile data synchronization Android](https://support.google.com/android/answer/2819582?hl=en)

[Mobile data synchronization IoS](https://support.apple.com/HT203977#icloud)


### Printers and server printers

[printer Technologies](https://en.wikipedia.org/wiki/Inkjet_printing)

[Inkjet printer](https://computer.howstuffworks.com/inkjet-printer.htm)

[Laser Printers](https://en.wikipedia.org/wiki/Laser_printing)

[How Laser works](https://computer.howstuffworks.com/laser-printer.htm)

[Dot matrix printers ](https://en.wikipedia.org/wiki/Dot_matrix_printer)

[Thermal printers](https://en.wikipedia.org/wiki/Thermal_printing)

[3D printers](https://en.wikipedia.org/wiki/3D_printing)

[How it works](https://en.wikipedia.org/wiki/3D_printing_processes)

[3D types printing machines](https://3dinsider.com/3d-printer-types/)

[Windows Connection printer](https://support.microsoft.com/help/4027370/windows-10-view-the-print-queue)

[Mac OS printer connection](https://support.apple.com/guide/mac-help/mchle453335f/mac)

[Ubuntu printer connect](https://help.ubuntu.com/stable/ubuntu-help/printing-setup-default-printer.html)


Installing printers

[Windows OS](https://support.microsoft.com/help/4015386/windows-10-install-printer)

[Mac Os](https://support.apple.com/guide/mac-help/mh14004/mac)

[Mac-Windows](https://support.apple.com/guide/mac-help/mac-print-a-printer-connected-windows-mchlp2437/mac)

[ubuntu OS ](https://help.ubuntu.com/stable/ubuntu-help/printing.html)

Virtual printers

[Document writer](https://docs.microsoft.com/windows/win32/printdocs/microsoft-xps-document-writer)

[save PDF on Mac](https://support.apple.com/guide/mac-help/mchlp1531/mac)

[Ubuntu print](https://help.ubuntu.com/stable/ubuntu-help/printing-to-file.html)

Printer sharing on network

[Windows](https://support.microsoft.com/help/4089224/windows-10-share-network-printer)

[Mac](https://support.apple.com/guide/mac-help/mchlp2424/mac)

[Add printer Mac](https://support.apple.com/guide/mac-help/mh14004/10.14/mac/10.14)

Network Printers

[Windows](https://support.microsoft.com/help/4015386/windows-10-install-printer)

[Mac Os](https://support.apple.com/guide/mac-help/mh14004/10.14/mac/10.14)

[Ubuntu](https://help.ubuntu.com/community/NetworkPrintingWithUbuntu#Printing_from_Ubuntu)

printing servers

[print doc service overview](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/hh831468(v=ws.11))

[ubuntu - CUPS print Server](https://help.ubuntu.com/lts/serverguide/cups.html)



### Platform services

Enables developers to build code and ship softwares without many configurations

Web servers:

    most used is Apache server

[web servers](https://stackshare.io/stackups/apache-httpd-vs-microsoft-iis-vs-nginx)

[Database Admins](https://www.bls.gov/ooh/computer-and-information-technology/database-administrators.htm)

[Types of Database](https://www.digitalocean.com/community/tutorials/sqlite-vs-mysql-vs-postgresql-a-comparison-of-relational-database-management-systems)

#### Diagnose a faulty website

HTTP status code:

    shows numbers incase of errors when accessing a web service

    4XX ---Codes indicate issues on Client slide

    5XX --->Server side code error

    2XX -->Successful request

[Troubleshooting with Chrome Developer Tools](https://developer.chrome.com/devtools)

[List of HTTP status code](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes)

### Managing Cloud Resources

SaaS--->Software as a Service

    The software is already pre configured and the user isn't deeply involved in the cloud configuration

IaaS---Infrastructure as a Service

    Hosting your own service in the cloud

    you decide how you want the infrastructure to look,depending on what you want ot run on it

public cloud--cloud services provided by third party

private cloud-->When your company owns the services and the entire infrastructure both onsite/remote data center

Hybrid cloud-->mix of both private and public cloud

#### Cloud infrastructure Setups

Load balancer:

    Ensures each VM receives a number a balanced number of queries

Autoscaling:

    service increase/decrease as needed .

    service owner only pays for the active ones in use

Service:

    Monitoring

    Alerting

### Popular Cloud providers

[Microsoft Azure](https://azure.microsoft.com/en-us/overview/what-is-cloud-computing/)

[Amazon ](https://aws.amazon.com/getting-started/)

[Google Cloud](https://cloud.google.com/docs/overview/)


#### commandline interface to create a VM

    gcloud compute instances create linux-instance --zone=us-central1-f --machine-type=n1-standard-1 --subnet=default  --tags=http-server --image=ubuntu-1604-xenial-v20190628 --image-project=ubuntu-os-cloud --boot-disk-size=10GB

    gcloud compute firewall-rules create default-allow-http --direction=INGRESS --priority=1000 --network=default --action=ALLOW --rules=tcp:80 --source-ranges=0.0.0.0/0 --target-tags=http-server

Windows instance

    gcloud compute instances create windows-instance --zone=us-central1-f --machine-type=n1-standard-1 --subnet=default --image=windows-server-2016-dc-v20190709 --image-project=windows-cloud --boot-disk-size=50GB

list all instance

    gcloud compute instances list

Time to connect to linux

    gcloud compute ssh linux-instance --zone us-central1-f
    
make an update

    sudo apt update

install nginx software

    sudo apt install nginx

#### creating an additional disk

Has NAme,source,Type and size

    gcloud compute disks create additional-disk --type=pd-standard --size=500GB --zone=us-central1-f

Attach disk to instance

     gcloud compute instances attach-disk windows-instance --disk additional-disk
