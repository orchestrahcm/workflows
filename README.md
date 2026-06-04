## Workflow List
- [Annual Leave Request](#annual-leave-request-only-via-manager-approval) - A single-step process where annual leave requests are submitted for manager approval.
- [Absence Request](#absence-request-only-via-manager-approval) - A single-step manager approval process for different types of absence requests.

# Workflows
Scheme Based Business Workflows with UI Designs for Web and Mobile
# 
## Annual Leave Request (only via Manager Approval)
![Annual Leave Request](OrcHCM_AnnualLeaveRequestWorkflow.png)
### Business Requirement
Company need to have a digital solution to enable workforce to request annual leave from their managers. 
### Solution Scenerio
Employee requests annual leave from his/her manager online. Manager approves or rejects from taskbox. Manager assignment is read from infotype 0500. This is one step workflow process.
### Download Files and Upload to OrchestraHCM
Download [Scheme](/WF_LREQUEST.json) and  [Screen](/orc.ess.tm.leavereq.json), and make your changes according to your business requirements.
### Notes
- Please customize absence types in your time management module, annual leave absence type in scheme is 1000, if different please modify in INFTY function.
### Versions
- June 4, 2026 - Initial Commit
## Absence Request (only via Manager Approval)
![Annual Leave Request](OrcHCM_AbsenceRequestWorkflow.png)
### Business Requirement
Company need to have a digital solution to enable workforce to request different types of absences from their managers. 
### Solution Scenerio
Employee requests absence request from his/her manager online. Manager approves or rejects from taskbox. Manager assignment is read from infotype 0500. This is one step workflow process.
### Download Files and Upload to OrchestraHCM
Download [Scheme](/WF_AREQUEST.json) and  [Screen](/orc.ess.tm.absrequest.json), and make your changes according to your business requirements.
### Notes
- Please customize absence types in your time management module.
- You can exclude any of absences in SETOP function options by using EXFILTER.
- There is no file attachment feature in this workflow, for absence types that needs document proof, you can add file component and modify your scheme.
### Versions
- June 4, 2026 - Initial Commit
