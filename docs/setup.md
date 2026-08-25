| [Home](../README.md) |
| -------------------- |

# Installation

1. Click **Content Hub** <picture><source media="(prefers-color-scheme: dark)" srcset="./res/icon-chevron-light.svg"><img alt="then" src="./res/icon-chevron-dark.svg"></picture> **Discover**.
2. Search for **SLA Management** in the list of solution packs.
3. Click the **SLA Management** solution pack card.
4. Click **Install**.

## Prerequisites

The **SLA Management** solution pack depends on the following solution pack, which is installed automatically if it is not already installed.

| Solution pack name | Version         | Purpose                            |
|:-------------------|:----------------|:-----------------------------------|
| SOAR Framework     | v3.0.0 or later | Required for Case Response modules |

To create and manage SLAs, you must be assigned a role with the following minimum permissions:

1. `Create`, `Read`, and `Update` permissions on the **SLA Templates** module
2. `Execute` permission on the **Playbooks** module
3. `Usage` permission on the **Widgets** module
4. Default `Read` permission on the **Application** module
5. Permissions on the **Alerts** and **Cases** modules, if you want to view SLA values within those records

# Configuration

The solution pack includes the **SLA Calculator** connector, which calculates SLA due dates based on the locale and work hours that you specify. Configure the connector before you use the SLA playbooks.

To configure the connector, see [Configuring SLA Calculator](https://docs.fortinet.com/fortisoar/connectors/slacalc).

>[!Note]
>The SLA Calculator connector requires the SOAR Framework solution pack for its supporting playbooks and module changes.

# Next steps

| [Usage](./usage.md) | [Contents](./contents.md) |
|:--------------------|:--------------------------|