# Reference List

This is where I put handy links, commands, 3rd party resources, documentation links, etc that I have found helpful in my technology journey

Referenced often, Updated simi-regularly :)

<a name="top"></a>

## TOC

1. [Apple  ](#macintosh)

	1. [Tools](#macos_tools)
	2. [Handy Sites](#macos_sites)
	3. [Handy Terminal Commands](#macos_commands)
	4. [Documentation](#macos_documentation)
	5. [Apple Device Automation](#apple_device_automation)
	6. [Networking & Wi-Fi](#macos_network_and_wifi)
	7. [Security](#macos_security)
	8. [Encryption & FileVault](#macos_encryption_and_fv)
	9. [Apple Device Automation](#apple_device_automation)
	10. [Support](#apple_support)

1. [Unix & GNU/Linux](#unix_linux)
1. [Windows](#windows)

    1. Tools
    2. MSFT Office
    3. Active Directory/AzureAD/LDAP
    4. OIDC & Microsoft Identity Platform
    5. SCCM Administration
    6. Image Creation
    7. Handy Commands
    8. [Reset IE Settings](#reset_ie_settings)
    8. Error Codes

1. [MDM](#mdm)

	1. [Apple](#mdm_apple_apns)
	1. [Jamf](#mdm_jamf)
	2. [WorkspaceONE](#mdm_wso)
	3. [MSFT Device Manager](#mdm_msft_device_manager)
	3. [Mobile Iron](#mdm_mobile_iron)
	4. [Google Enterprise](mdm_google_enterprise)

1. [Identity & Access Management](#idam)

    1. [WorkspaceONE Access](#idam_wso_access)

1. [Virtualization](#virtualization)

    1. VMware Horizon

1. [Certificate Information](#cert_information)
1. [Scripting & Development](#scripting-and-languages)

    1. [Code Signing](@scripting_code_signing)
    1. Git
    1. [Python](#python)
    1. [Swift](#swift_code)
    1. [Bash](#bash)
    1. [Vim](#vim)
    2. [VSCode](#vscode)
    1. [Atom](#atom)
    1. [Markdown](#markdown)
    2. RegEx
    3. PowerShell
    4. sed

1. Software

    1. Opera Browser Settings

1. Security

    1. Handy Commands

<a name="macintosh"></a>

## Related to Apple Macintosh Support & Administration

<a name="macos_tools"></a>

### Tools

- [Packages](http://s.sudre.free.fr/Software/Packages/about.html): Awesome package creator
	- [User Guide](http://s.sudre.free.fr/Software/documentation/Packages/en_2017/index.html)
- [iMazing Profile Editor](https://imazing.com/profile-editor) - iMazing Profile Editor lets you create, edit, and sign Apple configuration profiles. Define settings with ease, ready to be deployed locally or via MDM to fleets of iPhones, iPads, Macs, and other Apple devices.

    - [Manifests](https://github.com/ProfileCreator/ProfileManifests/tree/master/Manifests)

- [AutoPkg](https://autopkg.github.io/autopkg/) - AutoPkg is a system for automatically preparing software for distribution to managed clients. Recipes allow you to specify a series of simple actions which combined together can perform complex tasks, similar to Automator workflows or Unix pipes.

	- [recipe-robot](https://github.com/homebysix/recipe-robot): help create AutoPkg 
recipes.

- [Suspicious Package](http://www.mothersruin.com/software/SuspiciousPackage/get.html): look inside of packages. 
- [PPPC Utility (Jamf)](https://github.com/jamf/PPPC-Utility) - PPPC Utility is a macOS (10.13 and newer) application for creating configuration profiles containing the Privacy Preferences Policy Control payload for macOS. The profiles can be saved locally signed or unsigned. Profiles can also be uploaded directly to a Jamf Pro server.
- (NO LONGER DEVELOPED)[Profile Creator](https://github.com/ProfileCreator/ProfileCreator) - macOS application to create configuration profiles.
- [Payload-Free-Package-Creator](https://github.com/rtrouton/Payload-Free-Package-Creator): when you want to just dumb a script somewhere.
- [Google Santa](https://github.com/google/santa): Application blacklisting
- [DEPNotify](https://gitlab.com/Mactroll/DEPNotify): Simple tool to display
    what is happening during DEP enrollment on the Mac.

    - [cannonball](http://cannonball.tombridge.com/2017/04/27/getting-started-with-installapplication-depnotify-and-simplemdm/)

- [mac-ibm-enrollment-app](https://github.com/IBM/mac-ibm-enrollment-app) - The Mac@IBM enrollment app makes setting up macOS with Jamf Pro more intuitive for users and easier for IT. The application offers IT admins the ability to gather additional information about their users during setup, allows users to customize their enrollment by selecting apps or bundles of apps to install during setup, and provides users with next steps when enrollment is complete.

- [SplashBuddy](https://github.com/Shufflepuck/SplashBuddy) - SplashBuddy goal is to provide an elegant and secure onboarding process for Mac users using DEP.
- [ManagedMac](http://dayglojesus.github.io/managedmac/) - puppet plugin for managing mac.
- [Dock Master](https://github.com/Error-freeIT/Dock-Master) - Dock Master is a tool for generating dock profiles and dock packages.
- [mas-cli](https://github.com/mas-cli/mas): App Store from the CLI    
- [NoMAD](https://nomad.menu/downloads/ "No More Active Directory"): Active
    Directory broker client. OpenSource alt to Apple's Enterprise Connect
    service
- [AutoDMG](https://github.com/MagerValp/AutoDMG) - The award winning AutoDMG takes a macOS installer (10.10 or newer) and builds a system image suitable for deployment with Imagr, DeployStudio, LANrev, Jamf Pro, and other asr-based imaging tools.
- [precache](https://github.com/krypted/precache) - Pull updates down top the
    Apple macOS Server Caching service.
- [MCXToProfile](https://github.com/timsutton/mcxToProfile) - mcxToProfile is a simple command-line utility to create "Custom Settings" Configuration Profiles without the need for the Profile Manager Device Management service in OS X Server 10.7 and 10.8.
- [Automator](https://configautomation.com)
- [Apple Configurator 2](https://help.apple.com/configurator/mac/2.0/) - Apple Configurator 2 makes it easy to deploy iPad, iPhone, iPod touch, and Apple TV devices in your school or business.
- [EraseInstall](https://bitbucket.org/prowarehouse-nl/erase-install/src/master/) - EraseInstall.app for macOS is designed to allow users to easily erase the HD on their Mac and install a fresh copy of macOS. The application is a wrapper around the command `startosinstall`.
- [InstallApplications](https://github.com/erikng/installapplications):
    dynamically download packages for use with `InstallApplication` 
- [Recipe Robot](https://github.com/homebysix/recipe-robot) - Recipe Robot is the easiest way to create new AutoPkg recipes for simple Mac apps.
- [vfuse](https://github.com/chilcote/vfuse) - Takes a never-booted DMG and converts it to a VMware Fusion VM.    

<a name="macos_sites"></a> 

### Handy Sites

- [http://www.getmacapps.com](http://www.getmacapps.com)
- [macadmins.software](macadmins.software)
- [https://derflounder.wordpress.com](https://derflounder.wordpress.com)
- [iOS Release Versions](https://en.wikipedia.org/wiki/IOS_version_history)
    

<a name="macos_commands"></a>

### Handy Commands

- Query LDAP

	- Example directory domain

		`dirservices.example.com`
		
	- Example query

		Return container where the user exists

		`ldapsearch -h dirservices.example.com -x -b "dc=dirservices,dc=example,dc=com" "uid=user_name_searched_for"`
		
		Only look in the 'users' CN
		
		`ldapsearch -h dirservices.example.com -x -b "cn=users,dc=dirservices,dc=example,dc=com" "uid=user_name_searched_for"`
		
		Return all users in the "Everyone" group
		
		`ldapsearch -h dirservices.example.com -x -b "cn=Everyone,dc=dirservices,dc=example,dc=com"`
		
	- Flags

		**-h**: hostname for the directory services server.  
		**-b**: search base (base DN).  
		**-p**: define a none standard port if one is being used.  
		**-x**: sorts the results on the server before sending them to the client.  
		**-z**: Limit the number of results returned.  
		**-l**: Specify amount of time to allow the query to run.
		**-W**: prompt for password
		

- Grab macOS installers

	Note: Only works in Catalina.

	`sudo softwareupdate --fetch-full-installer`
	`sudo softwareupdate --fetch-full-installer --full-installer-version 10.15.1`
	
	- This one works for downloading older "signed" versions of macOS as well. 

- Show `failedLoginCount` for a user
	
	`dscl . -readpl /Users/<user_name> accountPolicyData failedLoginCount`
	
- Reset `failedLoginCount` setting

	`dscl . -deletepl /Users/<user_name> accountPolicyData failedLoginCount`

- Read & Write Apple language preferences

	`defaults read -g AppleLocale`
	`defaults read -g AppleLanguages`
	`defaults read NSGlobalDomain AppleLanguages`
	`defaults write NSGlobalDomain AppleLanguages "(en-AU)"`
	
	[Retrieving the languages in Terminal](https://developer.apple.com/library/archive/qa/qa1391/_index.html)

- Show all ARP table entries

	`arp -a`

- Force unbind from AD domain

	`sudo dsconfigad -force -remove -u johndoe -p nopasswordhere`
	
- Generate a random UUID

	`uuidgen | tr "[:upper:]" "[:lower:]"`
	
- Sign a package with a developer ID installer cert

	`productsign --sign “Developer ID Installer: Your Developer Name (1A2B3C4D5E)” ~/Desktop/example.pkg ~/Desktop/signed-example.pkg`
	
- Remove GateKeeper restrictions

	`sudo spctl --master-disable`
	
- Clear passcode profile settings
	
	`sudo pwpolicy -clearaccountpolicies`
	
- Boot macOS in Verbose Mode

    `sudo nvram boot-args="v"`


<a name="macos_documentation"></a>

### Documentation

#### Apple KBs

- [HT201407 - If you can't activate your iPhone](https://support.apple.com/en-us/HT201407)
- [HT208643 - APNS Support Doc](https://support.apple.com/en-us/HT208643)
- [HT201260 - macOS Builds](https://support.apple.com/en-us/HT201260)
- [HT201255 - Mac Startup Cmd Options](https://support.apple.com/en-us/HT201255)
- [HT201853 - Apple Video Adapters and Cables](https://support.apple.com/en-us/HT201853 "About Apple Video Adapters and Cables")
- [HT208987 - About Activation Lock on your Mac](https://support.apple.com/en-us/HT208987)
    - [Activation Lock](https://support.apple.com/guide/mdm/activation-lock-apd593fdd1c9/web)


#### White Papers

- APNS
	- [Apple Developer - APFS](https://developer.apple.com/library/content/documentation/FileManagement/Conceptual/APFS_Guide/Introduction/Introduction.html#//apple_ref/doc/uid/TP40016999-CH1-DontLinkElementID_19)
	- [Apple Developer - APNS - API](https://developer.apple.com/library/archive/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/CommunicatingwithAPNs.html#//apple_ref/doc/uid/TP40008194-CH11-SW1)
	- [Apple Developer - APNS - Overview](https://developer.apple.com/library/archive/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/APNSOverview.html#//apple_ref/doc/uid/TP40008194-CH8-SW1)
- [GameplayKit](https://developer.apple.com/documentation/gameplaykit)
- [Kerberos Extension](https://developer.apple.com/documentation/devicemanagement/extensiblesinglesignonkerberos/extensiondata)
- [System Extensions](https://developer.apple.com/system-extensions/)


#### Other

- [Apple Document Style Guide](https://help.apple.com/applestyleguide/#/apsg3acde405)
- [Apple Open Source Documentation](https://opensource.apple.com/)
- [Installing Beta Software](https://developer.apple.com/support/install-beta/)
- [keyboard shortcuts](http://support.apple.com/kb/HT1343 )
- Launchd Documentation
	- `man launchd.plist` - to see a full list of keys available to daemons/agents.
	- ~/Library/LaunchAgents         Per-user agents provided by the user.
	- /Library/LaunchAgents          Per-user agents provided by the administrator.
	- /Library/LaunchDaemons         System-wide daemons provided by the administrator.
	- /System/Library/LaunchAgents   Per-user agents provided by OS X.
	- /System/Library/LaunchDaemons  System-wide daemons provided by OS X.

- [Apple software Restore (ASR)](https://en.wikipedia.org/wiki/Apple_Software_Restore)
- [Disabled Accounts](https://www.jamf.com/jamf-nation/discussions/18243/password-policy-profile-disables-user-account)
- [Setting Printer Options Via CLI](http://www.brunerd.com/blog/2012/03/13/getting-and-setting-ppd-options-via-command-line-for-use-with-lpadmin-in-os-x/)


#### MDM Protocol Related

- [Apple MDM Documentation](https://developer.apple.com/library/content/documentation/Miscellaneous/Reference/MobileDeviceManagementProtocolRef/3-MDM_Protocol/MDM_Protocol.html#//apple_ref/doc/uid/TP40017387-CH3-SW2)
- [Configuration Profile Reference](https://developer.apple.com/business/documentation/Configuration-Profile-Reference.pdf)
- [Apple Profile Manager](http://help.apple.com/profilemanager/mac/5.4/#/apd5BD57F16-A2BF-43B9-AB4B-24948FB52C1E)
- [Apple Configurator 2](http://help.apple.com/configurator/mac/2.0/)
- [MacOS Deployment Reference](https://help.apple.com/deployment/macos/#/ior5d40635d0)


### Apple Business Manager

- [What are Managed Apple IDs in Apple Business Manager?](https://support.apple.com/guide/apple-business-manager/what-are-managed-apple-ids-tes78b477c81/1/web/1)
- [Create Managed Apple IDs in Apple Business Manager](https://support.apple.com/guide/apple-business-manager/create-managed-apple-ids-mdm1c9622977/web)
- [Configure federated authentication with Microsoft Azure AD for Apple Business Manager](https://support.apple.com/guide/apple-business-manager/configure-federated-authentication-microsoft-apdc9611d0e0/1/web/1#apddc46155ee)
- [Add federated domains in Apple Business Manager](https://support.apple.com/guide/apple-business-manager/add-federated-domains-apdf867462bc/1/web/1)
- [Intro to federated authentication with Apple Business Manager](https://support.apple.com/guide/apple-business-manager/intro-to-federated-authentication-apdb19317543/1/web/1)


<a name="macos_network_and_wifi"></a>

### Networking & Wi-Fi

- [HT210060 - Use Apple products on enterprise networks](https://support.apple.com/en-us/HT210060)
- [HT201999 - About macOS, iOS, and iTunes server host connections and iTunes background processes](https://support.apple.com/en-us/HT201999)
- [Connet to a Wireless Network from CLI](http://osxdaily.com/2011/04/12/connect-wireless-network-command-line/)
- [802.1x](https://www.esecurityplanet.com/views/article.php/3899996/How-to-Use-Enterprise-WiFi-Encryption-and-8021X-in-Mac-OS-X.htm)
- [Port Specifications for Apple Services](https://support.apple.com/en-us/HT202944)


<a name="macos_security"></a>

### Security

- [Apple Platform Security - 2019](https://manuals.info.apple.com/MANUALS/1000/MA1902/en_US/apple-platform-security-guide.pdf)
- [App security overview](https://support.apple.com/guide/security/app-security-overview-sec35dd877d0/1/web/1)
- [Product security certifications, validations, and guidance for SEP: Secure Key Store](https://support.apple.com/en-us/HT209632)
- [NIST - Apple Security](https://github.com/usnistgov/applesec)  

    This page contains supplemental resources to NIST Special Publication (SP) 800-179 Revision 1, Guide to Securing macOS 10.12 Systems for IT Professionals: A NIST Security Configuration Checklist. The publication is located at https://csrc.nist.gov/publications/detail/sp/800-179/rev-1/draft.
Please send any comments to 800-179comments@nist.gov.

- [CIS Benchmark - Apple](https://www.cisecurity.org/benchmark/apple_os/)
- [Sudoers Modification](https://derflounder.wordpress.com/2016/07/11/editing-etcsudoers-to-manage-sudo-rights-for-users-and-groups/)

- PPPC

	- [Derflounder](https://derflounder.wordpress.com/2018/08/31/creating-privacy-preferences-policy-control-profiles-for-macos/)

- Approving KEXTs

	- [Derflounder](https://derflounder.wordpress.com/2018/04/12/whitelisting-third-party-kernel-extensions-using-profiles/)
	- [Vendor KEXT Info](https://docs.google.com/spreadsheets/d/1IWrbE8xiau4rU2mtXYji9vSPWDqb56luh0OhD5XS0AM/edit#gid=0)

- SysEXT

- [Making Changes to the authorizationdb](https://derflounder.wordpress.com/2014/02/16/managing-the-authorization-database-in-os-x-mavericks/) 

	- `security authorizationdb read <system.preferences.[preferencez_setting_name>`
	- `security authorizationdb read referenced.rights > /path/to/filename.plist`
	- `security authorizationdb write system.preferences allow`
	- `security authorizationdb write system.preferences.startupdisk allow`

- The `security` command

	- Find a specific keychain item by name
		`security find-generic-password -l Hermes`


<a name="macos_encryption_and_fv"></a>

### Encryption & FileVault

- [Manage FileVault with `fdesetup`](https://derflounder.wordpress.com/2015/12/20/managing-el-capitans-filevault-2-with-fdesetup/)
- [FileVault Institutional Recovery Keys - DerFlounder](https://derflounder.wordpress.com/2014/08/13/filevault-2-institutional-recovery-keys-creation-deployment-and-use/)


<a name="apple_device_automation"></a>

### Automation

- [ConfigAutomation](https://configautomation.com/)  
    - [Supervision Identities](https://configautomation.com/identity-files.html)
    - [APU Doc](https://configautomation.com/apu)
- IPSW Download location
	`$HOME/Library/Group\ Containers/K36BKF7T3D.group.com.apple.configurator/Library/Caches/Downloads/ACUDownloadFileOperation/`
	`$HOME/Library/Group\ Containers/K36BKF7T3D.group.com.apple.configurator/Library/Caches/Firmware/`
- Device STUB File Location

	`$HOME/Library/Caches/com.apple.configurator.AttachedDevices`


<a name="apple_support"></a>

### Support

- [ABM Support Numbers](https://help.apple.com/businessmanager/?lang=en-us#/apd098f3d709)
- [Check Apple Services](https://www.apple.com/support/systemstatus/)


\[[top](#top)]

<a name="unix_linux"></a>

## Unix & GNU/Linux

-   [Sane scanner](https://wiki.archlinux.org/index.php/SANE)
-   [Linux Journey](https://linuxjourney.com/lesson/etc-group-file)
-   netboot.xyz
-   Banking with a live cd: <http://krebsonsecurity.com/2012/07/banking-on-a-live-cd/>
-   SSH Tricks: <http://www.linuxjournal.com/article/6602>
-   Rsync command examples - <http://www.thegeekstuff.com/2010/09/rsync-command-examples/>
-   POSIX - <https://en.wikipedia.org/wiki/POSIX>
-   Security Enhanced Linux: <http://selinuxproject.org/page/Main_Page>
-   Cool old terminal - old looking terminal for linux: <http://linuxg.net/how-to-install-cool-old-term-0-9-on-ubuntu-14-04-debian-jessie>


### ZSH

- Change the keybindings back to EMACS by adding the following to `.zshrc`

	`bindkey -e`

\[[top](#top)]


## Related to Windows Administration

- [sway.office.com](https://sway.office.com/leB5lmZDQsxnrMAv?ref=Link)
- List of WMIC CSProduct Get Name Results - <http://faqshop.com/misc/list-of-wmic-csproduct-get-name-results/>
- [Troubleshooting Slow Logons via PowerShell](https://www.citrix.com/blogs/2015/08/05/troubleshooting-slow-logons-via-powershell/)
- [Logon GPO Analysis via PowerShell](https://www.controlup.com/blog/logon-gpo-analysis-via-powershell/)
- [Windows 10 Environment Variables](https://www.tenforums.com/tutorials/3234-environment-variables-windows-10-a.html)
- [Install RSAT - Win10 1809](https://www.prajwaldesai.com/install-rsat-tools-on-windows-10-version-1809/)


### Tools

- [Windows ISO Downloader](https://heidoc.net/joomla/technology-science/microsoft/67-microsoft-windows-and-office-iso-download-tool)
- [GPO Migration Tool](https://code.vmware.com/samples/3527/airwatch-gpo-migration-tool?h=gpo%20migration%20tool)


### MSFT Office

- [Change Native Language](https://www.jamf.com/jamf-nation/discussions/25722/changing-languages-in-office-2016)

	```shell
	defaults write com.microsoft.Excel AppleLanguages ‘(“ES”)’
	defaults write com.microsoft.Powerpoint AppleLanguages ‘(“ES”)’
	defaults write com.microsoft.Word AppleLanguages ‘(“ES”)’
	```
	
- [macadmins.software](https://macadmins.software)
	- [Outlook Preferences](https://docs.microsoft.com/en-us/DeployOffice/mac/preferences-outlook)
	- [OneDrive Preferences](https://docs.microsoft.com/en-us/onedrive/deploy-and-configure-on-macos)
- [Mac Office 2011 Rem Tool](https://github.com/pbowden-msft/Remove2011/blob/master/Remove2011)
- [Office One-click login - Jamf](https://www.jamf.com/blog/help-users-activate-microsoft-office-365-and-configure-outlook-in-one-click/)
- [MacOS Word Keyboard Shortcuts](https://support.office.com/en-us/article/Keyboard-shortcuts-in-Word-for-Mac-3256d48a-7967-475d-be81-a6e3e1284b25)
	- Page Break - `⌘ + Return`
	- Paste and Match Style - `⌘ + ⌥ + ⇧ + V`
- [MacOS Excel Keyboard Shortcuts](https://support.office.com/en-us/article/Keyboard-shortcuts-in-Excel-for-Mac-acf5419e-1f87-444d-962f-4e951a658ccd)
	- AutoFit Width - `⌥ + H + O + I` - in sequence. Not at the same time
	- AutoFit Height - `⌥ + H + O + A` - in sequence. Not at the same time

### Active Directory/AzureAD/LDAP

- Objects
	- CN = Common Name
	- OU = Organizational Unit
	- DC = Domain Component
- Example Search Criteria
	- ("CN=Dev-India,OU=Distribution Groups,DC=gp,DC=gl,DC=google,DC=com");


#### AzureAD

- Password Hash Synchronization with AzureAD

	- [What is password hash synchronization with Azure AD?](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-phs)
	- [What is federation with Azure AD?](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-fed)

- [AzureADv1 Error Codes](https://docs.microsoft.com/en-us/azure/active-directory/develop/reference-aadsts-error-codes)
- [AzureADv2 Error Codes](https://docs.microsoft.com/en-us/azure/active-directory/develop/reference-aadsts-error-codes)


### OIDC & Microsoft Identity Platform

- [Identity Platform](https://docs.microsoft.com/en-us/azure/active-directory/develop/about-microsoft-identity-platform)
	- [2.0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-overview)
- [Microsoft identity platform and OpenID Connect protocol](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-protocols-oidc)


\[[top](#top)]

### SCCM Administration

-   [SCCM Queries with PowerShell](http://blog.ctglobalservices.com/powershell/kaj/working-with-queries-in-configmgr-with-powershell/)

-   [WMI SCCM Queries](https://www.andersrodland.com/ultimate-sccm-querie-collection-list/)

-   Convert from BIOS to UEFI Using SCCM - <https://www.systemcenterdudes.com/sccm-bios-uefi-conversion-task-sequence>

    -   Another Article regarding Bios to UEFI conversion - <https://docs.microsoft.com/en-us/sccm/osd/deploy-use/task-sequence-steps-to-manage-bios-to-uefi-conversion>

-   Deploy Windows from Captured Media -  <https://blogs.technet.microsoft.com/configurationmgr/2010/04/12/how-to-set-up-a-task-sequence-to-deploy-windows-7-images-captured-via-an-sccm-2007-capture-cd/>

-   Driver management - <https://technet.microsoft.com/en-us/library/hh301101.aspx>


### Image Creation

- [ngen.exe](https://docs.microsoft.com/en-us/dotnet/framework/tools/ngen-exe-native-image-generator)
- [DISM](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/what-is-dism)
- [Win10 Sysprep](https://theitbros.com/sysprep-windows-10-machine-guide/)
- [cleanmgr.exe](https://support.microsoft.com/en-us/help/253597/automating-disk-cleanup-tool-in-windows)
- [Sdelete Tool](https://docs.microsoft.com/en-us/sysinternals/downloads/sdelete)
- [OS Optimization Tool](https://labs.vmware.com/flings/vmware-os-optimization-tool)


### Handy Commands

- Get windows version

	`systeminfo | findstr /B /C:"OS Name" /C:"OS Version"`
	

- Import a Root Cert into Local Trusted CAs

	1. Download and save the certificate.
	1. Open the Certificate Manager
	1. Hit Windows+R, or click on the Blue Vista icon in the lower left hand corner
	1. In the "Start Search" box, type "certmgr.msc" (no quotes).
	1. The certificate manager will open.
	1. Right click on "Trusted Root Certification Authorities" from the folder list on the left.
	1. In the pop-up menu, choose "All Tasks" >> "Import.."
	1. Click the "Next" button
	1. Click the "Browse" button
	1. Browse to the location where the certificate is saved, click on it then click the "Open" button
	1. Click the "Next" button
	1. Select "Place all certificates in the following store"
	1. Click the "Browse" button
	1. Put a checkmark beside "Show physical stores"
	1. Expand the "Trusted Root Certification Authorities" folder
	1. Click "Local Computer"
	1. Click the "OK" button.
	1. Click the "Next" button
	1. Click the "Finish" button

<a name="reset_ie_settings"></a>

### Reset Internet Explorer

If IE security settings are blocking you from downloading a file use the following steps to reset the security settings.

1. Open Control Panel
2. Select **Networking**
3. Under **Internet Options** click **Manage Browser Add-ons**. This will bring up Internet Properties.
4. Select the **Security** tab and click **Reset all zones to default** and follow any prompts should they appear.
5. Select the **Advanced** tab and click the **Reset** button. A dialogue may come up asking to close all applications.
6. Open **Task Manager** and clock any of the Internet Explorer processes.
7. Close the Task Manager.
8. Go back to the **Internet Properties** window and reset the defaults again and do the same on the Advanced tab again.


### Error Codes

- 0x80070422 - restart the windows update service
- The trust relationship between this workstation and the primary domain failed.
	- Un Bind/Bind

\[[top](#top)]


<a name="mdm"></a>

## MDM

<a name="mdm_apple_apns"></a>

### Apple

- [MacOS WiFi Login Window Profile]( https://ntsystems.it/post/joining-wifi-before-login-on-mac-os-x-108)
- APNS URI (Jamf --> Apple APNS)
	- api.push.apple.com | 443
	- feedback.push.apple.com* | 2196
- APNS URI (Mac Client --> Apple APNS)
	- courier.push.apple.com | 5223
	- [APNS Under the Hood](https://www.youtube.com/watch?v=E39aYd2RMdE&t=1568s)
	- 17.0.0.0/8:5223
- Additional FQDNs
	- albert.apple.com
	- iprofiles.apple.com
	- *.symcb.com
	- evintl-ocsp.verisign.com
	- evsecurer-oscp.verisign.com
- [Set a Policy Banner at Login Window](https://support.apple.com/en-us/HT202277)


#### DEP Debug

https://jamf.it/dep-debug

1. Start up the freshly-wiped Mac into single-user mode: at boot hold down CMD + S
1. Mount the boot drive as read/write: /sbin/mount -uw /
1. Enable opendirectory:
1. launchctl load /System/Library/LaunchDaemons/com.apple.opendirectoryd.plist
1. Ignore the error that is thrown and click Enter
1. Enable root password: passwd root
1. Reboot: reboot
1. When Setup Assistant is up but we haven’t yet advanced to the Remote Management pane, launch Terminal by clicking CTL + OPTION + CMD + T, then run the following:

	```bash
	su root 
	defaults write /Library/Preferences/com.apple.apsd EnableDetailedLogging -bool TRUE
	defaults write /Library/Preferences/com.apple.MCXDebug debugOutput -2
	defaults write /Library/Preferences/com.apple.MCXDebug collateLogs 1
	touch /var/db/MDM_EnableDebug
	```

1. Run the Mac through the DEP prestage enrollment as normal, once booted to the Desktop, we should find the log written to: /Library/Logs/ManagedClient/ManagedClient.log


<a name="mdm_jamf"></a>
 
### Jamf

*API Documentation*

- [API Support](http://developer.jamf.com/apis/jamf-pro-api/index)
- [New Swagger API - https://[your_url].jamfcloud.com/uapi/doc](https://[your_url].jamfcloud.com/uapi/doc/#)
- What can be manipulated
	- Enbale/disable Bluetooth


*Education*

- [Jamf 200 Course Materials](https://docs.jamf.com/education-services/resources/20190920/200_Resources.html)
- [Jamf 300 Course Materials](https://docs.jamf.com/education-services/resources/20190920/300_Resources.html)
- [Jamf 400 Course Materials](https://docs.jamf.com/education-services/resources/20190920/400_Resources.html)

*Maintenance URLs*

- [Service Status](https://status.jamf.com)
- [Jamf Pro Known Issues](https://www.jamf.com/jamf-nation/my/products/jamf-pro/known-issues)


*Network Information*

- [Ports Used](https://www.jamf.com/jamf-nation/articles/34/network-ports-used-by-jamf-pro)
- [JamfCloud IP Addresses](https://www.jamf.com/jamf-nation/articles/409/permitting-inbound-outbound-traffic-with-jamf-cloud)


*LDAP Integration*

- [JIM Install Guide](http://docs.jamf.com/infrastructure-manager/1.3.2/Installing_a_Jamf_Infrastructure_Manager_Instance.html)
    - [JIM Multi-site](https://github.com/jamf/Multi-JIM/blob/master/Multi-Instance%20JIM-Install.sh)
- [AzureAD LDAPS](https://www.jamf.com/jamf-nation/discussions/25876/a-guide-to-jss-azure-ad-integration-ldap-+-sso)    
    - [MSFT Doc: LDAPS Integration](https://docs.microsoft.com/en-us/azure/active-directory-domain-services/tutorial-configure-ldaps)
    - [MSFT Doc: Create and Configure an AD DS Instance](https://docs.microsoft.com/en-us/azure/active-directory-domain-services/tutorial-create-instance)
    - [HCS: Integrating Jamf with Azure AD LDAPS](https://hcsonline.com/support/white-papers/a-guide-to-identity-management-with-azure-active-directory-jamf-pro)
- [Okta LDAP Integration](https://travellingtechguy.eu/integrating-okta-ldap-in-jamf-pro/)

*Certificate Services Integration*

- [Jamf ADCS Connector](https://docs.jamf.com/ad-cs-connector/1.0.0/Jamf_AD_CS_Connector_Overview.html)


*Single-Sign-On*

- [Single Sign-On](http://docs.jamf.com/10.10.0/jamf-pro/administrator-guide/Single_Sign-On.html)
	- [Okta](https://www.jamf.com/jamf-nation/articles/435/configuring-single-sign-on-with-okta)
	- [ADFS](https://www.jamf.com/jamf-nation/articles/436/)
	- [Shibboleth](https://www.jamf.com/jamf-nation/articles/437/)
	- [OneLogin](https://www.jamf.com/jamf-nation/articles/438/)
	- [Ping Identity](https://www.jamf.com/jamf-nation/articles/439/)
	- [G-Suite](https://www.jamf.com/jamf-nation/articles/440/)
- [MSFT Azure AD SSO Doc](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/jamfprosamlconnector-tutorial)


*Conditional Access*

- [Conditional Access and Why it Matters](https://www.jamf.com/products/jamf-pro/microsoft/)
- [Intune Integration - Traveling Tech Guy](https://travellingtechguy.eu/jamf-pro-and-ms-azure-intune-for-macos/)
- [Integrating with Microsoft Intune to Enforce Compliance on Mac Computers Managed by Jamf Pro](https://docs.jamf.com/technical-papers/jamf-pro/microsoft-intune/10.17.0/Introduction.html)
- [Conditional Access with Azure](https://resources.jamf.com/documents/white-papers/conditional-access-going-beyond-perimeter-based-security.pdf)
- [MSFT Doc: Enforcing Conditional Access](https://docs.microsoft.com/en-us/mem/intune/protect/conditional-access-assign-jamf)
- Only applies to AAD User groups
- [MSFT Doc: Troubleshooting](https://docs.microsoft.com/en-us/mem/intune/protect/troubleshoot-jamf)



*SCEP Proxy Configuration*

- Port 443 or 80
- [Enabling SCEP in Jamf Pro](https://docs.jamf.com/technical-papers/jamf-pro/scep-proxy/10.0.0/Enabling_Jamf_Pro_as_SCEP_Proxy_for_Configuration_Profiles.html)
- [Jamf Pro SCEP Communication](https://www.jamf.com/jamf-nation/articles/488/communication-of-jamf-pro-as-scep-proxy)
- [Obtaining a SCEP Proxy Signing Certificate from a Microsoft CA Using Terminal and Uploading the Certificate to Jamf Pro](https://www.jamf.com/jamf-nation/articles/538/obtaining-a-scep-proxy-signing-certificate-from-a-microsoft-ca-using-terminal-and-uploading-the-certificate-to-jamf-pro) - using an external SCEP cert during device enrollment.
- [Video on Setting up Jamf as a SCEP Proxy](https://www.youtube.com/watch?v=jn0HTWKubFY)
- [SCEP - Microsoft CA Integration](https://www.ibm.com/support/knowledgecenter/en/SS8H2S/com.ibm.mc.doc/ce_source/concepts/ce_ca_ms_ca_int.htm)


*Extension Attributes*

- [Jamf GitHub Extension Attributes Repo](https://github.com/jamf/Jamf-Nation-Extension-Attributes)

*Misc Documentation*

- [All Product Documentation](https://www.jamf.com/resources/product-documentation/)
- [Jamf Pro Security Overview](https://www.jamf.com/resources/product-documentation/jamf-pro-security-overview/)
- [MacOS Security Checklist](https://resources.jamf.com/documents/products/documentation/macos-security-checklist.pdf)
- [Startinstall Repo](https://github.com/jamf/erase-install-webinar/wiki)

*Commands*

- `sudo jamf help -hidden` - show the hidden commands

    ```
    sudo jamf help -hidden

    Usage: jamf verb [options]

	verb is one of the following:

	canRunOnThisOSXVersion	 Prints YES if this version is compatible with this OSX version.
	encryptDisk		 Activates disk encryption on this computer
	fixPermissions		 Deprecated: You cannot execute the fixPermissions command on computers with macOS 10.12 or later.
	launchAgent		 Sends events on a per user basis to the jamf daemon.
	launchDaemon		 Performs actions in an ongoing daemon process.
	listPrinters		 Lists all the installed printers.
	logTesting		 
	mdm			 Prepares the computer for use with MDM commands.
	reenroll		 Shorcut for enroll -reenroll -archiveDeviceCertificate
	removeMdmProfile	 Removes the JAMF MDM Profile
	scheduledTask		 Create a JAMF scheduled task
	trustJSS		 Adds a trust for the JAMF CA into the System keychain.
	update			 Updates the jamf binary and related applications to the latest version from the JSS.



	Global Flags:

	-displayJSSTraffic 	 Displays the total network traffic between the jamf binary and the JSS
	-randomDelaySeconds 	 Delays a random amount of time before starting
				 Specify the maximum number of seconds as the next parameter
	-verbose 		 Shows verbose events
	-showPID 		 Prints the PID of the process



	jamf help <verb> will provide details on that verb
	```

- `sudo jamf help`

    ```
    sudo jamf help -v    

    Usage: jamf verb [options]

	verb is one of the following:

	about			 Displays information about the jamf binary
	bind			 Binds this computer to a directory service
	bless			 Blesses a System or a NetBoot Server
	changePassword		 Changes a local user's password
	checkJSSConnection	 Checks the availability of the JSS
	createAccount		 Creates a new local account on the system
	createConf		 Creates a configuration file that the jamf binary uses to find the JSS
	createHooks		 Creates and configures login/logout hooks
	createSetupDone		 Ensures the Setup Assistant does not launch immediately on the next boot
	createStartupItem	 Creates a startup script to contact the JSS
	deleteAccount		 Deletes a local account from NetInfo or the local dscl database
	deletePrinter		 Deletes a printer from the system
	deleteSetupDone		 Causes the Setup Assistant to launch on the next boot
	displayMessage		 Displays a message to the current user
	enablePermissions	 Enables permissions on a volume
	enroll			 Enrolls this computer with the JSS
	fixByHostFiles		 Fixes the ByHost files
	fixDocks		 Repairs docks that have question marks after certain OS Updates
	flushCaches		 Flush cache files for the system and/or users
	flushPolicyHistory	 Flush the policy history on the JSS
	getARDFields		 Displays the ARD Fields on a volume
	getComputerName		 Displays the computer name on a volume
	help			 Displays this message or details on a specific verb
	install			 Installs a package
	installAllCached	 Installs all packages that are cached
	listUsers		 Lists all the users on the computer
	log			 Log the IP address, action, and username to the JSS
	manage			 Enforces the entire management framework from the JSS
	mapPrinter		 Maps a printer
	mcx			 Apply Managed Preferences
	modifyDock		 Installs or removes items in all users docks
	mount			 Mounts a file share
	policy			 Checks for policies on the JSS
	reboot			 Reboots the computer
	recon			 Runs Recon to update the inventory in the JSS
	removeFramework		 Removes the JAMF Binary and associated files from the computer.
	removeSWUSettings	 Remove settings that point SWU at internal servers
	resetPassword		 Resets a local user account password. (Warning: User keychain and FileVault 2 passwords may be affected. Use changePassword when current password is known)
	runScript		 Runs a script
	runSoftwareUpdate	 Run Software Update
	setARDFields		 Sets the ARD Fields
	setComputerName		 Sets the computer name
	setHomePage		 Sets the default home page for users
	setOFP			 Sets the Open Firmware mode and password
	startSSH		 Starts the ssh server
	uninstall		 Uninstalls a package
	unmountServer		 Unmounts a file server
	updatePrebindings	 Updates the prebindings on a volume
	version			 Prints the version of this application



	Global Flags:

	-displayJSSTraffic 	 Displays the total network traffic between the jamf binary and the JSS
	-randomDelaySeconds 	 Delays a random amount of time before starting
				 Specify the maximum number of seconds as the next parameter
	-verbose 		 Shows verbose events
	-showPID 		 Prints the PID of the process



	jamf help <verb> will provide details on that verb
	```    

- `sudo jamf help policy` - see additional info about a particular command.

    ```
    sudo jamf help policy
    Password:

    Usage:	 jamf policy [-event <event>] [-username <username>] [-id <policy_id>] [-forceNoRecon]

	-event		The event or trigger that the policy is associated with in the JSS. Historical synonyms include –trigger and –action.
				Note: Running policy without an event will default to the scheduled event.
				Other events include: login, logout, startup, networkStateChange, enrollmentComplete, along with custom events.

	-username		The username to check for policies for.

	-id			The ID of the policy to be executed. Used by Casper Remote and Self Service.

	-forceNoRecon		Prevents computers from submitting inventory update when a policy is configured to update inventory.

    Return Codes: 
	 0        The policy process finished with success.
	 50       An unknown error occurred while running a policy.
	 51       An error occurred because a policy is already being executed for this event.
	 52       An error occurred while checking for policies.
	 53       An error occurred while submitting the offline policy log to Jamf Pro.
	 54       Policy execution needed to be restarted in the background because of the jamf binary update.
	 55       An error occurred while submitting the Azure Active Directory ID information file.
	 57       An error occurred while updating the jamf binary or Jamf apps.
	 60       An error occurred while enforcing the management framework.
	 300      An unknown error occurred while creating directory bindings.
	 400      Disk encryption could not be executed because the jamf binary could not obtain a disk encryption ID from Jamf Pro.
	 401      An error occurred while encrypting a disk.
	 402      An error occurred while remediating a recovery key.
	 440      An error occurred while mounting a distribution point.
	 500      An unknown error occurred while modifying a dock item.
	 501      An error occurred while modifying a dock item without contents.
	 600      An error occurred while running an inventory update.
	 700      An error occurred while manipulating a local account.
	 750      An error occurred while resetting the managed account password.
	 751      An error occurred while changing the managed account password.
	 752      An error occurred while updating the managed account password in Jamf Pro.
	 800      An error occurred because this computer does not meet the OS requirements for a package.
	 801      An error occurred while installing a package.
	 802      An error occurred while caching a package.
	 803      An error occurred while installing a cached package.
	 804      An error occurred while uninstalling a package.
	 805      An error occurred while installing all of the cached packages.
	 806      An error occurred while installing a patch package.
	 900      An error occurred while installing or uninstalling a printer.
	 911      An error occurred because the device URI was not provided.
	 912      An error occurred because the printer name was not provided.
	 913      An error occurred because the PPD file path is invalid.
	 914      The printer cannot be installed because the computer does not meet the OS requirements for that printer.
	 915      An error occurred while mapping a printer.
	 921      An error occurred while uninstalling a printer.
	 1001     An error occurred while setting an EFI password.
	 1002     An error occurred while removing an EFI password.
	 2100     An error occurred while saving an embedded script to the disk.
	 2101     An error occurred while executing a script.
	 2103     An error occurred because this computer does not meet the OS requirements for the script.
	 2200     An error occurred while installing software updates.
	 2201     An error occurred while installing software updates. There may be a proxy in place.
	 2202     An error occurred while adding a software update server.
	 2300     An error occurred while running Microsoft Device Registration.
	 2301     An error occurred because Microsoft Device Registration can only register computers when they are connected to the network.
    ```

*Errors*

- 


#### Packaging

- [Re-packaging Installer Packages](https://derflounder.wordpress.com/2013/11/03/re-packaging-installer-packages-with-packages/)
- [Package Management](https://docs.jamf.com/10.9.0/jamf-pro/administrator-guide/Managing_Packages.html)


#### Tools

- Jamf Protect
    
    - [YouTube: Introduction to Protect](https://www.youtube.com/watch?v=gsbfkCSjwxc&t=1s)`
    - [Product Page](https://www.jamf.com/products/jamf-protect/)
    - [Admin Guide](https://docs.jamf.com/jamf-protect/administrator-guide/Preface.html)
    - [Evaluation Guide]( https://docs.jamf.com/jamf-protect/evaluation-guide/Overview.html)

- [GitHub](https://github.com/jamf)

	- [DEPNotify-Starter](https://github.com/jamf/DEPNotify-Starter)

- Jamf Connect

    - [Admin Guide](https://www.jamf.com/resources/product-documentation/jamf-connect-administrators-guide/)
    - [Using FileVault with Jamf Connect Login](https://www.jamf.com/jamf-nation/articles/682/using-filevault-with-jamf-connect)
    - [Understanding Jamf Connect Authentication with Azure AD Hybrid Identity Solutions](https://www.jamf.com/jamf-nation/articles/702/understanding-jamf-connect-authentication-with-azure-ad-hybrid-identity-solutions)
    - [Understanding Jamf Connect with OpenID Connect Authentication](https://www.jamf.com/jamf-nation/articles/696/understanding-jamf-connect-with-openid-connect-authentication)
    - [Configuring Jamf Connect with Azure AD Hybrid Identity Solutions](https://www.jamf.com/jamf-nation/articles/697/configuring-jamf-connect-with-azure-ad-hybrid-identity-solutions)

	- Licensing
		- Jamf Connect Verify preferences
		- A .jamfconnectlicense file in /Library/Application Support/com.jamf.connect.verify
		- A .jamfconnectlicense file in ~/Library/Application Support/com.jamf.connect.verify
		- Note: To store the license in the preferences configuration profile, you must convert the license file to base64 format, and then use the LicenseFile key in your configuration profile.

- [NoMAD Helper](https://www.youtube.com/watch?v=fQ4Epy1J7ZU)
- [Composer User Guide](https://www.jamf.com/resources/product-documentation/composer-user-guide/)


<a name=“mdm_wso”></a>
### Workspace ONE

- [MacOS Samples](https://github.com/vmware-samples/euc-samples/tree/master/macOS-Samples)
- [AirWatch Learning Path](https://mylearn.vmware.com/mgrReg/plan.cfm?plan=47955&ui=www_edu)
- [MacOS Profile Guide](https://my.air-watch.com/help/9.1/en/Content/Platform_Guides/macOS/C/Profiles_Overview.htm?TocPath=PROFILES|macOS%C2%A0Device%20Profiles|_____0)
- [Documentation](https://resources.air-watch.com/documentation?sort=newest)
- [Munki Integration](https://support.air-watch.com/articles/360000721788)
    - [Munki teardown](http://www.aarondavidpolley.com/vmware-airwatch-munki-teardown/)
- [AW REST APIs]()
	- [Get devices from AW](https://macadminsdoc.readthedocs.io/en/master/MDM/AirWatch/AirWatch-API.html)
	- your_console.com/api/help
	- Reserved REST Chars
		- Reserved: & ( ) {} [] " <>
		- Allowed: ! @ $ % ^ *  - + | \ ' ?
- [MacOS](https://my.air-watch.com/help/9.1/en/Content/Platform_Guides/macOS/C/Profiles_Overview.htm?TocPath=PROFILES|macOS%C2%A0Device%20Profiles|_____0)
- [vSphere SDK - Python](https://github.com/vmware/vsphere-automation-sdk-python/blob/master/README.md)
- [VMware Code](https://code.vmware.com/home)
- [Azure AD DS Integration](https://blog.virtualprivateer.com/workspace-one-and-azure-ad-1/)

#### Documentation

- [Workspace ONE UEM Docs](https://docs.vmware.com/en/VMware-Workspace-ONE-UEM/1907/rn/VMware-Workspace-ONE-UEM-Release-Notes-1907.html)
- [Device Profiles](https://docs.vmware.com/en/VMware-Workspace-ONE-UEM/1908/iOS_Platform/GUID-AWT-IOS-PROFILE-OVERVIEW.html)
	- [Windows](https://docs.vmware.com/en/VMware-Workspace-ONE-UEM/1908/Windows_Desktop_Device_Management/GUID-AWT-PROFILE-OVERVIEWWD.html)
- [Console Administrator Password Policies for Shared SaaS Environments (50122050)](https://kb.vmware.com/s/article/50122050)


#### Secure Email Gateway

- KCD

	- [MIT Kerberos Documentation](https://web.mit.edu/kerberos/krb5-1.12/doc/admin/conf_files/krb5_conf.html)
	- [Kerberos Error Code: 0x7 KDC_ERR_S_PRINCIPAL_UNKNOWN](https://social.technet.microsoft.com/wiki/contents/articles/2064.kerberos-error-code-0x7-kdc-err-s-principal-unknown-dsforum2wiki.aspx)
		- [Service Logons Fail Due to Incorrectly Set SPNs](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2003/cc772897(v=ws.10)?redirectedfrom=MSDN)
	- [4771(F): Kerberos pre-authentication failed.](https://docs.microsoft.com/en-us/windows/security/threat-protection/auditing/event-4771)
	- [Troubleshooting Stuff at the bottom](https://docs.vmware.com/en/VMware-Workspace-ONE-UEM/1810/WS1-Cross-Domain-KCD.pdf)
	- [Common Kerberos Errors](https://docs.oracle.com/cd/E19253-01/816-4557/trouble-6/index.html)
	- [Yet another common kerberos errors doc](https://pvtl.force.com/s/article/common-errors-and-resolutions)
	- [Table of Kerberos v5 Status Codes](https://docs.oracle.com/cd/E19683-01/816-1331/kerberrs-1/index.html)
	- [Troubleshooting Kerberos](https://docs.oracle.com/cd/E19253-01/816-4557/trouble-5/index.html)
	- [413 Error from Exchange](https://stackoverflow.com/questions/15300064/getting-413-errors-on-iis-with-concurrent-sessions-using-the-same-https-client-c)

#### Tools

- [Workspace ONE Validation Analyzer](https://docs.vmware.com/en/VMware-Workspace-ONE-UEM/9.4/vmware-airwatch-guides-94/GUID-AW94-ValidationTool.html)
- [Workspace ONE Provisioning Tool](https://labs.vmware.com/flings/vmware-workspace-one-provisioning-tool)


<a name=“mdm_msft_device_manager”></a>
### MSFT Device Manager

- [REST API](https://docs.microsoft.com/en-us/rest/api/azure/)

<a name=“mdm_mobile_iron”></a>
### Mobile Iron


<a name="mdm_google_enterprise"></a>

### Google Enterprise


#### Handy Links

- [Chrome Enterprise policy list](https://cloud.google.com/docs/chrome-enterprise/policies/#contentSettings) - definitions for chrome settings that can be managed via configuration policy.
- [About Google Cloud Directory Sync](https://support.google.com/a/answer/106368?hl=en)
- [G Suite Admin Help | Administrator Privilege Definitions](https://support.google.com/a/answer/1219251?hl=en)
- [Manage Networks](https://support.google.com/chrome/a/answer/2634553)
- [Google Chrome Enterprise Help | Set Chrome User Policies](https://support.google.com/chrome/a/answer/2657289?hl=en)
- [Google Chrome Enterprise Help | Set Chrome Device Policies](https://support.google.com/chrome/a/answer/1375678?hl=en)
- [Google Chrome Enterprise Help | Google Cloud Print Services](https://support.google.com/chrome/a/answer/3179168)
- [Google Support](https://support.google.com/)
- [Site Help pages](https://support.google.com/sites/answer/98081)
- [G Suite Help | Build your support team](https://gsuite.google.com/setup/resources/support-users/)
- [Connect to LDAP](https://support.google.com/a/answer/9089736?hl=en)


#### Commands 

- Google Enterprise Mode - `Ctrl+Alt+E`
- Wipe Device - `Esc+Refresh+Power`
	- Once in Developer Mode press - `Enter` then `Spacebar`


#### Locations to Know

- `chrome://policies` - verify that all required policies have been properly applied.
- `chrome://version` - Chrome and platform version of the affected Chrome device.


<aname="idam"></a>

## Identity & Access Management

<aname="idam_wso_access"></a>

### VMware WSO Access (formerly IDM)


- [Product Documentation vIDM](https://docs.vmware.com/en/VMware-Identity-Manager/index.html)
- [Carl Stalhood | IDM 19.03 Walkthrough](https://www.carlstalhood.com/vmware-identity-manager/)
- [Upload a New Certificate Authority for SAML Signing Certificates](https://docs.vmware.com/en/VMware-AirWatch/9.1/com.vmware.idm-administrator_aw91/GUID-A31EDEF9-5819-4C06-9A91-6E3F67566A39.html)


#### Identity Manager Connector

- [Identity Manager Deployment v3.3](https://docs.vmware.com/en/VMware-Identity-Manager/3.3/com.vmware.vidm-dmz-deployment/GUID-570583AB-1B77-422F-9916-CB2337EE6140.html)
- [Enable Outbound Mode for the Connector](https://docs.vmware.com/en/VMware-Identity-Manager/3.3/com.vmware.vidm-dmz-deployment/GUID-C97A4D37-8F1F-4B24-9A97-1A25A0033999.html)


#### APIs

- `https://insight-enterprises-inc-global.vmwareidentity.com/SAAS/jersey/manager/api/tenants/tenant/airwatchoptin/config`

#### Troubleshooting

- Health API Endpoints for vIDM and On-Prmise implementations respectively.

	`https://<idM_SERVER_NAME>/hc/API/1.0/REST/system/health?pretty`
	`https:/</idm_server_name>/SAAS/API/1.0/REST/system/health`


\[[top](#top)]
<a name="virtualization"></a>

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

<a name="cert_information"></a

## Certificate Information

- [SSL Checker with SSL Shopper](https://www.sslshopper.com/ssl-checker.html#hostname=https://awseg.foley.com) - Enter a site FQDN to see if it has a proper SSL certificate associated with it.

- Check the SSL/TLS cert using openssl

    `openssl s_client -connect example.com:443 -showcerts`
    
    This can be uploaded directly to an MDM server if using LDAPS to do queries over 636

- [Build a Concatenated PEM File](https://kb.vmware.com/s/article/2046591)
	- IDM Server PEM Cert

- Concatenate Root and Intermediate certs

	- Open a text editor
	- Copy the intermediate certs as they should appear in the chain
		- This can also be done in Terminal via the following command.
			
			```bash
			cat intermediate_cert.cer \
				intermediate_cert_2_cer \
				intermediate_cert_n \
				root_cert.cer > concatenated_cert.pfx
			```

	- Add the Root cert in last
	- Name the file with the `.pfx` file extension

- [Convert Certificate Files to One-Line PEM Format](https://docs.vmware.com/en/Unified-Access-Gateway/3.3.1/com.vmware.uag-331-deploy-config.doc/GUID-870AF51F-AB37-4D6C-B9F5-4BFEB18F11E9.html#GUID-870AF51F-AB37-4D6C-B9F5-4BFEB18F11E9)
	- UAG SAML file signing
	- IdM Appliance SAML Cert
	- vRealize

	`cat server_cert.cer key_filename.key cacerts.cer > multi_part.pem`

- Convert .cer to .pem

    `openssl x509 -in /path/to/in_file.cer -out /path/to/out_file.pem`

- [Convert P7B to PFX with OpenSSL](https://www.lisenet.com/2014/convert-p7b-to-pfx-with-openssl/) - If you need to convert from P7B to PFX make sure that you have both the certificate and the private key handy for this command sequence.

- DigiCert

	- [CSR Creation Instructions for Microsoft Servers](https://www.digicert.com/util/csr-creation-microsoft-servers-using-digicert-utility.htm) - Walks through the CSR request process using the DigiCert tool and walks through the process of exporting a Windows cert and private key from the MSFT Certificate Manager console.
	- [How to Export/Back Up Your SSL Certificate w/Private Key](https://www.digicert.com/ssl-support/certificate-pfx-file-export-import-iis-10.htm#export-pfx) - Use IIS 10 to export a copy of your SSL certificate from one server and import and configure it on a (different) Windows Server 2016

- [OpenSSL for Windows](http://slproweb.com/products/Win32OpenSSL.html)

    - `set OPENSSL_CONF=C:\OpenSSL-Win32\bin\openssl.cfg`

- [OpenSSL.org](http://www.openssl.org/)

\[[top](#top)]
<a name="scripting-and-languages"></a>

## Scripting & Development

- [HTTPS Status Code Explanations](https://httpstatuses.com/)
- [shields.io](https://shields.io)
- [Carbon - Beautiful Code Snippets](https://carbon.now.sh/T1BQoqf2hzlMLWEWAEfG)
- [Unicode Character DB](http://www.unicode.org/reports/tr44/#GC_Values_Table)


<a name="scripting_code_signing"></a>

### Code Signing

- Sign a code, plist, or mobileconfig file using a developer certificate.

	`codesign --sign "Mac Developer: Example Name (XXXXXXXXXX)" --verbose <configuration_profile_name>.mobileconfig`


### Git

- [GitHub Repo API](https://developer.github.com/v3/repos/#create)

#### Error Running Git on MacOS After Upgrade


***Error*** 

```
Avengers%: git
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun
```

***Solution***

The Mac does not have the necessary developer tools installed.

***Steps***

1. Run the following command from Terminal.app:

	```
	xcode-select --install
	```
2. You'll then receive:
	
	```
	xcode-select: note: install requested for command line developer tools
	```
	
	And be prompted in a window to update Xcode Command Line tools.
	
	![](Screenshots/git/macos-git-error.png)

3. After the update is completed, open a new terminal window and your development tools should be returned.


	**Addition**: With any major or semi-major update you'll need to update the command line tools in order to get them functioning properly again. Check Xcode with any update. This goes beyond Mojave...

4. After that restart your terminal


<a name="python"></a>

### ![](Screenshots/Python/python-icon.png) Python

-	Install `pip` python package manager MacOS - **P**ip **I**nstalls **P**ackages
	- `sudo easy_install pip`
-   For **pycodestyle** - PEP8 linter for _Atom_
    - `pip (or pip2) install pycodestyle && apm install pycodestyle`
- [Python for InfoSec](http://strategicsec.com/python-for-infosec-pros-2015/)
- [Python Naming Conventions](http://visualgit.readthedocs.io/en/latest/pages/naming_convention.html)
- [Built-in Exceptions](https://docs.python.org/3/library/exceptions.html#os-exceptions)
- [Requests Module](http://docs.python-requests.org/en/master/user/quickstart/#more-complicated-post-requests) - API Manipulation - `sudo pip install requests`
	- [HTTP Status codes](https://github.com/requests/requests/blob/master/requests/status_codes.py)
	- [Cache-Control](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control)	
- [python ldap module](https://www.python-ldap.org/en/latest/bytes_mode.html#porting-recommendations) - `pip install python-ldap`
- [Send emails](https://realpython.com/python-send-email/)
- [RealPython.com](https://realpython.com)

*PEPs*

- [PEP0440: Version Identification and Dependency Specification](https://www.python.org/dev/peps/pep-0440/)

*Learning Sites*

- [CheckIO](https://checkio.org)
- [Real Python: fstrings](https://realpython.com/python-f-strings/)
- [Real Python: Python String Formatting Best Practices](https://realpython.com/python-string-formatting/)

*Modules*

- [pyobjc-framework-SystemConfiguration 5.2](https://pypi.org/project/pyobjc-framework-SystemConfiguration/)

	Wrappers for framework ‘SystemConfiguration’.
These wrappers don’t include documentation, please check Apple’s documention for information on how to use this framework and PyObjC’s documentation for general tips and tricks regarding the translation between Python and (Objective-)C frameworks

	[Docs](https://pyobjc.readthedocs.io/en/latest/)

<a name="swift_code"></a>

### ![](Screenshots/Swift/swift_icon.png) Swift

#### Code Docs

- [Updating and Deleting Keychain Items](https://developer.apple.com/documentation/security/keychain_services/keychain_items/updating_and_deleting_keychain_items)

#### Swift Packages for Atom

- [SwiftLint](https://realm.github.io/SwiftLint/) - A tool to enforce Swift style and conventions, loosely based on GitHub’s Swift Style Guide.

    `brew install swiftlint`
    
- [linter-swiftlint](https://atom.io/packages/linter-swiftlint) - This linter plugin for Linter provides an interface to SwiftLint's styling advice. Used with files that have the Swift syntax.

- [language-swift](https://atom.io/packages/language-swift) - Swift language support for Atom.

- [autocomplete-swift](https://atom.io/packages/autocomplete-swift)

    - [SourceKittenDaemon](https://github.com/terhechte/SourceKittenDaemon) - This is a simple daemon that can read Xcode Swift projects and offers auto completion for Swift files and more over a built-in webserver. Effectively, this allows any kind of editor like Vim, Emacs, Sublime, or Atom to support Swift, Auto Completion, and Xcode projects.


<a name="bash"></a>

### Bash

- [Bash Cheat Sheet](https://devhints.io/bash)
- [Cyber Dojo](https://www.cyber-dojo.org)
- [bashoneliners.com](http://www.bashoneliners.com/oneliners/oneliner/popular/)
- Shell Variables - <https://www.gnu.org/software/bash/manual/bash.html#Shell-Variables>
- User input with a while loop - <http://alvinalexander.com/linux-unix/shell-script-how-prompt-read-user-input-bash>
- 8 examples of Bash if statements - <http://bencane.com/2014/01/27/8-examples-of-bash-if-statements-to-get-you-started/>
- [25 Simple Find commands](http://www.binarytides.com/linux-find-command-examples/)
- [The /sbin Directory](http://www.linfo.org/sbin.html)
- [Working with tar](http://www.tecmint.com/18-tar-command-examples-in-linux/)


#### Code Snippets

- Remove training and leading whitespace

	`sed -e 's/^[ \t]*//'`

#### File Testing

| flag | Def |
| :-- | :-- |
| -b filename	| Block special file |
| -c filename	| Special character file |
| -d directory name | Check for directory existence |
-e filename | Check for file existence |
-f filename | Check for regular file existence not a directory |
-G filename | Check if file exists and is owned by effective group ID. |
-g filename | true if file exists and is set-group-id. |
-k filename | Sticky bit |
-L filename | Symbolic link |
-O filename | True if file exists and is owned by the effective user id. |
-r filename | Check if file is a readable |
-S filename | Check if file is socket |
-s filename | Check if file is nonzero size |
-u filename | Check if file set-ser-id bit is set |
-w filename | Check if file is writable |
-x filename | Check if file is executable |


#### String Comprehension

| flag | Def |
| :-- | :-- |
| [ STRING1 == STRING2 ] | STRING1 is equal to STRING2 |
| [ STRING1 = STRING2 ]	| STRING1 is equal to STRING2 |
[ STRING1 != STRING2 ]	| STRING1 is NOT equal to STRING2
[ STRING1 \> STRING2 ]	| STRING1 is lexically greater than STRING2 - b is greater than a
[ STRING1 \< STRING2 ]	| STRING1 is lexically less than STRING2 - a is less than b
[ -n STRING ]	| STRING is non zero - a variable has been set
[ -z STRING ]	| STRING is zero - variable has no value
[[ STRING1 =~ REGEXPRESSION ]] |	STRING1 matches Regular Expression

\[[top](#top)]
<a name="vim"></a>

### Vim Customization

-   [vim wiki](http://vim.wikia.com/wiki)
-   [NerdTree Doc](https://github.com/scrooloose/nerdtree/blob/master/doc/NERDTree.txt)

*Learning*

- [Vim Adventures](https://vim-adventures.com)

<a name="vscode"></a>

### VSCode

- [Docs](https://code.visualstudio.com/docs)

#### Settings

```css
{
    "window.zoomLevel": 0,
    "editor.wordWrap": "bounded",
    "workbench.editor.highlightModifiedTabs": true,
    "editor.minimap.side": "left",
    "workbench.colorTheme": "Dracula",
    "workbench.colorCustomizations": {
        "editor.selectionBackground": "#e9497e77",
        "editor.selectionHighlightBackground": "#e9497e77",
        "editor.lineHighlightBorder": "#e9497e77",
        "editor.lineHighlightBackground": "#e9497e77",
        "editorBracketMatch.border": "#e9497ebd",
        "minimap.selectionHighlight": "#e9497e77",
        "editorCursor.foreground": "#e9497e",
    },
    "editor.fontSize": 9,
    "editor.fontFamily": "Hack, Fira Code, Menlo, Consolas, DejaVu Sans Mono, monospace",
    "editor.multiCursorModifier": "ctrlCmd",
    "python.formatting.provider": "black",
    "python.linting.pydocstyleEnabled": true,
    "[python]": {
        "editor.defaultFormatter": "ms-python.python"
    },
    "atomKeymap.promptV3Features": true,
    "editor.formatOnPaste": true,
    "editor.formatOnSave": true,
    "editor.snippetSuggestions": "bottom",
    "files.trimTrailingWhitespace": true,
    "search.showLineNumbers": true,
    "editor.renderLineHighlight": "all",
    "html.format.wrapLineLength": 79,
    "python.linting.pycodestyleEnabled": true,
    "python.linting.pylintEnabled": false,
    "editor.wordWrapColumn": 88,
    "editor.rulers": [
        88
    ],
    "editor.cursorStyle": "block",
    "editor.cursorSurroundingLinesStyle": "all",
    "editor.minimap.maxColumn": 50,
}
```

<a name="atom"></a>

### Atom IDE Customization ...

```css
// Selection color - added by captam3rica
atom-text-editor::shadow .selection .region {
    background-color: #EA4760;
}

// To style other content in the text editor's shadow DOM, use the ::shadow expression
atom-text-editor::shadow .cursor {
  border-color: #EA4760;
}

// Minimap cursor color style
.minimap .cursor-line {
    background: #EA4760;
}

// add or import these into your Atom styles.less

/******************  VIM MODE STATUS BAR ****************************************/

// green
@normal-bg: rgb(105, 238, 103);
// blue
@insert-bg: rgb(7, 193, 242);
// yellowish
@visual-bg: rgb(255, 206, 98);


// change the current cursor-line background color
// based on vim mode
atom-text-editor.is-focused.editor {
  .cursor-line {
    // background: rgba(64, 64, 37, 5);
    background: fadeout(@normal-bg, 80%);
  }
  &.insert-mode {
    .cursor-line {
      background: fadeout(@insert-bg, 90%);
    }
  }
}


// vim mode in the status bar at the bottom
// make it nice and big so you can see it out of the corner of your eye
// without thinking about it.
.status-bar-vim-mode-normal,
.status-bar-vim-mode-insert,
.status-bar-vim-mode-visual {
  font-weight: bold;
  text-align: center;
  font-size: 1.5em;
  width: 18rem;
  text-transform: uppercase;
}


.status-bar-vim-mode-normal {
  background: @normal-bg;
  color: rgb(4, 111, 11);
}

.status-bar-vim-mode-insert {
  background: @insert-bg;
  color: white;
}

.status-bar-vim-mode-visual {
  background: @visual-bg;
  color: rgb(168, 117, 5);
}

// change cursor color in normal mode
atom-text-editor.vim-mode.normal-mode.is-focused.editor {
  .cursor {
    background-color: @normal-bg;
  }
}

// visual mode and selected text
atom-text-editor.editor .selection .region {
  background-color: fadeout(@visual-bg, 75%);
}
```

<a name="markdown"></a>

### Markdown

-   [CommmonMark](http://commonmark.org/)

    -   [CommmonMark Spec](http://spec.commonmark.org/)

-   [Brett Terpstra: Write Better Markdown](http://brettterpstra.com/2015/08/24/write-better-markdown/)

-   [vim wiki](http://vim.wikia.com/wiki)
-   [vim-markdownfmt](https://github.com/moorereason/vim-markdownfmt)

-   Build a table of contents

    ```markdown
    # Markdown syntax

      # Table of contents
      1. [Introduction](#introduction)
      2. [Some paragraph](#paragraph1)
      3. [Sub paragraph](#subparagraph1)
      4. [Another paragraph](#paragraph2)

      ## This is the introduction <a name="introduction"></a>
      Some introduction text, formatted in heading 2 style

      ## Some paragraph <a name="paragraph1"></a>
      The first paragraph text

      ### Sub paragraph <a name="subparagraph1"></a>
      This is a sub paragraph, formatted in heading 3 style

      <a name="paragraph2"></a>
      ## Another paragraph
      The second paragraph text
    ```

\[[top](#top)]

### RegEx

-   [RegEx - Grymoire](http://www.grymoire.com/Unix/Regular.html "Learn about regex")

\[[top](#top)]

### PowerShell

- [Running Remote Commands](https://docs.microsoft.com/en-us/powershell/scripting/learn/remoting/running-remote-commands?view=powershell-7)

    - `Enter-PSSession <computer_name>`
    - `Exit-PSSession`
    - `$SESSION = New-PSSession -ComputerName <server_01>`
    
        - This session can now be used throughout the PS script. Anything run agains the computers in the `$SESSION` var will show up on the local machine that invoked the PS script.

    - `Invoke-Command -ComputerName <server_01>, <server_n> -ScriptBlock {remote_ps_command}`
    - `Invoke-Command -ComputerName <server_01> -FilePath <path\to\local\script.ps1`

        - The script needs to be accessible to your local machine. The machine that you are evoking the command from.

- [Get-Content](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.management/get-content?view=powershell-7) - Gets the content of the item at the specified location.
- [Memory and Handle Quotas in the WMI Provider Ser](https://blogs.technet.microsoft.com/askperf/2008/09/16/memory-and-handle-quotas-in-the-wmi-provider-service/)
- Bypass Execution Policies - <https://blog.netspi.com/15-ways-to-bypass-the-powershell-execution-policy/>
- [Passing Credentials](https://gallery.technet.microsoft.com/scriptcenter/Execute-PowerShell-Script-38881dce)
- [Get AD Computer Info](https://4sysops.com/archives/get-adcomputer-display-computers-in-ou-or-ad-group-with-powershell/)
	- [MSFT Doc](https://www.akaplan.com/blog/2014/02/get-computers-distinguished-name-in-powershell/)
- [Get Distinguished Computer Name](https://www.akaplan.com/blog/2014/02/get-computers-distinguished-name-in-powershell/)

\[[top](#top)]


### sed

-   [Learn Sed](http://www.grymoire.com/Unix/Sed.html)

## Software

### Web Browser Settings

-   Chrome, Chromium, and Vivaldi Autofill Settings: `chrome://settings/search#autofill`
-   Opera flag settings: `opera://flags/`

    -   Smooth Scrolling: Disabled
    -   Experimental QUIC (Similar to TCP but over UDP): Enabled

[[top](#top)]


## Networking

### Wireshark

#### Commands

- Find partial IP address

    `ip.host matches "\.1\.62$"`  
    `ip.src_host matches "\.1\.62$"`  
    `uo.dst_host matches "\.1\.62$"`  


## Security

-   [Hashing vs Encryption](http://www.darkreading.com/safely-storing-user-passwords-hashing-vs-encrypting/a/d-id/1269374)

### Handy Commands

- Check the SSL/TLS cert using openssl

	`openssl s_client -connect example.com:443`

[[top](#top)]

<a name="windows"></a>
