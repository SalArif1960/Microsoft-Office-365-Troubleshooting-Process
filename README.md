Microsoft Office 365 Troubleshooting Process
Author: Arif Ghuznavi
Environment: Personal Microsoft 365 / Intune Lab
Status: In Progress / Hands-On Verified Sections Included
WHY
Build a repeatable Microsoft 365 troubleshooting process that starts with cloud-side validation before making endpoint changes.
Core flow:
Identity → License → Service Health → Workload → Device / Client → Verify
WHAT
This folder documents hands-on troubleshooting for:
- Microsoft 365 user administration
- Exchange Online
- Microsoft Teams
- SharePoint Online
- OneDrive for Business
- Microsoft 365 Service Health
WHERE
Main portals:
- Microsoft 365 Admin Center
- Exchange Admin Center
- Teams Admin Center
- SharePoint Admin Center
- Windows OneDrive client
HOW
Use this investigation order:
1. Confirm the user exists and can sign in.
2. Confirm the correct Microsoft 365 license and service plan.
3. Check Microsoft 365 Service Health.
4. Open the affected workload.
5. Check user-specific settings, permissions, policies, or mail flow.
6. Move to the local client/device only after cloud-side checks are healthy.
7. Verify the result after any change.
RESULTS
Hands-on work completed so far:
- Active user verification
- Microsoft 365 Business Premium license verification
- Exchange mailbox verification
- Exchange delegation check
- Message Trace showing Received → Processed → Delivered
- Teams user and effective policy review
- Global Teams Meeting Policy review
- Teams Client Health review
- SharePoint Active Sites review
- SharePoint membership and Site Members review
- SharePoint site browser access
- OneDrive cloud settings review
- OneDrive desktop client account verification
TROUBLESHOOTING
Exchange Online
Mailbox → Address → Forwarding → Delegation → Message Trace → Outlook / Web
Microsoft Teams
User → License → Service Health → Effective Policy → Policy Settings → Client Health → Logs
SharePoint Online
Service Health → Site → Membership → Permission → Library / File → Browser / Device
OneDrive
Service Health → Provisioning → Storage → Sharing → Web Access → Sync Client → Device
VERIFICATION
Verified in the lab:
- [x] User account exists
- [x] Business Premium license assigned
- [x] Exchange Online enabled
- [x] Mailbox exists
- [x] No forwarding configured
- [x] No mailbox delegation configured
- [x] Message Trace completed
- [x] Message delivered successfully
- [x] Teams policies reviewed
- [x] Teams meeting policy reviewed
- [x] Teams Client Health checked
- [x] SharePoint site exists
- [x] SharePoint membership verified
- [x] SharePoint site opens in browser
- [x] OneDrive provisioned
- [x] OneDrive desktop client connected
EVIDENCE
Store screenshots in the evidence/ folder.
Suggested naming:
evidence/
├── 01-m365-active-users.png
├── 02-user-account.png
├── 03-license-and-apps.png
├── 04-exchange-mailbox.png
├── 05-exchange-delegation.png
├── 06-message-trace-delivered.png
├── 07-service-health.png
├── 08-teams-effective-policies.png
├── 09-teams-meeting-policy.png
├── 10-teams-client-health.png
├── 11-sharepoint-active-sites.png
├── 12-sharepoint-membership.png
├── 13-sharepoint-site-access.png
├── 14-onedrive-admin-settings.png
└── 15-onedrive-client-account.png
KEY LESSON
Start high in the cloud, isolate the failing layer, change only what is necessary, and always verify the result.

Do not immediately reset passwords, remove licenses, reinstall apps, unlink OneDrive, or change policies without evidence.# Microsoft-Office-365-Troubleshooting-Process
