# Cmnw 145 Active Directory Project Documentation

**ProjectM27.local**

**Joseph Emerson**

**Lorain County Community College**

**Table of Contents**
# Table of Contents
1. [LAN Overview](#lan-overview)
2. [Network Settings Setup Diagram](#network-settings-setup-diagram)
3. [Users and Groups](#user-and-groups)
4. [Definition of Terms](#definition-of-terms)





## **LAN Overview**

**Server and Client description**:

ProjectM27.local consists of 2 Windows 2019 servers, and 2  Windows 10 clients.

- The servers have the following specifications:
    - Processor: Intel® Xeon® Silver 4112 CPU @ 2.60GHz 2.60GHz
    - RAM: 4GB
    - Storage: 39.9GB
    - Windows Server 2019 Standard Edition
- The Clients have the Following Specifications:
    - Processor: Intel® Xeon® Silver 4112 CPU @ 2.60GHz 2.60GHz
    - RAM: 4GB
    - Storage: 39.9GB
    - Windows Server 10 Pro Education Edition

**Summary of users and groups:**

The users are assigned by function to the following groups –

- Bank President
- Bank Vice President
- Bank Manager
- Bank Loan Officer
- Human Resources
- Bank Teller
- Account Holder

The groups are setup in global and local groups. The local groups contain the global group as members, as well as the individual users that belong to those groups.

**An overview of the share and NTFS permissions**

The security is setup so that the bank presidents and vice presidents are capable of accessing, reading, and editing all of the folder structure. The Bank Managers have the second most level of access. They can manage bank loan officers, human resources, bank tellers, and account holders.

There is a Main share folder that has the share permissions allowing all domain users to access it, with the following permissions:

- Change
- Read
    - Administrators have full control over this folder

![Untitled](/Images/Picture10.png)

## **Network Settings Setup Diagram**

1. System Name: **145SRV19M27**
    1. (The **Domain Controller**)
    2. (**DNS server**)

**IP information**

![Untitled](/Images/Picture1.png)

The server naming convention is use 192.168.24.M#. In this case the server’s M# assigned is 27 which makes the IP address 192.168.24.27.

The subnet is the default subnet assigned of 255.255.255.0.

The DNS IP address is setup to 192.168.24.27

1. System Name: **145SRV19M64**
    1. **Second Server**

**IP information**

![Untitled](/Images/Picture2.png)

The server naming convention is use 192.168.24.M#. In this case the server’s M# assigned is 64 which makes the IP address 192.168.24.64.

The subnet is the default subnet assigned of 255.255.255.0.

The DNS IP address is setup to 192.168.24.27

1. System Name: **145WIN10M27**
    1. **Client system**

**IP Information**

![Untitled](/Images/Picture3.png)

The server naming convention is use 192.168.24.M#.

If the system’s M# is repeated we do M# + 100 for the new number to use.

In this case the server’s M# assigned is 27 which makes the IP address 192.168.24.127.

The subnet is the default subnet assigned of 255.255.255.0.

The DNS IP address is setup to 192.168.24.27

1. System Name: **145WIN10M64**
    1. **Client system**

**IP Information**

![Untitled](/Images/Picture4.png)

The server naming convention is use 192.168.24.M#.

If the system’s M# is repeated we do M# + 100 for the new number to use.

In this case the server’s M# assigned is 64 which makes the IP address 192.168.24.164.

The subnet is the default subnet assigned of 255.255.255.0.

The DNS IP address is setup to 192.168.24.27

## **User and Groups**

A list of the users, passwords,  group memberships, and other pertinent information.

| Position | Full Name | Username | Password | Telephone Number |
| --- | --- | --- | --- | --- |
| Bank President | Cory E. Ealy | ealyc | cmnw2#1 | 562-458-2909 |
| Bank Vice President | Helen A. Cook | cookh | cmnw2#1 | 305-658-7674 |
| Bank Vice President | Max J. McCain | mccainm | cmnw2#1 | 706-484-3290 |
| Bank Manager | Ruth V. Velez | velezr | cmnw2#1 | 606-636-0233 |
| Bank Manager | Sarah E. Junior | juniors | cmnw2#1 | 309-739-1214 |
| Bank Loan Officer | Valerie B. Patton | pattonv | cmnw2#1 | 318-556-2287 |
| Bank Loan Officer | George F. Atherton | athertong | cmnw2#1 | 239-236-9311 |
| Human Resources | Harry G. Parker | parkerh | cmnw2#1 | 734-782-4198 |
| Human Resources | Graig D. Gomez | gomezg | cmnw2#1 | 972-838-7133 |
| Bank Teller | Maggie C. Austin | austinm | cmnw2#1 | 845-431-0297 |
| Bank Teller | Rebecca J. Yokley | yokleyr | cmnw2#1 | 918-928-4216 |
| Bank Teller | Richard S. Connolly | connollyr | cmnw2#1 | 856-946-7545 |
| Bank Teller | Shelly L.  McCullough | mcculloughs | cmnw2#1 | 919-818-5596 |
| Account Holder | Suzanne J. Wallis | walliss | cmnw2#1 | 217-808-7510 |
| Account Holder | Ada S. Armstron | armstronga | cmnw2#1 | 605-256-5487 |
| Account Holder | Kerry J. Weller | wellerk | cmnw2#1 | 985-249-5101 |
| Account Holder | Dale R. Adelson | adelsond | cmnw2#1 | 772-294-1761 |
| Account Holder | Lawrence A. Brockway | brockwayl | cmnw2#1 | 201-336-6790 |
| Account Holder | Dorothy J. Portillo | portillod | cmnw2#1 | 773-606-1132 |

| Account Holder | Paul A. Hedberg | hedbergp | cmnw2#1 | 818-999-2521 |
| --- | --- | --- | --- | --- |
| Account Holder | Jeffrey E. Obrien | obrienj | cmnw2#1 | 602-315-4703 |
| Account Holder | Odell B. Miller | millero | cmnw2#1 | 240-243-0814 |
| Account Holder | Peggy C. Mulholland | mulhollandp | cmnw2#1 | 419-692-5485 |
| Account Holder | Juan R. Miller | millerj | cmnw2#1 | 240-257-7804 |
| Account Holder | Marco F. Wojciechowski | wojcieechowskim | cmnw2#1 | 863-585-6550 |

**A list of the groups and the memberships.**

| Group | Members | Member Of |
| --- | --- | --- |
| accountholder_lg | accountholder_gg |  |
| accountholder_gg | Suzanne Wallis
Ada. Armstron
Kerry Weller 
Dale Adelson
Lawrence Brockway
Dorothy Portillo
Paul Hedberg 
Jeffrey Obrien 
Odell Miller
Peggy Mulholland 
Juan Miller 
Marco Wojciechowski | accountholder_lg |
| bankloanofficer_lg | bankloanofficer_gg |  |
| bankloanofficer_gg | Valerie Patton 
George Atherton | bankloanofficer_lg |
| bankmanager_lg | bankmanager_gg |  |
| bankmanager_gg | Ruth Velez 
Sarah  Junior | bankmanager_lg |
| bankpresident_lg | bankpresident_gg |  |
| bankpresident_gg | Cory Ealy | bankpresident_lg |
| bankteller_lg | bankteller_gg |  |
| bankteller_gg | Maggie Austin
Rebecca Yokley
Richard Connolly
Shelly  McCullough | bankteller_lg |
| bankvicepresident_lg | bankvicepresident_gg |  |
| bankvicepresident_gg | Helen Cook 
Max McCain | bankvicepresident_lg |
| humanresources_lg | humanresources_gg |  |
| humanresources_gg | Harry Parker , Graig Gomez | humanresources_lg |

## **Permissions Table**

![Untitled](/Images/Picture5.png)

![Untitled](/Images/Picture6.png)

![Untitled](/Images/Picture7.png)

![Untitled](/Images/Picture8.png)

![Untitled](/Images/Picture9.png)

## **Definition Of Terms**

Server- A software that performs operating systems and identifies information when a specific file is changed or accessed.

Client- Request services or resources from another computer system (the server).

NTFS Permissions- Allows the users to log in to the server locally.

Share Permissions- This allows you to restrict access or the number of people who can access a folder.

Domain Controller- A domain controller is a server that requests authentication from other users in a computer domain.

DNS Server- DNS servers allow you to find an IP address from a website.
