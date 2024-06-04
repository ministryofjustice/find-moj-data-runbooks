---
owner_slack: "#data-catalogue"
title: Configure DBT (Create a Derived Table) to send metadata to the catalogue
last_reviewed_on: 2024-06-04
review_in: 3 months
---

# <%= current_page.data.title %>

The data catalogue uses DBT as a source of metadata about the Analytical Platform.

By default, all models and sources will be ingested into the Datahub catalogue, but they will not be shown in the Find MOJ Data service.

## Make a model or source visible

To make a model or source visible in the Find MOJ Data frontend, set the `dc_display_in_catalogue` tag.

For example, in `dbt_project.yaml` you can include

```yaml
models:
    courts:
        some_subdirectory:
            common_platform_derived:
                +tags:
                    - dc_display_in_catalogue
```

This tag should be used for sources and derived tables that users are expected to work with directly. Don't add it to intermediate/staging tables.

## Set required metadata

When adding new entities to the catalgoue, we require that you specify some additional metadata in DBT. For example:

```yaml
models:
    courts:
        +meta:
            dc_slack_channel_name: #ask-data-engineering
            dc_slack_channel_url: https://moj.enterprise.slack.com/archives/C8X3PP1TN
            dc_owner_id: Joe.Bloggs
```

This metadata can be set at any level but we recommend setting it at the domain level.

The required fields are as follows:

| field name | description | example |
| -- | -- | -- |
| dc_slack_channel_name | The name of a slack channel to be used as a contact point for users of the catalogue service, including the leading '#'. Note: this is not the same as the owner channel for notifications. | `#data-engineering` |
| dc_slack_channel_url | The URL to the slack channel | `https://moj.enterprise.slack.com/archives/C8X3PP1TN` |
| dc_owner_id | The Datahub user ID for the [data owner](https://www.gov.uk/government/publications/essential-shared-data-assets-and-data-ownership-in-government/data-ownership-in-government-html#data-owner-2), usually in the form FirstName.LastName. This is the senior individual accountable for the data, *not* a data custodian. This is not the same as the DBT owner. | `Joe.Bloggs` |

## Additional metadata

| field name | description | example |
| -- | -- | -- |
| dc_where_to_access_dataset | An enum representing how the data can be accessed by end users. For DBT, this always defaults to AnalyticalPlatform. | AnalyticalPlatform |

## Ensure the data owner has an account in Datahub

The owner's Datahub account must exist before you set the `dc_owner_id`. This will happen automatically the first time they log into Datahub.

The user ID is visible in the URL of a user page in Datahub, e.g.

https://datahub-catalogue-dev.apps.live.cloud-platform.service.justice.gov.uk/user/**urn:li:corpuser:Joe.Bloggs**/owner%20of

Speak to the Data catalogue team if you would like us to manually add a set of users without them logging in.
