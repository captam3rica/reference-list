# Ref list for virtualizaton

## Virtualization

-	[VDI Design Guide](https://vhojan.nl/category/vdi-design-guide/) | Johan van Amersfoort
- 	[Desktop as a Service: Everything you need to know about DaaS and hosted VDI](https://www.amazon.com/gp/product/0985217421/ref=ox_sc_act_title_2?smid=ATVPDKIKX0DER&psc=1) | Brian Madden
-	[VMware vSphere 6.5 Hosted Resources Deep Dive](https://www.amazon.com/gp/product/1540873064/ref=ox_sc_act_title_3?smid=ATVPDKIKX0DER&psc=1) | Frank Denneman

### VMware Horizon

- [Horizon 7 Documentation](https://docs.vmware.com/en/VMware-Horizon-7/index.html)
	- [Architecture Planning - v7-7.8](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-architecture-planning.pdf)
	- [Hardware Requirements](https://docs.vmware.com/en/VMware-Horizon-7/7.9/horizon-installation/GUID-332CFB83-784A-4578-9354-888C0538909A.html)
- Carl Stalhood - [www.carlstalhood.com/](http://www.carlstalhood.com/)
	- [7.7-8 - Installation](https://www.carlstalhood.com/vmware-horizon-7-configuration/#vcenter)
- 50 Articles to fix everything - https://blogs.vmware.com/kb/2015/03/50-kbs-fix-everything-horizon-view.html
- [WorkspaceONE Horizon Reference Arch](https://techzone.vmware.com/resource/workspace-one-and-horizon-reference-architecture#horizon-seven-vmware-identity-manager-integration)
- [Understanding Horizon Connections - Blog](https://techzone.vmware.com/blog/understanding-horizon-connections)
- Cloud Connector Virtual Appliance - 7-7.8
	- [Deployment](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-installation/GUID-973234D9-000A-4732-957A-CA8BEA3D5D24.html)


#### Licensing

- [Horizon Subscription Configuration - 7.10](https://docs.vmware.com/en/VMware-Horizon-7/7.10/horizon-installation/GUID-F8637B55-EC4B-4100-9075-27D9B3E07EFE.html)


#### Horizon Agent

- [Supported versions of Windows 10 on Horizon Agent Including All VDI Clones (Full Clones, Instant Clones, and Linked Clones on Horizon 7) (2149393)](https://kb.vmware.com/s/article/2149393)
- [Configure Realtime Audio Video](https://docs.vmware.com/en/VMware-Horizon-7/7.6/horizon-remote-desktop-features/GUID-0923B4C2-16C7-4C45-BD6E-945858518798.html)

#### Login Portals

- https://cloud.horizon.vmware.com/login


#### Upgrading

- [Horizon 7-7.8 Upgrade Documentation](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-upgrades/GUID-E3607442-8936-49A8-97B4-722D012FDF1E.html)


#### vSphere (ESXi) Server

- [Install and Setup - ESXi 6.7](https://docs.vmware.com/en/VMware-vSphere/6.7/vsphere-esxi-671-installation-setup-guide.pdf)
- [Install ESXi 6.7 on Workstation, VirtualBox, and Bare Metal](https://www.sysnettechsolutions.com/en/vmware/install-vmware-esxi-6-7/)
- [Adding vSphere CA Cert](https://www.techazine.com/2017/09/22/an-easy-fix-for-vsphere-6-5-web-client-and-certificates-to-keep-your-uploads-flowing/)
- [Import the VCSA Self-Signed Cert](https://tinkertry.com/how-to-get-rid-of-vsphere-browser-certificate-warnings-in-windows)


#### vCenter Server

- [Install and Setup - vCenter 6.7](https://docs.vmware.com/en/VMware-vSphere/6.7/vsphere-vcenter-server-671-installation-guide.pdf)
- [vCenter User Privilege Requirements - 7.7-8](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-installation/GUID-A878F876-B359-42FC-9124-A1E34BFB3319.html)
- VCSA Sysprep file location
	- `/etc/vmware-vpx/sysprep/`
		- https://kb.vmware.com/s/article/1005593
- [Trust the VSCA Cert](https://tinkertry.com/how-to-get-rid-of-vsphere-browser-certificate-warnings-in-windows)


*Linked Clones*

- [Linked Clone Worksheet - Horizon 7.8](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-console-administration/GUID-F336E9DA-EC69-440A-A1B8-28E4FDC1784B.html)


*Configuration Specifications*

- [Create a Customization Specification for Windows](https://docs.vmware.com/en/VMware-vSphere/6.7/com.vmware.vsphere.vm_admin.doc/GUID-CAEB6A70-D1CF-446E-BC64-EC42CDB47117.html?hWord=N4IghgNiBcKEQEACA4gVwKYGcAuCDCLsB7AWwEsAvMLUwgOwQHcKwAnAExAF8g)
- [Guest Operating System Customization Requirements](https://docs.vmware.com/en/VMware-vSphere/6.7/com.vmware.vsphere.vm_admin.doc/GUID-E63B6FAA-8D35-428D-B40C-744769845906.html#GUID-E63B6FAA-8D35-428D-B40C-744769845906)

*Master VM Creation*

- [Creating an Optimized Windows Image for a VMware Horizon Virtual Desktop](https://techzone.vmware.com/creating-optimized-windows-image-vmware-horizon-virtual-desktop#934148)

*Handy Commands*

- VMware has an easy way of retrieving logs both on the connection servers and the virtual machine.
The command to collect the logs from a remote machine is:

	```
	vdmadmin -A -getDCT -outfile file_name.zip -d pool_name -m virtual_machine_name
	```

#### Unified Access Gateway

- [VMware Doc: Deploying and Configuring VMware Unified Access Gateway 3.6](https://docs.vmware.com/en/Unified-Access-Gateway/3.6/com.vmware.uag-36-deploy-config.doc/GUID-F5CE0D5E-BE85-4FA5-BBCF-0F86C9AB8A70.html)
- [UAG 3.6 - Carl Stalhood](https://www.carlstalhood.com/vmware-unified-access-gateway/)
- [UAG 3.5 - Carl Stalhood](https://www.carlstalhood.com/vmware-unified-access-gateway/)
- [Replace the Default TLS/SSL Server Certificate for Unified Access Gateway](https://docs.vmware.com/en/Unified-Access-Gateway/3.1/com.vmware.uag-31-deploy-config.doc/GUID-EDC244DD-07AB-4841-A893-84ADF8D59838.html)
- [UAG SAML Metadata File](https://docs.vmware.com/en/Unified-Access-Gateway/3.3.1/com.vmware.uag-331-deploy-config.doc/GUID-2A689F41-0A6A-4F41-A898-C286DFD70C85.html)
- [UAG Multiple NICs](https://communities.vmware.com/docs/DOC-32926)
- [Load Balancing](https://communities.vmware.com/docs/DOC-32792)


*Troubleshooting*

- [Connection Problems Between Horizon Client and the PCoIP Secure Gateway](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-virtual-desktops/GUID-5117AC00-79FC-4A74-8234-014C157A17F6.html)

#### View Connection Server

- [Installation Pre Requisites - Horizon 7-7.8](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-installation/GUID-68621B8E-F018-4BC4-811A-5CF76B55DB2C.html)
- [Installation - Carl Stalhood](https://www.carlstalhood.com/vmware-horizon-7-connection-server/)
	- Does require load balancing for multiple View Connection Servers
- Hardware
	- 4 CPUs
	- 10 GB MEM
	- 100 GB Disk
- Connections
	- Horizon 7.2 and newer: 4000 connections
	- Horizon 7.1 <= x < 7.2: 2000 connections
- [Creating Single-User Desktop Pools](https://techzone.vmware.com/quick-start-tutorial-series-vmware-horizon-7/creating-single-user-desktop-pools#915877)
- [Allow HTML Access Through a Gateway](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-installation/GUID-FE26A9DE-E344-42EC-A1EE-E1389299B793.html?hWord=N4IghgNiBcIQ9gYwNYFMAmA6ADgJ3tqrgC4CWqAzgAQDmYxqA7mAJ4gC+QA)  

	Connection Server instances and security servers that are directly behind a gateway, such as Access Point, must know the address by which browsers will connect to the gateway when users use HTML Access.

	For Connection Server instances and security servers that are behind a load-balancer or load-balanced gateway, perform the procedure described in [Allow HTML Access Through a Load Balancer](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-installation/GUID-BFF2E726-A5EB-4105-A0EA-F3D718C5880E.html#GUID-BFF2E726-A5EB-4105-A0EA-F3D718C5880E).

	1. Go to the following directory: `C:\Program Files\VMware\VMware View\Server\sslgateway\conf\`
	1.	Create the following document in this location `locked.properties`.
	2.	Add the `checkOrigin=false` property and add the address of the UAG similar to the below.
	3.	Restart the Connection server service.

- [Modify the listed domains in Horizon Console, HTML Access, and Horizon Client](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-administration/GUID-3E9924EC-1554-43E5-A812-84F9711909A5.html)

	Make sure to either launch PowerShell as an admin or pass credentials with the `-b` flag.

	- List the domain configuration  
		`vdmadmin -N -domains -list`

	- Add a domain to the include list
		`vdmadmin -N -domains -include -domain <your_domain> -add`

	- `-s conn_server` Specifies that the operation applies to the domain filters on a Connection Server instance. You can specify the Connection Server instance by its name or IP address.

		If you do not specify this option, any change that you make to the search configuration applies to all Connection Server instances in the group.

	- Make sure to go back into the Horizon Admin (Console) and enable the check box `Send Domain List` under **View Configuration > Global Settings > General**
		- This option will not show up if at least one domain is not in the list.
- VDI Machine Naming
	- [Provide a List of names and user assignments](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-virtual-desktops/GUID-F9A7022F-6CB0-482E-9D72-C912F117C240.html)

*Desktop Pools*

- [Carl Stalhood - VMware Horizon 7 – Virtual Desktop Pools](https://www.carlstalhood.com/vmware-horizon-7-virtual-desktop-pools/)
- [Pool Creation - Carl Stalhood](https://www.carlstalhood.com/vmware-horizon-7-virtual-desktop-pools/#prep)

*Errors*

- [Accessing the Horizon View Administrator page displays a blank error window in Horizon 7 (2144768)](https://kb.vmware.com/s/article/2144768)

#### Database Information

- [Configuring Event Reporting - v7-7.10]https://docs.vmware.com/en/VMware-Horizon-7/7.10/horizon-installation/GUID-F6075DF0-9614-4A81-B27A-7EE7C4CCB46F.html)
- [Create the ViewEvent Database - Horizon 7.7-8](https://www.virtuallyboring.com/vmware-horizon-view-7-create-events-database/)


#### Persona Management

- [Configuring a Horizon Persona Management Deployment](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-virtual-desktops/GUID-E9411421-EE62-4870-98CA-ADEE7B70EB32.html)
- [Best Practices for Configuring a Horizon Persona Management Deployment](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-virtual-desktops/GUID-574E2280-E796-4946-8CE4-6617683B5BE3.html)
- [Providing User Personas in Horizon 7 - Horizon 7.8](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-virtual-desktops/GUID-F9F1320A-F6BC-4120-8A8D-2D5F73F79335.html)
- [Using Horizon Persona Management to Retain User Data and Settings - Horizon 7 7.8](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-architecture-planning/GUID-05B1BE12-8DD2-4EAE-A3E2-B52CDB6DFC32.html)
- [Horizon Persona Management and Windows Roaming Profiles](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-virtual-desktops/GUID-E158A9D4-5FCD-4A61-B987-D01622A96FBF.html)


#### View Composer

*View Composer Database*

- [Prepare View Composer DB](https://docs.vmware.com/en/VMware-Horizon-7/7.0/com.vmware.horizon-view.installation.doc/GUID-4CF63F93-8AEC-4840-9EEF-2D60F3E6C6D1.html)
- [Event DB Sizing](http://myvirtualcloud.net/vmware-view-database-sizing/)


#### vSAN

- [Design and Sizing - 2014](https://www.vmware.com/content/dam/digitalmarketing/vmware/en/pdf/whitepaper/products/vsan/vmw-tmd-virt-san-dsn-szing-guid-horizon-view-white-paper.pdf)


#### Active Directory

- [Preparing AD for Horizon - Horizon 7.8](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-installation/GUID-F6075DF0-9614-4A81-B27A-7EE7C4CCB46F.html)
- [Accounts and Permissions - Horizon 7](https://thevirtualhorizon.com/2016/08/08/horizon-7-0-part-6-service-accounts-and-databases/)


#### Tools

- [OS Optimization Tool](https://labs.vmware.com/flings/vmware-os-optimization-tool)
- [Horizon 7 Component Installers](https://my.vmware.com/web/vmware/info?slug=desktop_end_user_computing/vmware_horizon/7_0)
- [ESXi Configuration Maximums](https://kb.vmware.com/s/article/1003497)
- [Health Analyzer](https://vmware.my.salesforce.com/apex/page?name=sales.services.software.solutions)
- [Interoperability Matrix](https://www.vmware.com/resources/compatibility/sim/interop_matrix.php)
- [Digital Workspace Topology Tool](https://tools.techzone.vmware.com/static/topology/index.html#result)
	- [Blog Post](https://blogs.vmware.com/euc/2019/02/introducing-the-vmware-digital-workspace-topology-tool.html?src=so_5a314d05e49f5&cid=70134000001SkJn)
- [Digital Workspace Designer](https://code.vmware.com/group/dp/dwdesigner#)


#### User Account Information

- [Horizon 7 User Accounts - 7-7.10](https://docs.vmware.com/en/VMware-Horizon-7/7.10/horizon-security/GUID-7C94B12F-0158-42EB-A011-00CC4912A435.html?hWord=N4IghgNiBcIBYHsBOBLAXggdgAgOzYFcBnAUyWzAGNKEDMAXIkAXyA)
- [vCenter Server User for Horizon 7 and View Composer - 7.11](https://docs.vmware.com/en/VMware-Horizon-7/7.11/horizon-installation/GUID-80D653FA-BCC0-45B9-AF84-5E0EEC2AD139.html)
	- [vCenter Server Role Permissions - 7-7.11](https://docs.vmware.com/en/VMware-Horizon-7/7.11/horizon-installation/GUID-A878F876-B359-42FC-9124-A1E34BFB3319.html)
- [View Composer and Instant Clone Privileges Required for the vCenter Server User - 7-7.10](https://docs.vmware.com/en/VMware-Horizon-7/7.10/horizon-installation/GUID-467F552F-3034-4917-A985-B5E5FEC5C68F.html)
- [Instant Clone Operations User Account - 7-7.8](https://docs.vmware.com/en/VMware-Horizon-7/7.8/horizon-installation/GUID-E91881F4-F8C0-48A5-A1A4-61577E287E29.html)


#### Troubleshooting

- [Provisioning View desktops fails due to customization timeout errors (2007319)](https://kb.vmware.com/s/article/2007319) - No longer required after 2018/12/17

- Issues with Sysprep & Customization

	- Guest Customization log: `C:/Windows/TEMP/vmware-imc/guestcust.log`
	- Sysprep Log: `C:\Windows\System32\Sysprep\Panther\setupact.log`

- [Horizon 7 Log Files](https://docs.vmware.com/en/VMware-Horizon-7/7.10/horizon-security/GUID-79A2A422-AF18-41BC-B15F-0117DBB10CCC.html	)
