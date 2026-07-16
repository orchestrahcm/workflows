# Workflows
Scheme Based Business Workflows with UI Designs for Web and Mobile

OrchestraHCM helps teams digitize HR processes with speed, clarity, and confidence.
With flexible workflow design and user-friendly screens, it turns complex approvals into smooth daily operations.
From web to mobile, OrchestraHCM delivers a modern employee experience while giving managers full control.

- [Annual Leave Request](#annual-leave-request-only-via-manager-approval) - A single-step process where annual leave requests are submitted for manager approval.
- [Annual Leave Request (Expat)](#annual-leave-request-expat-only-via-manager-approval) - A single-step process for expat employees where annual leave requests are submitted for manager approval.
- [Absence Request](#absence-request-only-via-manager-approval) - A single-step manager approval process for different types of absence requests.
- [Photo Update Workflow](#photo-update-workflow) - A workflow for employee photo update requests.
- [NonFlextime Overtime Notification](#nonflextime-overtime-notification-only-via-manager-approval) - A single-step manager approval process for overtime worked outside the employee's flexible working hours.
- [Time Off Request](#time-off-request) - A single-step manager approval process for requesting time off in return for previously worked overtime.
- [Half Day Annual Leave Request](#half-day-annual-leave-request-only-via-manager-approval) - A single-step manager approval process for requesting half-day annual leave.
- [Half Day Annual Leave Request (Expat)](#half-day-annual-leave-request-expat-only-via-manager-approval) - A single-step manager approval process for expat employees to request half-day annual leave.
- [Remote Work Notification](#remote-work-notification-only-via-manager-approval) - A single-step manager approval process for employees to notify their manager of remote working days.

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
- 
## Annual Leave Request (Expat) (only via Manager Approval)
![Annual Leave Request (Expat)](OrcHCM_AnnualLeaveRequestExpatWorkflow.png)
### Business Requirement
Company needs a digital solution to enable expat employees to request annual leave from their managers.
### Solution Scenerio
Expat employee requests annual leave from his/her manager online. Manager approves or rejects from taskbox. This is a one-step workflow process.
### Download Files and Upload to OrchestraHCM
Download [Scheme](/WF_LEAVEX.json) and  [Screen](/orc.ess.tm.requestleavembtexpat.json), and make your changes according to your business requirements.
### Notes
- Please customize absence types in your time management module, annual leave absence type in scheme is 1000, if different please modify in INFTY function.
### Versions
- July 16, 2026 - Initial Commit

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

## Photo Update Workflow
![Photo Update Workflow](OrcHCM_PhotoRequestWorkflow.png)
### Business Requirement
Company need to have a digital solution to enable workforce to update profile photos through a controlled approval process.
### Solution Scenerio
Employee submits a profile photo update request online. HR expoert reviews and approves or rejects from taskbox.
### Download Files and Upload to OrchestraHCM
Download [Scheme](/WF_FLEX.json) and [Screen](/orc.ess.tm.requestaddtime.json), and make your changes according to your business requirements.
### Notes
- You can define photo validation rules (file type, size, and image dimensions) in your screen and scheme logic.
- When employee 's photo approved, user should refresh the page to see her/his photo in app header.
- If your organization needs additional approvals, you can extend the scheme with extra approval steps.
### Versions
- June 4, 2026 - Initial Commit

## NonFlextime Overtime Notification (only via Manager Approval)
![NonFlextime Overtime Notification](OrcHCM_NonFlextimeOvertimeNotification.png)
### Business Requirement
Company need to have a digital solution to enable employees to notify overtime worked outside their flexible working hours through a controlled approval process.
### Solution Scenerio
Employee submits an overtime notification for hours worked outside flexible working hours online. Manager reviews and approves or rejects the request from taskbox.
### Download Files and Upload to OrchestraHCM
Download [Scheme](/WF_LREQUEST.json) and  [Screen](/orc.ess.tm.leavereq.json), and make your changes according to your business requirements.
### Notes
- You can define overtime hour/hours in your screen and scheme logic.
- When the employee's overtime notification is approved, it is automatically reflected in the relevant reporting/payroll processes.
- If your organization needs additional approvals, you can extend the scheme with extra approval steps.
### Versions
- July 16, 2026 - Initial Commit

## Time Off Request
![Time Off Request](OrcHCM_TimeOffRequestWorkflow.png)
### Business Requirement
Company needs a digital solution to enable employees to request time off of previously worked overtime through a controlled approval process.
### Solution Scenerio
Employee submits a time off request from his/her manager online. Manager approves or rejects from taskbox. Manager can also wants revision. When the manager requests a revision, personnel can resend or cancel the request. This is a one-step workflow process.
### Download Files and Upload to OrchestraHCM
Download [Scheme](/WF_FREETIME.json) and [Screen](/orc.ess.tm.requestfreetime.json), and make your changes according to your business requirements.
### Notes
- You can define the maximum time off balance and eligibility rules in your screen and scheme logic.
- The requested time off is automatically deducted from the employee's accrued balance upon approval.
- If your organization needs additional approvals, you can extend the scheme with extra approval steps.
### Versions
- July 16, 2026 - Initial Commit

## Half Day Annual Leave Request (only via Manager Approval)
![Half Day Annual Leave Request](OrcHCM_HalfDayAnnualLeaveRequestWorkflow.png)
### Business Requirement
Company needs a digital solution to enable employees to request half-day annual leave from their managers.
### Solution Scenerio
Employee requests half-day annual leave from his/her manager online. Manager approves or rejects from taskbox. This is a one-step workflow process.
### Download Files and Upload to OrchestraHCM
Download [Scheme](/WF_HDAYLEAVE.json) and [Screen](/orc.ess.tm.requesthdayleave.json), and make your changes according to your business requirements.
### Notes
- If your organization needs additional approvals, you can extend the scheme with extra approval steps.
### Versions
- July 16, 2026 - Initial Commit

## Half Day Annual Leave Request (Expat) (only via Manager Approval)
![Half Day Annual Leave Request (Expat)](OrcHCM_HalfDayAnnualLeaveRequestExpatWorkflow.png)
### Business Requirement
Company needs a digital solution to enable expat employees to request half-day annual leave from their managers.
### Solution Scenerio
Expat employee requests half-day annual leave from his/her manager online. Manager approves or rejects from taskbox. This is a one-step workflow process.
### Download Files and Upload to OrchestraHCM
Download [Scheme](/WF_HDAYLEAVEX.json) and [Screen](/orc.ess.tm.requesthdayleaveexpat.json), and make your changes according to your business requirements.
### Notes
- If your organization needs additional approvals, you can extend the scheme with extra approval steps.
### Versions
- July 16, 2026 - Initial Commit

## Remote Work Notification (only via Manager Approval)
![Remote Work Notification](OrcHCM_RemoteWorkNotification.png)
### Business Requirement
Company needs a digital solution to enable workforce to notify their managers of remote working days through a controlled approval process.
### Solution Scenerio
Employee submits a remote work notification for his/her manager online. Manager approves or rejects from taskbox. Manager can also wants revision. When the manager requests a revision, personnel can resend or cancel the request. This is a one-step workflow process.
### Download Files and Upload to OrchestraHCM
Download [Scheme](/WF_REMOTE.json) and [Screen](/orc.ess.tm.requesthomeofficeinf.json), and make your changes according to your business requirements.
### Notes
- You can define the maximum number of remote working days per week/month in your screen and scheme logic.
- If your organization needs additional approvals, you can extend the scheme with extra approval steps.
### Versions
- July 16, 2026 - Initial Commit
