## Systems Data Recovery and Bacuk up

## Dealing with Data

#### Data recovery

The process of trying to restore data after unexpected event that results in data loss /corruption

Nature to recover:

    Damaged devices-->HDD recovery

    presences of backup

post-mortem:

    A way of documenting problems discovered, how you fix them so that you make sure they don't happen again

[Gitlab response to data loss and outage](https://about.gitlab.com/2017/02/01/gitlab-dot-com-database-incident/)

#### Data backup

1. What dat you need to back up

2. How much data you have

3. Account for future growth


#### Backup solution

Data tapes-->standard medium for archival backup

rsync--cmd line file tool used to transfer and synchronize files between locations or computers
        --> uses SSH which is secure to transfer files
        
Time machine-->Apple backup machine

Backup and restore--->Microsoft

#### back up solution Read on

[Microsoft backup and restore](https://support.microsoft.com/en-us/help/17127/windows-back-up-restore)

[Apple time back up](https://support.apple.com/en-us/HT201250)

[Rsync back up utility](https://wiki.archlinux.org/index.php/rsync#As_a_backup_utility)



#### Testing backups

Document the backup procedures for other devs to recover them with minimal interruption

Disaster recovery Testing:

simulate data loss and implement a back up

#### Types of backup

Regular backup:

    back up the entire file/system

Differential back up:

    backup induplicate and unchanging data

Regular incremental back up:

    only back up changing data

File compression:

    store data with complex algorithms ro save on space

RAID-->Redundant Array of Independent Disk

    -->Combining multiple physical disk into one large virtual disk
    
        labels to determine RAID
        
    --performance
    
    --Reliability
    
    --capacity

[RAID supplementary reading](https://en.wikipedia.org/wiki/Standard_RAID_levels)

#### User back ups

    Dropbox

    Apple iCloud

    Google Drive


#### Disaster Recovery plan

collection of documented procedures and plans on how to react and handle an emergency/disaster  scenario

from the operational perspective

Detection measure:

    for alert to you and your team that a disaster has occurred that can impact operations

Corrective /Recovery measures:

    Those enacted after a disaster has occurred

#### Designing a Disaster Recovery plan

Steps:
    1. Perform a Risk Assessment
    
    2. Determine backup and recovery System
         operational documentation on different procedures and should be updated
         
    3. Determine Detection & Alert Measure & Test Systems
    
    4. Determine recovery measures


### Post-mortem

Analyze an event that occurred to make sure it doesn't happen

Learn from some mistakes and root cause and how to prevent them

#### writing a post-mortem

1. brief summary:

        what was the incident

        How long it lasted

        what was the impact

        How it was fixed

2. Detailed time line

        when it started

        people notified

        correct time zones,date and

        Actions takes

3. Root cause

          what led to the issue

          what can be learned
    
4. Resolution and Recovery efforts

          steps taken to resolve

          time zones also included

5. Actions to avoid same scenario

         Action taken to improve and prevent it

         monitoring systems

         what went well
