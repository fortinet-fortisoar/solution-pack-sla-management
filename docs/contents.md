| [Home](../README.md) |
| -------------------- |

  # Contents

The **SLA Management** solution pack contains the following resources.

## Module Schema

| Name          | Description                                                                             |
|:--------------|:----------------------------------------------------------------------------------------|
| SLA Templates | SLA Templates in FortiSOAR help create an in-built SLA management for cases and alerts. |

## Connector


| Name           | Description                                            |
|:---------------|:-------------------------------------------------------|
| SLA Calculator | Calculates SLA due date based on locale and work hours.|

## Roles

| Name                 | Description                                                               |
|:---------------------|:--------------------------------------------------------------------------|
| SOC Manager          | Adds Create, Read, and Update permissions for SLA Templates module        |
| Full App Permissions | Adds Create, Read, Update and Delete permissions for SLA Templates module |
| SOC Analyst          | Adds Read permissions for SLA Templates module                            |
| Read-Only User       | Adds Read permissions for SLA Templates module                            |


## Playbook Collection

| 06 - IRP - Case Management |
|:--------------------------:|


| Playbook Name                                                                 | Description                                                                                                            |
|:------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------|
| Alert - [01] Capture All SLA (Upon Create)                                    | Updates the alert's acknowledgement due date and response due date based on the alert's severity.                      |
| Alert - [02] Capture Acknowledge SLA (Upon Update)                            | Updates the alert's acknowledgement date and SLA Status based on when the alert status is changed.                     |
| Alert - [03] Capture Response SLA (Upon Update)                               | Updates the alert's response date and SLA Status based on when the alert status is changed.                            |
| Alert - [04] Check for SLA violations                                         | Checks periodically for violations of acknowledgement SLA of the open alerts.                                          |
| Alert - [05] Update Acknowledge and Response Due dates (Post Severity Change) | Updates the alert's acknowledge due date and response due date for change in the severity of alerts                    |
| Alert - Periodic Update Alert SLA Status                                      | This is a subroutine playbook to periodically check violations of acknowledgement and response SLA of the open alerts. |
| Alert - Update SLA Details                                                    | Updates an alert's acknowledgement due date and response due date based on the severity of the alert.                  |
| Fetch SLA Details                                                             | Fetches SLA Details for cases as per Service, that is, for MSSP or Enterprise.                                         |
| Case - [01] Capture All SLA (Upon Create)                                     | Updates an alert's acknowledgement due date and response due date based on the severity of the case.                   |
| Case - [02] Capture Acknowledge SLA (Upon Update)                             | Updates an case's acknowledgement date and SLA status when the status of the case is changed.                          |
| Case - [03] Capture Response SLA (Upon Update)                                | Update an case's response date and SLA status when the status of the case is changed.                                  |
| Case - [04] Check for SLA violations                                          | Periodically check Acknowledgement SLA violations of the Open Cases.                                                   |
| Case - [05] Update Response and Acknowledge Due date (Post Severity Change)   | Update an case's acknowledgement due date and response due date following a change in severity.                        |
| Case - [06] Check for Acknowledge SLA violations                              | Notifies users of violation of Acknowledgement SLA.                                                                    |
| Case - [07] Check for Response SLA violations                                 | Notifies users of violation of Response SLA.                                                                           |
| Case - Periodic Update Case SLA Status                                        | This is a subroutine playbook to check and update an case's SLA status.                                                |
| Cases - Update SLA Details                                                    | Updates an alert's acknowledgement due date and response due date based on case severity.                              |
| Notify Acknowledge SLA Violation                                              | Notify user for Acknowledgement SLA violation                                                                          |
| Notify Response SLA Violation                                                 | Checks every 5 minutes for Response SLA violations of acknowledged cases.                                              |
| Pause SLA - Alerts                                                            | Pauses the alert's acknowledgement or response when its respective SLA status is changed to 'Awaiting Action'.         |
| Pause SLA - Cases                                                             | Pauses the case's acknowledgement or response SLA when its respective SLA status is changed to 'Awaiting Action'.      |



## Navigation Menu

| Name       |
|:-----------|
| Resources  |

> [!Warning]
> We recommend that you clone these playbooks before customizing to avoid loss of information while upgrading the solution pack.

# Next Steps
| [Installation](./setup.md#installation) | [Configuration](./setup.md#configuration) | [Usage](./usage.md) |
| ----------------------------------------- | ------------------------------------------- | --------------------- |
