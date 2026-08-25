| [Home](../README.md) |
| -------------------- |

# Usage

The **SLA Management** solution pack contains playbooks that track the SLAs of alerts and cases automatically. The **SLA Calculator** connector calculates the SLA due dates based on the locale and work hours that you specify.

## Working with SLA templates

The solution pack contains one SLA template for each severity level defined for alerts and cases:

- Critical
- High
- Medium
- Low
- Minimal

![List of SLA templates in the SLA Templates module](./res/sla-templates.png)

The same SLA template applies to both alerts and cases.

To view or edit an existing SLA template:

1. Click **Automation** <picture><source media="(prefers-color-scheme: dark)" srcset="./res/icon-chevron-light.svg"><img alt="then" src="./res/icon-chevron-dark.svg"></picture> **SLA Templates** in the left navigation bar.

2. Click the template that you want to view or edit. For example, click **High** to edit the SLA parameters for alerts and cases whose severity is set to **High**.

    ![SLA template detail view showing acknowledge and response times for alerts and cases](./res/editing-sla-template.png)

    The template contains the following fields:

    - **Pause Case SLA On** and **Pause Alert SLA On**: The case status and alert status that trigger the playbooks to pause the SLA timer. By default, the case SLA pauses when the case status changes to `Awaiting`, and the alert SLA pauses when the alert status changes to `Pending`.

    - **Case Acknowledge Time** and **Alert Acknowledge Time**: The time within which a case or alert must be acknowledged, set to **20** minutes by default. The acknowledgement SLA is tracked when the case status changes to `In Progress` and the alert status changes to `Investigating`.

    - **Case Response Time** and **Alert Response Time**: The time within which a case or alert must be resolved, set to **30** minutes by default. The response SLA is tracked when the case status changes to `Resolved` and the alert status changes to `Closed`.

>[!Note]
>Changes to SLA values take effect in real time.

## Viewing SLAs on a record

The detail view of an alert or case record displays fields such as *Acknowledge Due Date*, *Acknowledge Date*, *Acknowledge SLA*, and *Response Due Date*, which show whether the SLAs are met, missed, or awaiting action.

1. Click **Alerts** in the left navigation bar to view alert records, or **Incident Response** <picture><source media="(prefers-color-scheme: dark)" srcset="./res/icon-chevron-light.svg"><img alt="then" src="./res/icon-chevron-dark.svg"></picture> **Cases** to view case records.

2. Click a record to open its detail view.

![Alert detail view showing a met acknowledge SLA and a running response SLA timer](./res/viewing-sla-record.png)

In the preceding example:

- The alert severity is **High**, and its **Acknowledge SLA** is **Met**, because the alert status was set to **Investigating** within the acknowledgement time.
- The response SLA timer is running, with 23 minutes and 18 seconds elapsed.
- The **Response SLA** is set to **Awaiting Action**.
- The **Response SLA** changes to **Met** or **Missed** depending on when the alert status is set to **Closed**.

# Next steps

| [Installation](./setup.md#installation) | [Configuration](./setup.md#configuration) | [Contents](./contents.md) |
|:----------------------------------------|:------------------------------------------|:--------------------------|