# Ref list for virtualizaton

## Related to Windows Administration

- [sway.office.com](https://sway.office.com/leB5lmZDQsxnrMAv?ref=Link)
- List of WMIC CSProduct Get Name Results - <http://faqshop.com/misc/list-of-wmic-csproduct-get-name-results/>
- [Troubleshooting Slow Logons via PowerShell](https://www.citrix.com/blogs/2015/08/05/troubleshooting-slow-logons-via-powershell/)
- [Logon GPO Analysis via PowerShell](https://www.controlup.com/blog/logon-gpo-analysis-via-powershell/)
- [Windows 10 Environment Variables](https://www.tenforums.com/tutorials/3234-environment-variables-windows-10-a.html)
- [Install RSAT - Win10 1809](https://www.prajwaldesai.com/install-rsat-tools-on-windows-10-version-1809/)

### Documenation

- [Microsoft Docs](https://docs.microsoft.com/en-us/)

### Tools

- [Windows ISO Downloader](https://heidoc.net/joomla/technology-science/microsoft/67-microsoft-windows-and-office-iso-download-tool)
- [GPO Migration Tool](https://code.vmware.com/samples/3527/airwatch-gpo-migration-tool?h=gpo%20migration%20tool)


### MSFT Office

- AutoUpdator Location

    `/Library/Application\ Support/Microsoft/MAU2.0`

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

#### Errors

- [Exchange Online: Apple Internet Accounts - Need admin approval](https://diecknet.de/en/2020/05/10/Apple-Internet-Accounts-Office365/)


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


<a name="msft_conditional_access"></a>

### Conditional Access

- [MSFT Doc: Enforcing Conditional Access](https://docs.microsoft.com/en-us/mem/intune/protect/conditional-access-assign-jamf)
- Only applies to AAD User groups
- [MSFT Doc: Troubleshooting](https://docs.microsoft.com/en-us/mem/intune/protect/troubleshoot-jamf)
- [MSFT Doc: macOS settings to mark devices as compliant or not compliant using Intune](https://docs.microsoft.com/en-us/mem/intune/protect/compliance-policy-create-mac-os)


### IIS

*Errors*

- [HTTP Error 403.7 - Forbidden](https://support.microsoft.com/en-us/help/942067/http-error-403-7-forbidden-error-when-you-run-a-web-application-that-i)

    This problem occurs because the Require SSL option is selected. This option appears on the SSL Settings page of Internet Information Services (IIS) Manager. When this option is selected, all requests that client computers make to the Web application must use a Secure Sockets Layer (SSL) connection.

    Additionally, the Require option of the "Client certificates" feature is selected. This option also appears on the SSL Settings page of IIS Manager. When this option is selected, all client computers that send requests to the server that is running IIS must have valid client certificates.

- [403.7 Forbidden: Client Certificate Required](https://support.microsoft.com/en-us/help/186812/403-7-forbidden-client-certificate-required-error-when-you-open-an-iis)

    This error occurs when the website requests a client certificate, and then the client either does not provide one or the certificate supplied by the client browser is rejected. Client certificates are a kind of Secure Sockets Layer (SSL) certificate typically used to identify a user or computer to a website.

    - The following are several possible causes of this problem:
    - The root certificate (certification authority certificate) of the client certificate is not installed on the computer that is running IIS.
    - The client certificate has expired, or the effective time has not been reached.
    - The client certificate was revoked.
    - No valid client certificate is available, or a potentially valid client certificate does not have an associated private key installed.

- [HTTP Error 403.16 - Forbidden](https://support.microsoft.com/en-us/help/942061/error-message-when-you-visit-a-web-site-that-is-hosted-on-iis-7-0-http)

    **Cause 1**

    This problem occurs because the root certificate of the certification authority is not in the Trusted Root Certification Authorities certificate store on the IIS Web server.

    Note The root certificate of the certification authority is used to issue the client certificate.

    **Cause 2**

    There are one or more non–self-signed certificates in the Trusted Root Certification Authorities certificate store. A non–self-signed certificate is any certificate for which the "Issued To" and "Issued By" values are not an exact match.

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
