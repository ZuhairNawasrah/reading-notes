# Version Control System

Version control system **VCS** allow you to revisit various versions of a file by recording changes, and there is three types of **VCS**:
1. Local **VCS**, which entails one database on your hard disk.
2. Centralized **VCS**, entails a single server which can be accessed by various clients, and this streamlined the collaboration process by eliminating the need to involve all local databases.
3. Distributed **VCS**. In event of corruption of central database's hard disk -with the absence of backups-all work at server will be lost, to prevent this type of catastrophic loss, a **DVCS** allows clients to create mirrored repositories.

## Git

**Git** isn't a **LVCS** or **CVCS**, it's a **DVCS** that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — **Git** creates a snapshot of the file and stores a reference to it. If the file has not changed, **Git** only stores a reference to the already-stored identical version of it.

Every single change applied to any file or directory is tracked by **Git**. And, as the gatekeeper, **Git** will always detect file corruption or loss of information in transit.Also **Git** is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. **Git** makes it extremely difficult for a snapshot of your file that is committed to be lost.