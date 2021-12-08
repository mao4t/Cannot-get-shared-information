Connect-PnPOnline as a service principal and set the values ​​of SharingAllowedDomainList, SharingBlockedDomainList and SharingDomainRestrictionMode.
First of all, I want to get it.
① Connect-PnPOnline -Url "https://xxx-admin.sharepoint.com"
② Connect-PnPOnline -Url "https://xxx.sharepoint.com/sites/SPO-TX010"

Get-PnPTenantSite -Filter "Url -like'* / sites / SPO-TX010'"
I tried to execute the above Get command with two types of connections, but the values ​​related to sharing are the same as when connecting to Get-SPOService.
Could not get it.
* The Get-PnPTenantSite command itself has been successful.
* Three values ​​can be obtained when Connect-PnPOnline is performed without using the service principal.
* The app ID is assigned the Azure AD role SharePint administrator and the app permissions SharePoint Sites.FullControl.All.
How can I get the values ​​of SharingAllowedDomainList, SharingBlockedDomainList and SharingDomainRestrictionMode? 
