Windows Server 2022 File Server LabA virtualized lab showcasing the deployment of Windows Server 2022 as a file server, integrated with an existing Active Directory domain to provide centralized file storage and access for an enterprise-like environment.

- Windows Client (Access Clients)
- VirtualBox (Virtualization Platform)
- File Server Administration, Active Directory Integration, Permissions Management

Deployed Windows Server 2022 in VirtualBox as a dedicated file server

  - Created a new virtual machine name FileServer, allocating 4GB of ram, 2 processors, and 50GB of storage.

![Fileserver-Creation](Fileserver-Creation.png)


  - Set static IP for file server and set DNS to DC1

![Static-IP](Static-IP.png)

  - Joined the new file server to the lab.com domain and renamed the server to FileServer

![Join-Domain](Join-Domain.png)

  - Installed the new File and Storage Services role through the Server Manager

![File-Server-Role](File-Server-Role.png)

  - Created a new folder with shared access to LabUser1 only

![LabUser1-Sharing](LabUser1-Sharing.png)

  - Client LabUser1 is able to connect to the folder and create documents

![Client1-Access](Client1-Access.png)

  - Created a network drive directly to the shared folder on the Client1 maching for LabUser1

![Client1-Network-Location](Client1-Network-Location.png)

  - When logging in as LabUser2, they are denied access to the shared folder

![Client2-Permission-Denied](Client2-Permission-Denied.png)
