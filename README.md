# Release information

- **Version**: 1.1.2
- **Certified**: Yes
- **Publisher**: Fortinet
- **Compatible version**: FortiSOAR v7.6.5 and later
- [Release notes](./release_notes.md)

# Overview

The SLA Management solution pack tracks and manages service level agreements (SLAs) for alerts and cases in FortiSOAR. It was previously part of the SOAR Framework solution pack and is now distributed as a standalone solution pack.

The solution pack provides the following:

- **SLA calculation**: The SLA Calculator connector calculates acknowledgement and response due dates using the locale-specific holidays and work hours that you configure.

- **SLA templates**: Five templates, one for each severity level, define the acknowledgement time, the response time, and the record statuses that pause the SLA timer.

- **Playbook collection**: Playbooks capture, update, and pause SLAs for alerts and cases, check for violations at scheduled intervals, and notify users when an SLA is missed.

SLA values are applied to alert and case records automatically, and the SLA status of a record is updated as its status changes.

# Next steps

| [Installation](./docs/setup.md#installation) | [Configuration](./docs/setup.md#configuration) | [Usage](./docs/usage.md) | [Contents](./docs/contents.md) |
|:---------------------------------------------|:-----------------------------------------------|:-------------------------|:-------------------------------|