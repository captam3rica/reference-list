# Reference List

This is where I put handy links, commands, 3rd party resources, documentation links, etc that I have found helpful in my technology journey

Referenced often, Updated semi-regularly :)

<a name="top"></a>

## TOC

1. [Apple  ](#macintosh)
    1. [Admin Tools](#macos_tools)
    1. [Apple STIG](#apple_stig)
    1. [Apple Device Automation](#apple_device_automation)
    1. [Application Management](#apple_app_management)
        1. [Handy Sites](#macos_sites)
    1. [Content Cache](#apple_content_caching)
    1. [Documentation](#macos_documentation)
        1. [MDM Protocol](#appls_mdm_protocol)
    1. [Encryption & FileVault](#macos_encryption_and_fv)
    1. [Handy Terminal Commands](#macos_commands)
    1. [Networking & Wi-Fi](#macos_network_and_wifi)
    1. [Security](#macos_security)
    1. [Support](#apple_support)

1. [Unix & GNU/Linux](#unix_linux)

1. [MDM](#mdm)

	1. [Apple](#mdm_apple_apns)
	1. [Jamf](#mdm_jamf)
	2. [Addigy](#mdm_addigy)
	2. [WorkspaceONE](#mdm_wso)
	3. [MSFT Device Manager](#mdm_msft_device_manager)
	3. [Mobile Iron](#mdm_mobile_iron)
	4. [Google Enterprise](mdm_google_enterprise)

1. [Identity & Access Management](#idam)

    1. [WorkspaceONE Access](#idam_wso_access)

1. [Certificate Information](#cert_information)

1. [Scripting, Automation, & Development](#scripting_automation_dev)

    1. [Ansible](#ansible)
    1. [Awk](#awk)
    1. [Bash](#bash)
    1. [Code Signing](@scripting_code_signing)
    1. [Git](#git)
    1. [golang](#golang)
    1. [Markdown](#markdown)
    1. [PowerShell](#powershell)
    1. [Python](#python)
    1. [RegEx](#regex)
    1. [sed](#sed)
    1. [Swift](#swift_code)
    1. [Vim](#vim)
    1. [VSCode](#vscode)
    1. [zshell](#zshell)

1. Software

    1. Opera Browser Settings

1. Security

    1. Handy Commands

1. [Other](#other)

    1. [JumpCloud](#jumpcloud)

1. Virtualization - moved to separate doc
1. Windows - moved to separate doc

<a name="macintosh"></a>

## Apple Support & Administration

<a name="macos_tools"></a>

### Admin Tools

- [Apple Configurator 2](https://help.apple.com/configurator/mac/2.0/) - Apple Configurator 2 makes it easy to deploy iPad, iPhone, iPod touch, and Apple TV devices in your school or business.

- [AutoDMG](https://github.com/MagerValp/AutoDMG) - The award winning AutoDMG takes a macOS installer (10.10 or newer) and builds a system image suitable for deployment with Imagr, DeployStudio, LANrev, Jamf Pro, and other asr-based imaging tools.

- [Automator](https://configautomation.com)

- [AutoPkg](https://autopkg.github.io/autopkg/) - AutoPkg is a system for automatically preparing software for distribution to managed clients. Recipes allow you to specify a series of simple actions which combined together can perform complex tasks, similar to Automator workflows or Unix pipes.

    - [GitHub Repo](https://github.com/autopkg/autopkg)
    - [recipe-robot](https://github.com/homebysix/recipe-robot): help create AutoPkg
recipes.

- [BigHonkingText](https://bitbucket.org/twocanoes/bighonkingtext/src/master/) - BigHonkingText is a command line tool to put up large letters on the screen from the command line on macOS.

- [DEPNotify](https://gitlab.com/Mactroll/DEPNotify): Simple tool to display
    what is happening during DEP enrollment on the Mac.

    - [cannonball](http://cannonball.tombridge.com/2017/04/27/getting-started-with-installapplication-depnotify-and-simplemdm/)

- [detectX](https://sqwarq.com/detectx/) - A lightweight, troubleshooting and security app for Macs to help find and remove adware, malware, keyloggers, and other unwanted programs. It doesn’t install any kernel extensions or privileged helper daemons, and it is free to use for everyone (no ads, no subscriptions, and no data collection!).

- [Dock Master](https://github.com/Error-freeIT/Dock-Master) - Dock Master is a tool for generating dock profiles and dock packages.

- [EraseInstall](https://bitbucket.org/prowarehouse-nl/erase-install/src/master/) - EraseInstall.app for macOS is designed to allow users to easily erase the HD on their Mac and install a fresh copy of macOS. The application is a wrapper around the command `startosinstall`.

- [iMazing Profile Editor](https://imazing.com/profile-editor) - iMazing Profile Editor lets you create, edit, and sign Apple configuration profiles. Define settings with ease, ready to be deployed locally or via MDM to fleets of iPhones, iPads, Macs, and other Apple devices.

    - [Manifests](https://github.com/ProfileCreator/ProfileManifests/tree/master/Manifests)

- [InstallApplications](https://github.com/erikng/installapplications): dynamically download packages for use with `InstallApplication`

- [Google Santa](https://github.com/google/santa): Application blacklisting

- [ManagedMac](http://dayglojesus.github.io/managedmac/) - puppet plugin for managing Mac.

- [mac-ibm-enrollment-app](https://github.com/IBM/mac-ibm-enrollment-app) - The Mac@IBM enrollment app makes setting up macOS with Jamf Pro more intuitive for users and easier for IT. The application offers IT admins the ability to gather additional information about their users during setup, allows users to customize their enrollment by selecting apps or bundles of apps to install during setup, and provides users with next steps when enrollment is complete.

- [mas-cli](https://github.com/mas-cli/mas): App Store from the CLI

- [Murus macOS Packet Firewall](https://www.murusfirewall.com/murus/)

	macOS features one of the best network firewalls: PF (Packet Filter). It comes in an "under the hood" fashion, installed and disabled by default.
Murus' purpose is to unleash its potential. With its easy and intuitive icons-based and drag&drop-based interface, visual layers of abstraction and a friendly view of the PF firewall it's a lean and mean tool to protect your Mac and network.
Designed with ease of use in mind, yet full of advanced options and monitoring tools, Murus is perfect for everybody; from the average user to the experienced UNIX guru/system administrator and even for educational purposes.
Configure and start the PF firewall in one click using built-in presets, use Murus graphical ruleset editor design tool or write fully customized rulesets using the advanced rule editor.
Murus Pro includes Vallum, an application-layer firewall. This allows you to take full control of your Mac at both application and network level.

	Click [here](https://murusfirewall.com/comparison/) to see a comparison between application and network firewalls.

- [NoMAD](https://nomad.menu/downloads/ "No More Active Directory"): Active
    Directory broker client. OpenSource alt to Apple's Enterprise Connect
    service

- [precache](https://github.com/krypted/precache) - Pull updates down top the
    Apple macOS Server Caching service.

- [MCXToProfile](https://github.com/timsutton/mcxToProfile) - mcxToProfile is a simple command-line utility to create "Custom Settings" Configuration Profiles without the need for the Profile Manager Device Management service in OS X Server 10.7 and 10.8.

- [Packages](http://s.sudre.free.fr/Software/Packages/about.html): Awesome package creator for macOS

	- [User Guide](http://s.sudre.free.fr/Software/documentation/Packages/en_2017/index.html)

- [PPPC Utility (Jamf)](https://github.com/jamf/PPPC-Utility) - PPPC Utility is a macOS (10.13 and newer) application for creating configuration profiles containing the Privacy Preferences Policy Control payload for macOS. The profiles can be saved locally signed or unsigned. Profiles can also be uploaded directly to a Jamf Pro server.

- ***(NO LONGER DEVELOPED)*** [Profile Creator](https://github.com/ProfileCreator/ProfileCreator) - macOS application to create configuration profiles.

- [Payload-Free-Package-Creator](https://github.com/rtrouton/Payload-Free-Package-Creator): when you want to just dumb a script somewhere.

- [Recipe Robot](https://github.com/homebysix/recipe-robot) - Recipe Robot is the easiest way to create new AutoPkg recipes for simple Mac apps.

- [SplashBuddy](https://github.com/Shufflepuck/SplashBuddy) - SplashBuddy goal is to provide an elegant and secure onboarding process for Mac users using DEP.

- [**Suspicious Package**](http://www.mothersruin.com/software/SuspiciousPackage/get.html): look inside of packages.

- [vfuse](https://github.com/chilcote/vfuse) - Takes a never-booted DMG and converts it to a VMware Fusion VM.

- [xmlAutomator](https://github.com/moofit/xmlAutomator) - Tool set created by MoofIT for manipulating `.plist` and `.mobileconfig` files. I mainly use it to unsign `.mobileconfig` files.

<a name="apple_stig"></a>

### Apple STIG

- [macOS 11](https://public.cyber.mil/stigs/downloads/)

<a name="apple_app_management"></a>

### Application Management

- Adobe CC

	- [VMware github](https://github.com/vmware-samples/euc-samples/tree/master/macOS-Samples/3rd-Party_Software_Guidance/Adobe%20Products)

- [Firefox Preferences](https://github.com/mozilla/policy-templates/blob/a46ede82219f2cf58364c13fb434e30670dcd257/README.md)
- [Symantec Endpoint Protection client Mac compatibility](https://knowledge.broadcom.com/external/article/152316/mac-compatibility-with-the-endpoint-prot.html)
- AppConfig
	- [AppConfig Community](https://www.appconfig.org)
	- [Managed App Configuration for App Developers](https://storage.googleapis.com/appconfig-media/appconfig-content/uploads/2017/01/ManagedAppConfig.pdf)
	- [Jamf AppConfig Generator Utility](https://beta.appconfig.jamfresearch.com/generator)

- [Bundle IDs for native iOS and iPadOS apps in mobile device management](https://support.apple.com/guide/mdm/bundle-ids-for-native-ios-and-ipados-apps-mdm90f60c1ce/web)

- [http://appsearch.co/](http://appsearch.co/)

- [Teamviewer Mass Deployment macOS](https://community.teamviewer.com/English/kb/articles/50739-mass-deployment-on-macos)


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

- Blueprint file location

    `/Users/<username>/Library/Group Containers/K36BKF7T3D.group.com.apple.configurator/Library/Application Support/com.apple.configurator/Blueprints`


<a name="macos_sites"></a>

### Handy Sites

- [http://www.getmacapps.com](http://www.getmacapps.com)
- [macadmins.software](macadmins.software)
- [https://derflounder.wordpress.com](https://derflounder.wordpress.com)
- [iOS Release Versions](https://en.wikipedia.org/wiki/IOS_version_history)


<a name="macos_documentation"></a>

### Documentation

- [Developer Documentation](https://developer.apple.com/documentation)

#### Apple KBs

- [HT208802 - ABM Release Notes](https://support.apple.com/en-us/HT208802)
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

<a name="appls_mdm_protocol"></a>

#### Apple MDM Protocol

- [Mobile Device Management Settings](https://support.apple.com/guide/mdm/welcome/web)
- [Apple MDM Documentation](https://developer.apple.com/library/content/documentation/Miscellaneous/Reference/MobileDeviceManagementProtocolRef/3-MDM_Protocol/MDM_Protocol.html#//apple_ref/doc/uid/TP40017387-CH3-SW2)
- [Configuration Profile Reference](https://developer.apple.com/business/documentation/Configuration-Profile-Reference.pdf)
- [Apple Profile Manager](http://help.apple.com/profilemanager/mac/5.4/#/apd5BD57F16-A2BF-43B9-AB4B-24948FB52C1E)
- [Apple Configurator 2](http://help.apple.com/configurator/mac/2.0/)
- [MacOS Deployment Reference](https://help.apple.com/deployment/macos/#/ior5d40635d0)
- Managing macOS Notifications

    - In the User's `~/Library/Preferences`
    - Plist: `com.apple.ncprefs.plist`
    - Look at previously answered prompts with

        ```
        sqlite3 "$(getconf DARWIN_USER_DIR)/com.apple.notificationcenter/db2/db" "select * from app;"
        ```

    - [Mr Macintosh](https://mrmacintosh.com/how-to-manage-catalinas-new-application-notifications-with-a-profile/)
- [Supervised MDM restrictions for Apple devices](https://support.apple.com/guide/mdm/supervised-restrictions-mdm54960f92a/web)
- [Installing Custom KEXT](https://developer.apple.com/documentation/apple_silicon/installing_a_custom_kernel_extension)


#### Other

- [Apple Document Style Guide](https://help.apple.com/applestyleguide)
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


<a name="macos_encryption_and_fv"></a>

### Encryption & FileVault

- [Manage FileVault with `fdesetup`](https://derflounder.wordpress.com/2015/12/20/managing-el-capitans-filevault-2-with-fdesetup/)
- [Mac FileVault recovery key rotation controls via Disk Encryption Configurations](https://www.jamf.com/jamf-nation/feature-requests/6146/mac-filevault-recovery-key-rotation-controls-via-disk-encryption-configurations)
- [FileVault Institutional Recovery Keys - DerFlounder](https://derflounder.wordpress.com/2014/08/13/filevault-2-institutional-recovery-keys-creation-deployment-and-use/)
- [GitHub: fv2RecoveryKeyCheck](https://github.com/CiscoMacIT/fv2RecoveryKeyCheck)

#### Key Rotation

- [Automatically Rotate FileVault Keys After Viewing and/or Usage](https://www.jamf.com/jamf-nation/feature-requests/8978/automatically-rotate-filevault-keys-after-viewing-and-or-usage)
- [Rotate the FileVault Key](https://developer.apple.com/documentation/devicemanagement/rotate_the_filevault_key)


<a name="macos_commands"></a>

### Handy File System Paths

- Core macOS icons

    `/System/Library/CoreServices/CoreTypes.bundle/Contents/Resources`

- Apple icon

    `/System/Library/Components/CoreAudio.component/Contents/Resources`

### Handy Commands

- `startosinstall` usage as of macOS Big Sur 11.3.2

    ```
    Usage: startosinstall

    Arguments
    --license, prints the user license agreement only.
    --agreetolicense, agree to the license you printed with --license.
    --rebootdelay, how long to delay the reboot at the end of preparing. This delay is in seconds and has a maximum of 300 (5 minutes).
    --pidtosignal, Specify a PID to which to send SIGUSR1 upon completion of the prepare phase. To bypass "rebootdelay" send SIGUSR1 back to startosinstall.
    --installpackage, the path of a package (built with productbuild(1)) to install after the OS installation is complete; this option can be specified multiple times.
    --eraseinstall, (Requires APFS) Erase all volumes and install to a new one. Optionally specify the name of the new volume with --newvolumename.
    --newvolumename, the name of the volume to be created with --eraseinstall.
    --preservecontainer, preserves other volumes in your APFS container when using --eraseinstall.
    --forcequitapps, on restart applications are forcefully quit. This is the default if no users are logged in.
    --usage, prints this message.
    --user, an admin user to authorize installation.
    --passprompt, collect a password for authorization with an interactive prompt.
    --stdinpass, collect a password from stdin without interaction.
    ```

- Launch Terminal session from SetupAssistant

    **Note** - This behavior has changed in Big Sur

    - `CTL + OPTION + CMD + T`
    - At the language screen you are root (Pre Device management screen)
    - At SetupAssitant screens you are _mbsetupuser

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

    `sudo nvram boot-args="-v"`

- Monitor and control the iCloudDoc daemon. Runs as a process called `bird`

    `man brctl`

- Configuration Profile Signatures

    - Unsign
        `security cms -D -i /path/to/profile.mobileconfig | xmllint --format - > /path/to/output.mobileconfig`
    - Sign
        `openssl smime -sign -signer /path/to/signingCertificate.pem -inkey /path/to/privateKey.key -nodetach -outform der -in /path/to/unsigned.mobileconfig -out /path/to/signed.mobileconfig`
        
- Profiles Binary

    - Show all Computer channel profiles

        `sudo profiles show`
    
    - Find the MDM profile UUID

        `profiles -Lv | awk '/attribute: name: MDM/,/attribute: profileUUID:/' | awk '/attribute: profileUUID:/ {print $NF}'`
        
    - Attempt to remove a profile via UUID

        `profiles -R -p 00000000-0000-0000-A000-4A414D460003`
        
    - Attempt to remvoe a profile via Profile Identifier

        `profiles remove -type configuration -identifier <profile_identifier_here>`
        `profiles remove -type configuration -identifier loginwindow.a5c9bf1d-3d17-4477-bf31-af725cfbfb13`


<a name="apple_content_caching"></a>

### Content Cache

- [Manage content caching from the command line on Mac](https://support.apple.com/guide/mac-help/manage-content-caching-command-line-mac-mchla6d4541e/mac)

#### Command Usage

```
AssetCacheTetheratorUt... BSD System Manager's ManualAssetCacheTetheratorUt...

NAME
     AssetCacheTetheratorUtil -- control networking of tethered devices

SYNOPSIS
     AssetCacheTetheratorUtil [-j|--json] enable
     AssetCacheTetheratorUtil [-j|--json] disable
     AssetCacheTetheratorUtil [-j|--json] isEnabled
     AssetCacheTetheratorUtil [-j|--json] status

DESCRIPTION
     iOS and tvOS devices connected to a computer with a USB cable can be "tethered," so that they route their Internet
     requests through the computer.  AssetCacheTetheratorUtil enables a tethered network, disables it, or reports on
     its status.  Tethering requires Content Caching.  AssetCacheTetheratorUtil must be run by root, except for the
     isEnabled and status commands.

OPTIONS
     -j|--json     Print results in machine-parseable JSON format to stdout.

SEE ALSO
     System Preferences > Sharing > Content Caching, AssetCacheLocatorUtil(8), AssetCacheManagerUtil(8)

macOS                            June 17, 2020                           macOS
```

```
AssetCacheManagerUtil(8)  BSD System Manager's Manual AssetCacheManagerUtil(8)

NAME
     AssetCacheManagerUtil -- control the macOS Content Cache

SYNOPSIS
     AssetCacheManagerUtil [-a|--all] [-j|--json] [-l|--linger] command

DESCRIPTION
     AssetCacheManagerUtil controls the macOS Content Cache.  AssetCacheManagerUtil must be run by root except as noted
     below.  The options are:

     -a|--all      Show all events, not just the end result of the specified command.

     -j|--json     Print results in machine-parseable JSON format to stdout.

     -l|--linger   Linger after completing command, to show other events.

     The commands are:

     activate      Activates the content cache.  Content caching is deactivated by default.  After you activate content
                   caching, restart devices on your network to take advantage of content caching immediately.  Devices
                   on your network will discover this content cache over time.  Devices that are restarted will use
                   this content cache immediately.

     deactivate    Deactivates the content cache.

     isActivated   Reports the content cache's activation status.  Does not require root.

     canActivate   Reports whether the content cache is eligible for activation.  Does not require root.

     flushCache    Flushes the content cache.

     flushPersonalCache
                   Flushes all personal (iCloud) content from the content cache.

     flushSharedCache
                   Flushes all shared (non-iCloud) content from the content cache.

     status        Reports the content cache's status.  Does not require root.

     settings      Reports the content cache's settings.  Does not require root.

     reloadSettings
                   Forces the content cache to reload its settings.

     moveCacheTo path
                   Moves the cache to path.  The path must end with /Library/Application Support/Apple/AssetCache/Data.
                   The contents of path are deleted and replaced with the cache.

     absorbCacheFrom path read-only|and-destroy
                   Imports the cache from path.  The path must end with either /Library/Application Sup-
                   port/Apple/AssetCache/Data or /Library/Server/Caching/Data.  If the last argument is read-only the
                   cache at path is not modified, otherwise it is emptied.  This command only starts the absorption,
                   which proceeds and finishes in the background.  Use the log(1) command to view progress, for exam-
                   ple: log show --predicate 'subsystem == "com.apple.AssetCache"' --style compact --last 5m

SEE ALSO
     System Preferences > Sharing > Content Caching, AssetCache(8), AssetCacheLocatorUtil(8),
     AssetCacheTetheratorUtil(8)

macOS                            June 17, 2020                           macOS
```

```
AssetCacheLocatorUtil(8)  BSD System Manager's Manual AssetCacheLocatorUtil(8)

NAME
     AssetCacheLocatorUtil -- Utility for reporting information about macOS Content Caches

SYNOPSIS
     AssetCacheLocatorUtil [-j|--json]

DESCRIPTION
     AssetCacheLocatorUtil reports information related to macOS Content Caches running on the computer or on the local
     network.

     Some of the information that AssetCacheLocatorUtil reports depends on the current network configuration, and on
     the user running it.  It might produce different results for different users, on different client devices, or on
     different networks.  Applications that use content caches might choose ones other than the ones
     AssetCacheLocatorUtil reports due to factors beyond its knowledge, such as iCloud affinity.

     AssetCacheLocatorUtil reports the following information separately for system daemons and for the current user:

     Availability hint
                   The system can temporarily save a hint about whether or not there might be content caches on the
                   computer or on the local network.  AssetCacheLocatorUtil prints that saved hint if it is available.

     Saved content caches
                   The system can temporarily save information about content caches it has previously found on the com-
                   puter or on the local network.  AssetCacheLocatorUtil prints that saved information if it is avail-
                   able.

     Refreshed content caches
                   AssetCacheLocatorUtil forces the system to search for content caches on the computer and on the
                   local network and to refresh the saved information above.  It then prints the results.

     Saved and refreshed public IP address ranges
                   If your network administrator has configured public IP address ranges in DNS, which the system uses
                   when looking up content caches, AssetCacheLocatorUtil prints saved and refreshed information about
                   those ranges.

     Saved and refreshed favored server ranges
                   If your network administrator has configured favored server ranges in DNS, which the system uses
                   when looking up content caches, AssetCacheLocatorUtil prints saved and refreshed information about
                   those ranges.

     AssetCacheLocatorUtil then reports the reachability status of all of the content caches it found.  If the computer
     cannot communicate with a content cache over the local network then it cannot request files from that content
     cache.  However, just because the computer can "ping" a content cache does not imply that that content cache will
     serve requests sent from this computer.

     The --json option prints the results in machine-parseable JSON format to stdout.
```

### Apple Business Manager

- [Service access with Managed Apple IDs in Apple Business Manager](https://support.apple.com/guide/apple-business-manager/service-access-with-managed-apple-ids-apd435283f6b/web)
- [What are Managed Apple IDs in Apple Business Manager?](https://support.apple.com/guide/apple-business-manager/what-are-managed-apple-ids-tes78b477c81/1/web/1)
- [Create Managed Apple IDs in Apple Business Manager](https://support.apple.com/guide/apple-business-manager/create-managed-apple-ids-mdm1c9622977/web)


#### Federation

- [Intro to federated authentication with Apple Business Manager](https://support.apple.com/guide/apple-business-manager/intro-to-federated-authentication-apdb19317543/1/web/1)
- [Configure federated authentication with Microsoft Azure AD for Apple Business Manager](https://support.apple.com/guide/apple-business-manager/configure-federated-authentication-microsoft-apdc9611d0e0/1/web/1#apddc46155ee)
- [Add federated domains in Apple Business Manager](https://support.apple.com/guide/apple-business-manager/add-federated-domains-apdf867462bc/1/web/1)
- [Link to new domains in Apple Business Manager](https://support.apple.com/guide/apple-business-manager/link-to-new-domains-apd48c3280c0/1/web/1)
- [Turn on and test federated authentication in Apple Business Manager](https://support.apple.com/guide/apple-business-manager/turn-on-and-test-federated-authentication-apdb02f73f18/1/web/1)


#### SCIM

- [Review SCIM requirements for Apple Business Manager](https://support.apple.com/guide/apple-business-manager/review-scim-requirements-apdd88331cd6/web)
- [Resolve SCIM user account conflicts in Apple Business Manager](https://support.apple.com/guide/apple-business-manager/resolve-scim-user-account-conflicts-apd313013d12/1/web/1)
- [View SCIM activity in Apple Business Manager](https://support.apple.com/guide/apple-business-manager/view-scim-activity-apd1bfd8dfde/1/web/1)
- [Disconnect the SCIM connection in Apple Business Manager](https://support.apple.com/guide/apple-business-manager/disconnect-the-scim-connection-apd609be3a61/1/web/1)


<a name="macos_network_and_wifi"></a>

### Networking & Wi-Fi

- [HT210060 - Use Apple products on enterprise networks](https://support.apple.com/en-us/HT210060)
- [HT201999 - About macOS, iOS, and iTunes server host connections and iTunes background processes](https://support.apple.com/en-us/HT201999)
- [Connet to a Wireless Network from CLI](http://osxdaily.com/2011/04/12/connect-wireless-network-command-line/)
- [802.1x](https://www.esecurityplanet.com/views/article.php/3899996/How-to-Use-Enterprise-WiFi-Encryption-and-8021X-in-Mac-OS-X.htm)
- [Port Specifications for Apple Services](https://support.apple.com/en-us/HT202944)
- [APNS](https://support.apple.com/en-us/HT203609)


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


<a name="software_updates_apple"></a>

### Software Updates - Apple

#### macOS

- Major OS Versions are announce in the September timeframe and released in the November timeframe.
- Keep your Mac up to date - https://support.apple.com/guide/mac-help/get-macos-updates-mchlpx1065/mac
- How to Upgrade - https://www.apple.com/macos/how-to-upgrade/
- Security Updats - https://support.apple.com/en-us/HT201222
- macOS Big Sur Release datses - https://en.m.wikipedia.org/wiki/MacOS_Big_Sur
- macOS Big Sure IPSW Release Dates - https://ipsw.me/MacBookPro17,1


<a name="apple_support"></a>

### Support

- [ABM Support Numbers](https://help.apple.com/businessmanager/?lang=en-us#/apd098f3d709)
- [Check Apple Services](https://www.apple.com/support/systemstatus/)


### User Enrollment

- [User Enrollment payload list for Apple devices](https://support.apple.com/guide/mdm/user-enrollment-payload-list-mdmd866a7407/1/web/1)
- [User Enrollment MDM queries for Apple devices](https://support.apple.com/guide/mdm/user-enrollment-queries-mdm455753d19/web)
- [User Enrollment MDM restrictions for Apple devices](https://support.apple.com/guide/mdm/user-enrollment-restrictions-mdm222c64f44/1/web/1)
-


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

#### MDM Trigger Files

- Directory: `/var/db/ConfigurationProfiles/Settings`
- Files
    - .cloudConfigHasActivationRecord
    - .cloudConfigRecordFound
    - .migrated

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


#### User Enrollment Type

- [What is Apple's User Enrollment](https://simplemdm.com/apple-user-enrollment/)
- [User Enrollment into MDM](https://support.apple.com/guide/deployment-reference-ios/user-enrollment-apdeb00576b2/web)
- [User Enrollment MDM Payload for Apple devices](https://support.apple.com/guide/mdm/user-enrollment-payloads-mdmd866a7407/web)
- [User Enrollment MDM Commands for Apple deviecs](https://support.apple.com/guide/mdm/user-enrollment-commands-mdm5dcf7ef50/web)
- [User Enrollment MDM restrictions for Apple devices](https://support.apple.com/guide/mdm/user-enrollment-restrictions-mdm222c64f44/web)
- [User Enrollment MDM queris for Apple devices](https://support.apple.com/guide/mdm/user-enrollment-queries-mdm455753d19/web)

<a name="mdm_jamf"></a>

### Jamf

*API Documentation*

- [API Support](http://developer.jamf.com/apis/jamf-pro-api/index)
- [Classic API](https://developer.jamf.com/apis/classic-api/index)
- [New Swagger API - https://[your_url].jamfcloud.com/uapi/doc](https://[your_url].jamfcloud.com/uapi/doc/#)
- What can be manipulated
	- Enbale/disable Bluetooth

*Certificate Services Integration*

- [Jamf ADCS Connector](https://docs.jamf.com/ad-cs-connector/1.0.0/Jamf_AD_CS_Connector_Overview.html)
- [DCOM Port Information](https://support.microsoft.com/en-us/help/832017/service-overview-and-network-port-requirements-for-windows)

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

*Conditional Access*

- [Conditional Access and Why it Matters](https://www.jamf.com/products/jamf-pro/microsoft/)
- [Intune Integration - Traveling Tech Guy](https://travellingtechguy.eu/jamf-pro-and-ms-azure-intune-for-macos/)
- [Jamf Doc: Integrating with Microsoft Intune to Enforce Compliance on Mac Computers Managed by Jamf Pro](https://docs.jamf.com/technical-papers/jamf-pro/microsoft-intune/10.17.0/Introduction.html)
- [Jamf Doc: Conditional Access with Azure](https://resources.jamf.com/documents/white-papers/conditional-access-going-beyond-perimeter-based-security.pdf)
- Only applies to AAD User groups
- MSFT KB: [Integration Jamf Pro with Intune for conditional access](https://docs.microsoft.com/en-us/mem/intune/protect/conditional-access-integrate-jamf)
- MSFT KB: [Enforce Compliance on macOS](https://docs.microsoft.com/en-us/mem/intune/protect/conditional-access-assign-jamf)
- MSFT KB: [What is Conditional Access](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview)


*Education*

- [Jamf 200 Course Materials](https://docs.jamf.com/education-services/resources/20190920/200_Resources.html)
- [Jamf 300 Course Materials](https://docs.jamf.com/education-services/resources/20190920/300_Resources.html)
- [Jamf 400 Course Materials](https://docs.jamf.com/education-services/resources/20190920/400_Resources.html)

*Errors*

-

*Extension Attributes*

- [Jamf GitHub Extension Attributes Repo](https://github.com/jamf/Jamf-Nation-Extension-Attributes)

*LDAP Integration*

- [JIM Install Guide](http://docs.jamf.com/infrastructure-manager/1.3.2/Installing_a_Jamf_Infrastructure_Manager_Instance.html)
    - [JIM Multi-site](https://github.com/jamf/Multi-JIM/blob/master/Multi-Instance%20JIM-Install.sh)
- [AzureAD LDAPS](https://www.jamf.com/jamf-nation/discussions/25876/a-guide-to-jss-azure-ad-integration-ldap-+-sso)    
    - [MSFT Doc: LDAPS Integration](https://docs.microsoft.com/en-us/azure/active-directory-domain-services/tutorial-configure-ldaps)
    - [MSFT Doc: Create and Configure an AD DS Instance](https://docs.microsoft.com/en-us/azure/active-directory-domain-services/tutorial-create-instance)
    - [HCS: Integrating Jamf with Azure AD LDAPS](https://hcsonline.com/support/white-papers/a-guide-to-identity-management-with-azure-active-directory-jamf-pro)
- [Okta LDAP Integration](https://travellingtechguy.eu/integrating-okta-ldap-in-jamf-pro/)

*Maintenance URLs*

- [Service Status](https://status.jamf.com)
- [Jamf Pro Known Issues](https://www.jamf.com/jamf-nation/my/products/jamf-pro/known-issues)

*Misc Documentation*

- [All Product Documentation](https://www.jamf.com/resources/product-documentation/)
- [Jamf Pro Security Overview](https://www.jamf.com/resources/product-documentation/jamf-pro-security-overview/)
- [MacOS Security Checklist](https://resources.jamf.com/documents/products/documentation/macos-security-checklist.pdf)
- [Startinstall Repo](https://github.com/jamf/erase-install-webinar/wiki)
- [Computer Payload Variables](https://docs.jamf.com/10.21.0/jamf-pro/administrator-guide/Computer_Configuration_Profiles.html)

*Network Information*

- [Ports Used](https://www.jamf.com/jamf-nation/articles/34/network-ports-used-by-jamf-pro)
- [JamfCloud IP Addresses](https://www.jamf.com/jamf-nation/articles/409/permitting-inbound-outbound-traffic-with-jamf-cloud)

*Remote Control*

- [Initiate Casper Remote session from the record in web interface](https://www.jamf.com/jamf-nation/feature-requests/3236/initiate-casper-remote-session-from-the-record-in-web-interface)
- [derflaunder: Using directory membership to manage Apple Remote Desktop permissions](https://derflounder.wordpress.com/2018/08/22/using-directory-membership-to-manage-apple-remote-desktop-permissions/)
- [Enable remote management (full control)](https://www.jamf.com/jamf-nation/discussions/29233/enable-remote-management-full-control-in-mojave#responseChild184447)
- [How to Enable Screen Sharing & Remote Login](https://www.jamf.com/jamf-nation/discussions/31975/how-to-enable-screen-sharing-remote-login)
- [Jamf Admin Guide: Screen Sharing](https://docs.jamf.com/10.25.0/jamf-pro/administrator-guide/Screen_Sharing.html)

*Reporting and Dashboards*

- ![Jamf Namtion: Show off your reporting dashboard](https://www.jamf.com/jamf-nation/discussions/35614/show-off-your-reporting-dashboard)
- Power PI
- Splunk

*SCEP Proxy Configuration*

- Port 443 or 80
- [Enabling SCEP in Jamf Pro](https://docs.jamf.com/technical-papers/jamf-pro/scep-proxy/10.0.0/Enabling_Jamf_Pro_as_SCEP_Proxy_for_Configuration_Profiles.html)
- [Jamf Pro SCEP Communication](https://www.jamf.com/jamf-nation/articles/488/communication-of-jamf-pro-as-scep-proxy)
- [Obtaining a SCEP Proxy Signing Certificate from a Microsoft CA Using Terminal and Uploading the Certificate to Jamf Pro](https://www.jamf.com/jamf-nation/articles/538/obtaining-a-scep-proxy-signing-certificate-from-a-microsoft-ca-using-terminal-and-uploading-the-certificate-to-jamf-pro) - using an external SCEP cert during device enrollment.
- [Video on Setting up Jamf as a SCEP Proxy](https://www.youtube.com/watch?v=jn0HTWKubFY)
- [SCEP - Microsoft CA Integration](https://www.ibm.com/support/knowledgecenter/en/SS8H2S/com.ibm.mc.doc/ce_source/concepts/ce_ca_ms_ca_int.htm)


*Security*

- [Administering FileVault on macOS 10.14 or Later with Jamf Pro](https://www.jamf.com/resources/technical-papers/administering-filevault-on-macos-10-14-or-later-with-jamf-pro/) - This guide provides step-by-step instructions for administering FileVault on macOS 10.14 or later with Jamf Pro.

*Single-Sign-On*

- [Single Sign-On](http://docs.jamf.com/10.10.0/jamf-pro/administrator-guide/Single_Sign-On.html)
	- [Okta](https://www.jamf.com/jamf-nation/articles/435/configuring-single-sign-on-with-okta)
	- [ADFS](https://www.jamf.com/jamf-nation/articles/436/)
	- [Shibboleth](https://www.jamf.com/jamf-nation/articles/437/)
	- [OneLogin](https://www.jamf.com/jamf-nation/articles/438/)
	- [Ping Identity](https://www.jamf.com/jamf-nation/articles/439/)
	- [G-Suite](https://www.jamf.com/jamf-nation/articles/440/)
- [MSFT Azure AD SSO Doc](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/jamfprosamlconnector-tutorial)

*Logging*

- [Integrating Splunk with Jamf Pro and Jamf Protect](https://www.jamf.com/resources/technical-papers/integrating-splunk-with-jamf-pro-and-jamf-protect/)
    - [Jamf Marketplace Splunk Integration](https://marketplace.jamf.com/details/jamf-splunk-integration/)
	- [Jamf Pro Add-on for Splunk](https://splunkbase.splunk.com/app/4729/)
	- [Splunk Test/Dev Environment](https://www.splunk.com/en_us/resources/personalized-dev-test-licenses.html)
- [Logstash](https://www.elastic.co/logstash)

    - Not sure if this solution can integrate with jamf pro but worth looking into.
    - [Quick Start Guide](https://www.tutorialspoint.com/logstash/logstash_quick_guide.htm)
    - [Udemy: Data Processing with Logstash](https://www.udemy.com/course/processing-events-with-logstash/)

#### Packaging

- [Re-packaging Installer Packages](https://derflounder.wordpress.com/2013/11/03/re-packaging-installer-packages-with-packages/)
- [Package Management](https://docs.jamf.com/10.9.0/jamf-pro/administrator-guide/Managing_Packages.html)


#### Tools

- Jamf Protect

    - [YouTube: Introduction to Protect](https://www.youtube.com/watch?v=gsbfkCSjwxc&t=1s)
    - [Product Page](https://www.jamf.com/products/jamf-protect/)
    - [Admin Guide](https://docs.jamf.com/jamf-protect/administrator-guide/Preface.html)
    - [Evaluation Guide]( https://docs.jamf.com/jamf-protect/evaluation-guide/Overview.html)

- [GitHub](https://github.com/jamf)

	- [DEPNotify-Starter](https://github.com/jamf/DEPNotify-Starter)

- Jamf Connect

    - [Admin Guide](https://www.jamf.com/resources/product-documentation/jamf-connect-administrators-guide/)
    - [Using FileVault with Jamf Connect Login](https://www.jamf.com/jamf-nation/articles/682/using-filevault-with-jamf-connect)
    - [Enabling FileVault with Jamf Connect Login on macOS 10.15 or Later](https://www.jamf.com/jamf-nation/articles/708/enabling-filevault-with-jamf-connect-login-on-macos-10-15-or-later)
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


#### Security

- [Privacy](https://www.jamf.com/trust-center/privacy/)
- [Information Security](https://www.jamf.com/trust-center/information-security/)
- [Compliance](https://www.jamf.com/trust-center/compliance/)
- [Jamf Pro Security Overview](https://resources.jamf.com/documents/products/documentation/Jamf-Pro-Security-Overview.pdf)
- [Permitted Inbound and Outbound Traffic with with Jamf Pro Cloud](https://www.jamf.com/jamf-nation/articles/409/permitting-inbound-outbound-traffic-with-jamf-cloud)
- [Network Ports Used by Jamf Pro](https://www.jamf.com/jamf-nation/articles/34/network-ports-used-by-jamf-pro)
- [Jamf Pro Security Overview](https://resources.jamf.com/documents/products/documentation/Jamf-Pro-Security-Overview.pdf)
- [Jamf ISO Certificate Award](https://resources.jamf.com/documents/products/documentation/jamf-iso-certificate-award.pdf)

#### Troubleshooting

- Verify that the port is open with the following powershell command.

	`Test-NetConnection <fqdn_server_hostname> -Port 80 -InformationLevel "Detailed"`

	- https://docs.microsoft.com/en-us/powershell/module/nettcpip/test-netconnection?view=win10-ps

- If you see the following error this may be because an Anchor certificate exists in the Pre Stage Enrollment profile after replacing a self-signed cert with a legitimate 3rd Party CA cert in Tomcat. Removing the profile should resolve the issue.

    ![](images/jamf/server_cert_chain_error.png)


<a name="mdm_addigy"></a>

### Addigy

- [Docs](support.addigy.com)


<a name="mdm_wso"></a>

### Workspace ONE

- [macOS - Custom Attributes](https://docs.vmware.com/en/VMware-Workspace-ONE-UEM/services/ProdProv_All/GUID-BFEAAE97-D112-4B19-8DAB-E0C681F57DDF.html)
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
- [WorkspaceONE Mobileconfig Importer](https://flings.vmware.com/workspace-one-mobileconfig-importer)


<a name="mdm_msft_device_manager"></a>
### MSFT Endpoint Manager (Intune)

- [Endpoint Manager Admin Console](https://endpoint.microsoft.com)
- [Create a User Enrollment Profile: iOS/iPadOS](https://docs.microsoft.com/en-us/mem/intune/enrollment/ios-user-enrollment)
- [REST API](https://docs.microsoft.com/en-us/rest/api/azure/)


#### Application Management

- [Add Apps](https://docs.microsoft.com/en-us/mem/intune/apps/apps-add)
    - [iOS Store](https://docs.microsoft.com/en-us/mem/intune/apps/store-apps-ios)
    - [VPP](https://docs.microsoft.com/en-us/mem/intune/apps/vpp-apps-ios)

        - [Uploading a VPP Token](https://docs.microsoft.com/en-us/mem/intune/apps/vpp-apps-ios#upload-an-apple-vpp-or-apple-business-manager-location-token)
        - [Assigning VPP Apps](https://docs.microsoft.com/en-us/mem/intune/apps/vpp-apps-ios#assign-a-volume-purchased-app)
        - [Removing a VPP App Assignment](https://docs.microsoft.com/en-us/mem/intune/apps/vpp-apps-ios#revoking-app-licenses)

- [macOS Line of Business Apps](https://docs.microsoft.com/en-us/mem/intune/apps/lob-apps-macos)

    - [intune-app-wrapping-tool-mac](https://github.com/msintuneappsdk/intune-app-wrapping-tool-mac)

#### Configuration Profile Management

*iOS*

- [Custom Configuration Profiles](https://docs.microsoft.com/en-us/mem/intune/configuration/custom-settings-ios)

*macOS*

- [Custom Configuration Profiles](https://docs.microsoft.com/en-us/mem/intune/configuration/custom-settings-macos)


#### Endpoint Protection

 - [macOS endpoint protection settings in Intune](https://docs.microsoft.com/en-us/mem/intune/protect/endpoint-protection-macos?toc=/intune/configuration/toc.json&bc=/intune/configuration/breadcrumb/toc.json)


#### Enrollment

*iOS*

- [Enroll iOS/iPadOS devices in to Intune](https://docs.microsoft.com/en-us/mem/intune/enrollment/ios-enroll)
- [APNS](https://docs.microsoft.com/en-us/mem/intune/enrollment/apple-mdm-push-certificate-get)
- [Apple Business Manager](https://docs.microsoft.com/en-us/mem/intune/enrollment/tutorial-use-device-enrollment-program-enroll-ios)
    - Name Template: `{{DEVICETYPE}}-{{SERIAL}}`
- [Device Categories](https://docs.microsoft.com/en-us/mem/intune/enrollment/device-group-mapping)
- [Troubleshooting iOS/iPadOS device enrollment problems in Intune](https://docs.microsoft.com/en-us/mem/intune/enrollment/troubleshoot-ios-enrollment-errors)

*macOS*

- [macOS Enrollment](https://docs.microsoft.com/en-us/mem/intune/enrollment/macos-enroll)
- [macOS Enrollment with the Company Portal](https://docs.microsoft.com/en-us/mem/intune/user-help/enroll-your-device-in-intune-macos-cp)
- [OneNote API](https://docs.microsoft.com/en-us/graph/integrate-with-onenote)

#### GRAPH API

- [GRAPH API Overview](https://docs.microsoft.com/en-us/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [Use the Microsoft Graph API](https://docs.microsoft.com/en-us/graph/use-the-api)

#### Fundamentals

- [Group Add](https://docs.microsoft.com/en-us/mem/intune/fundamentals/groups-add)
    - [Dynamic Membership Rules](https://docs.microsoft.com/en-us/azure/active-directory/enterprise-users/groups-dynamic-membership)


#### MISC

- [User Group Assignment vs Device Group Assginment](https://www.vansurksum.com/2019/11/22/intune-choosing-whether-to-assign-to-user-or-device-groups/)


#### RBAC

- Scope Tags

    - [Demystifying Scope Tags](https://timmyit.com/2019/07/22/demystifying-scope-tags-in-intune-part-1/)

<a name="mdm_mobile_iron"></a>
### Mobile Iron


<a name="mdm_google_enterprise"></a>

### Google Enterprise


#### Handy Links

- [Google Cloud Docs](https://cloud.google.com/docs)
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
<a name="scripting_automation_dev"></a>

## Scripting, Automation, & Development

- [HTTPS Status Code Explanations](https://httpstatuses.com/)
- [shields.io](https://shields.io)
- [Carbon - Beautiful Code Snippets](https://carbon.now.sh/T1BQoqf2hzlMLWEWAEfG)
- [Unicode Character DB](http://www.unicode.org/reports/tr44/#GC_Values_Table)
- [Dev Cheatsheets](https://devhints.io/)

<a name="ansible"></a>

### Ansible

- [Manage macOS user defaults](https://docs.ansible.com/ansible/latest/modules/osx_defaults_module.html)
- [Python 3 Support](https://docs.ansible.com/ansible/latest/reference_appendices/python_3_support.html)

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

	![](images/git/macos-git-error.png)

3. After the update is completed, open a new terminal window and your development tools should be returned.


	**Addition**: With any major or semi-major update you'll need to update the command line tools in order to get them functioning properly again. Check Xcode with any update. This goes beyond Mojave...

4. After that restart your terminal


<a name="golang"></a>

### <img src="images/go-lang/go_gopher.png" alt="golang gopher" width="64"/> Go

#### Resources

- [Effective Go](https://golang.org/doc/effective_go.html)
- [Go by Example](https://gobyexample.com) - Go by Example is a hands-on introduction to Go using annotated example programs. Check out the first example or browse the full list below.
- [godoc.org](godoc.org) - standard library and 3rd party packages
- [golang.org](golang.org) - language and standard library
- [golang language specification](https://golang.org/ref/spec)
- [github - Todd McLeod - example code](https://github.com/GoesToEleven/go-programming)


#### Packages

- [mackit](https://github.com/groob/mackit)


<a name="python"></a>

### ![](images/Python/python-icon.png) Python

-	Install `pip` python package manager MacOS - **P**ip **I**nstalls **P**ackages
	- `sudo easy_install pip`
-   For **pycodestyle** - PEP8 linter for _Atom_
    - `pip (or pip2) install pycodestyle && apm install pycodestyle`
- [Python for InfoSec](http://strategicsec.com/python-for-infosec-pros-2015/)
- [Python Naming Conventions](http://visualgit.readthedocs.io/en/latest/pages/naming_convention.html)
- [Built-in Exceptions](https://docs.python.org/3/library/exceptions.html#os-exceptions)
- [Requests Module](http://docs.python-requests.org/en/master/user/quickstart/#more-complicated-post-requests) - API Manipulation - `sudo pip install requests`

    - [Requests: Status Codes](https://github.com/psf/requests/blob/master/requests/status_codes.py)

        ```python
        # Informational.
        100: ('continue',),
        101: ('switching_protocols',),
        102: ('processing',),
        103: ('checkpoint',),
        122: ('uri_too_long', 'request_uri_too_long'),
        200: ('ok', 'okay', 'all_ok', 'all_okay', 'all_good', '\\o/', '✓'),
        201: ('created',),
        202: ('accepted',),
        203: ('non_authoritative_info', 'non_authoritative_information'),
        204: ('no_content',),
        205: ('reset_content', 'reset'),
        206: ('partial_content', 'partial'),
        207: ('multi_status', 'multiple_status', 'multi_stati', 'multiple_stati'),
        208: ('already_reported',),
        226: ('im_used',),
    
        # Redirection.
        300: ('multiple_choices',),
        301: ('moved_permanently', 'moved', '\\o-'),
        302: ('found',),
        303: ('see_other', 'other'),
        304: ('not_modified',),
        305: ('use_proxy',),
        306: ('switch_proxy',),
        307: ('temporary_redirect', 'temporary_moved', 'temporary'),
        308: ('permanent_redirect',
              'resume_incomplete', 'resume',),  # These 2 to be removed in 3.0
    
        # Client Error.
        400: ('bad_request', 'bad'),
        401: ('unauthorized',),
        402: ('payment_required', 'payment'),
        403: ('forbidden',),
        404: ('not_found', '-o-'),
        405: ('method_not_allowed', 'not_allowed'),
        406: ('not_acceptable',),
        407: ('proxy_authentication_required', 'proxy_auth', 'proxy_authentication'),
        408: ('request_timeout', 'timeout'),
        409: ('conflict',),
        410: ('gone',),
        411: ('length_required',),
        412: ('precondition_failed', 'precondition'),
        413: ('request_entity_too_large',),
        414: ('request_uri_too_large',),
        415: ('unsupported_media_type', 'unsupported_media', 'media_type'),
        416: ('requested_range_not_satisfiable', 'requested_range', 'range_not_satisfiable'),
        417: ('expectation_failed',),
        418: ('im_a_teapot', 'teapot', 'i_am_a_teapot'),
        421: ('misdirected_request',),
        422: ('unprocessable_entity', 'unprocessable'),
        423: ('locked',),
        424: ('failed_dependency', 'dependency'),
        425: ('unordered_collection', 'unordered'),
        426: ('upgrade_required', 'upgrade'),
        428: ('precondition_required', 'precondition'),
        429: ('too_many_requests', 'too_many'),
        431: ('header_fields_too_large', 'fields_too_large'),
        444: ('no_response', 'none'),
        449: ('retry_with', 'retry'),
        450: ('blocked_by_windows_parental_controls', 'parental_controls'),
        451: ('unavailable_for_legal_reasons', 'legal_reasons'),
        499: ('client_closed_request',),
    
        # Server Error.
        500: ('internal_server_error', 'server_error', '/o\\', '✗'),
        501: ('not_implemented',),
        502: ('bad_gateway',),
        503: ('service_unavailable', 'unavailable'),
        504: ('gateway_timeout',),
        505: ('http_version_not_supported', 'http_version'),
        506: ('variant_also_negotiates',),
        507: ('insufficient_storage',),
        509: ('bandwidth_limit_exceeded', 'bandwidth'),
        510: ('not_extended',),
        511: ('network_authentication_required', 'network_auth', 'network_authentication'),
        ```
    
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
- [How to build a python gui app with wxpython](https://realpython.com/python-gui-with-wxpython/)
- [Advanced import techniques](https://realpython.com/python-import/)

*Modules*

- [pyobjc-framework-SystemConfiguration 5.2](https://pypi.org/project/pyobjc-framework-SystemConfiguration/)
- [site](https://docs.python.org/3/library/site.html)
- sys
    - sys.path

	Wrappers for framework ‘SystemConfiguration’.
These wrappers don’t include documentation, please check Apple’s documention for information on how to use this framework and PyObjC’s documentation for general tips and tricks regarding the translation between Python and (Objective-)C frameworks

	[Docs](https://pyobjc.readthedocs.io/en/latest/)

<a name="swift_code"></a>

### ![](images/Swift/swift_icon.png) Swift

#### Code Docs

- [Updating and Deleting Keychain Items](https://developer.apple.com/documentation/security/keychain_services/keychain_items/updating_and_deleting_keychain_items)

<a name="bash"></a>

### Shell

- [Parse JSON Using JQ](https://stedolan.github.io/jq)
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

```json
{
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[python]": {
    "editor.defaultFormatter": "ms-python.black-formatter",
    "editor.formatOnSave": true
  },
  "[shellscript]": {
    "editor.defaultFormatter": "foxundermoon.shell-format"
  },
  "atomKeymap.promptV3Features": true,
  "autoDocstring.startOnNewLine": true,
  "black-formatter.showNotifications": "always",
  "css.format.spaceAroundSelectorSeparator": true,
  "editor.accessibilitySupport": "off",
  "editor.comments.ignoreEmptyLines": false,
  "editor.fontFamily": "Fira Code, monospace",
  "editor.fontSize": 11,
  "editor.formatOnPaste": false,
  "editor.formatOnSave": true,
  "editor.minimap.enabled": true,
  "editor.minimap.maxColumn": 75,
  "editor.minimap.renderCharacters": false,
  "editor.minimap.showSlider": "always",
  "editor.minimap.side": "left",
  "editor.multiCursorModifier": "ctrlCmd",
  "editor.renderLineHighlight": "all",
  "editor.rulers": [88],
  "editor.suggest.insertMode": "replace",
  "editor.wordBasedSuggestionsMode": "allDocuments",
  "editor.wordWrap": "wordWrapColumn",
  "editor.wordWrapColumn": 96,
  "explorer.confirmDelete": false,
  "flake8.args": [
    "--ignore",
    "--max-line-length",
    "88",
    "E501,E402,F841,F401,E302,E305,E266,E133,W503"
  ],
  "flake8.showNotifications": "always",
  "python.analysis.diagnosticSeverityOverrides": {},
  "python.analysis.extraPaths": [],
  "python.autoComplete.extraPaths": [],
  "python.defaultInterpreterPath": "/Users/captam3rica/.pyenv/shims/python",
  "python.formatting.provider": "black",
  "python.linting.flake8Enabled": true,
  "python.linting.flake8Path": "/Users/captam3rica/.pyenv/shims/flake8",
  "python.linting.pylintEnabled": true,
  "scm.diffDecorationsGutterPattern": {
    "modified": false
  },
  "scm.diffDecorationsGutterWidth": 4,
  "security.workspace.trust.untrustedFiles": "open",
  "shellcheck.customArgs": ["--shell=bash"],
  "shellcheck.ignorePatterns": {
    "**/*.zsh": false
  },
  "syntax.highlightLanguages": [
    "markdown",
    "bash",
    "zshell",
    "c",
    "cpp",
    "python",
    "typescript",
    "typescriptreact",
    "javascript",
    "go",
    "rust",
    "php",
    "ruby",
    "shellscript",
    "ocaml",
    "lua"
  ],
  "workbench.activityBar.visible": false,
  "workbench.colorCustomizations": {
    "[Dracula Pro]": {
      "editor.findMatchBackground": "#E22E4E",
      "editor.findMatchBorder": "#ffff00",
      "editor.findMatchHighlightBackground": "#b38ee6",
      "editor.findMatchHighlightBorder": "#b38ee6",
      "editor.lineHighlightBackground": "#181818",
      "editor.lineHighlightBorder": "#181818",
      "editor.selectionBackground": "#980077",
      "editor.selectionForeground": "#E22E4E",
      "editor.selectionHighlightBackground": "#980077",
      "editor.selectionHighlightBorder": "#000000",
      "editor.wordHighlightBackground": "#980077",
      "editor.wordHighlightStrongBackground": "#980077",
      "editorGutter.deletedBackground": "#E22E4E",
      "editorGutter.modifiedBackground": "#96734c",
      "gitDecoration.deletedResourceForeground": "#E22E4E",
      "gitDecoration.modifiedResourceForeground": "#b38ee6",
      "gitDecoration.stageModifiedResourceForeground": "#b38ee6",
      "gitDecoration.untrackedResourceForeground": "#5be174",
      "minimap.selectionHighlight": "#980077",
      "minimapGutter.modifiedBackground": "#96734c",
      "panel.border": "#1A1921",
      "settings.modifiedItemIndicator": "#b38ee6",
      "sideBar.background": "#1A1921",
      "sideBar.foreground": "#656989",
      "sideBarSectionHeader.background": "#1A1921",
      "tab.activeBorder": "#1A1921",
      "tab.activeBorderTop": "#5be174",
      "tab.unfocusedActiveBorderTop": "#1A1921"
    }
  },
  "terminal.integrated.env.osx": {
    "FIG_NEW_SESSION": "1"
  },
  "files.autoSave": "onWindowChange",
  "black-formatter.importStrategy": "fromEnvironment",
  "workbench.iconTheme": "atom-icons",
  "workbench.colorTheme": "Dracula Pro",
  "workbench.preferredHighContrastColorTheme": "Dracula Pro",
  "workbench.preferredHighContrastLightColorTheme": "Dracula Pro",
  "workbench.preferredDarkColorTheme": "Dracula Pro",
  "shellcheck.executablePath": "/Users/captam3rica/.pyenv/shims/shellcheck"
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

- [regex101](https://regex101.com)
- [RegEx - Grymoire](http://www.grymoire.com/Unix/Regular.html "Learn about regex")

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

### ZShell

- Validating command-ling args

    ```sh
    # Validate Args
    # Don't forget that zsh array index start at 1 and not zero
    for (( i = 1; i <= ${#ARG_ARRAY[@]}; i++ )); do

        # Validate if no agrs given, -h, or --help are passed.
        if [[ "${#ARG_ARRAY}" == 0 ]] || [[ "${ARG_ARRAY}" == "-h" ]] || \
            [[ "${ARG_ARRAY}" == "--help" ]]; then
            # Print this tool's help message
            help_message
        fi

        if [[ "${ARG_ARRAY[$i]}" == "--app-name" ]]; then
            APP_NAME="${ARG_ARRAY[$i+1]}"
            # Make sure that an app name was passed.
            if [[ "$APP_NAME" == "" ]]; then printf "Error: Please enter app name!\n"; usage; exit 1; fi
        fi

        if [[ "${ARG_ARRAY[$i]}" == "--app-version" ]]; then
            APP_VERSION="$(/bin/echo ${ARG_ARRAY[$i+1]} | /usr/bin/sed 's/-/./g')"
            if [[ "$APP_VERSION" == "" ]]; then printf "Error: Please enter app version!\n"; usage; exit 1; fi
        fi

        if [[ "${ARG_ARRAY[$i]}" == "--pkg-name" ]]; then
            PKG_NAME="${ARG_ARRAY[$i+1]}"
            if [[ "$PKG_NAME" == "" ]]; then printf "Error: Please enter package name!\n"; usage; exit 1; fi
        fi

        if [[ "${ARG_ARRAY[$i]}" == "--version" ]]; then; echo "$VERSION"; fi

    done
    ```
    
- Cast to Array - `ARRAY_VAR=($(some command to do a thing where output is added as an array))`

### API Documentation

- [Swagger Documenation](https://swagger.io/docs/specification/2-0/what-is-swagger/)
- [Swagger: Bearer Token](https://swagger.io/docs/specification/authentication/bearer-authentication/)


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

<a name="other"></a>

## Other

<a name="jumpcloud"></a>

### JumpCloud

- [JumpCloud User Attributes](https://support.jumpcloud.com/support/s/article/user-attributes-2019-08-21-10-36-47)
- [Travelingtechguy: JumpCloud LDAP and Jamf](https://travellingtechguy.eu/jumpcloud-as-ldap-provider-in-jamfcloud-jamfpro/)
- [Weldon Dodd: JumpCloud SSO & Jamf](https://medium.com/@weldon/using-jumpcloud-sso-with-jamf-pro-e5fd7006bdf1)
resetpass
