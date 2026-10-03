---
name: documents/docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update
uri: https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update
title: gcloud gemini gemini-gcp-enablement-settings update
description: Offers tools and libraries that allow you to create and manage resources across Google Cloud.
data_source: docs.cloud.google.com
---

NAME

gcloud gemini gemini-gcp-enablement-settings update - update geminiGcpEnablementSettings

SYNOPSIS

`gcloud gemini gemini-gcp-enablement-settings update` ( [`GEMINI_GCP_ENABLEMENT_SETTING`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#GEMINI_GCP_ENABLEMENT_SETTING) : [`--location`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--location) = `LOCATION` ) \[ [`--custom-instructions`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--custom-instructions) = `CUSTOM_INSTRUCTIONS` \] \[ [`--[no-]disable-web-grounding`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--%5Bno-%5Ddisable-web-grounding) \] \[ [`--[no-]enable-customer-data-sharing`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--%5Bno-%5Denable-customer-data-sharing) \] \[ [`--gemini-enterprise-project`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--gemini-enterprise-project) = `GEMINI_ENTERPRISE_PROJECT` \] \[ [`--[no-]mutations-enabled`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--%5Bno-%5Dmutations-enabled) \] \[ [`--[no-]proactive-agents-enabled`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--%5Bno-%5Dproactive-agents-enabled) \] \[ [`--release-channel`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--release-channel) = `RELEASE_CHANNEL` \] \[ [`--request-id`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--request-id) = `REQUEST_ID` \] \[ [`--web-grounding-type`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--web-grounding-type) = `WEB_GROUNDING_TYPE` \] \[ [`--labels`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--labels) =\[ `LABELS` , …\] \| [`--update-labels`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--update-labels) =\[ `UPDATE_LABELS` , …\] [`--clear-labels`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--clear-labels) \| [`--remove-labels`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#--remove-labels) = `REMOVE_LABELS` \] \[ [`GCLOUD_WIDE_FLAG`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/update#GCLOUD-WIDE-FLAGS)` …` \]

DESCRIPTION

Update a geminiGcpEnablementSetting

EXAMPLES

To update the geminiGcpEnablementSetting, run:

```
gcloud gemini gemini-gcp-enablement-settings update
```

POSITIONAL ARGUMENTS

GeminiGcpEnablementSetting resource - Identifier. Name of the resource. Format:projects/{project}/locations/{location}/geminiGcpEnablementSettings/{geminiGcpEnablementSetting} The arguments in this group can be used to specify the attributes of this resource. (NOTE) Some attributes are not given arguments in this group but can be set in other ways.

To set the `project` attribute:

- provide the argument `gemini_gcp_enablement_setting` on the command line with a fully specified name;
- provide the argument `--project` on the command line;
- set the property `core/project` .

This must be specified.

`GEMINI_GCP_ENABLEMENT_SETTING`  
ID of the geminiGcpEnablementSetting or fully qualified identifier for the geminiGcpEnablementSetting.

To set the `gemini_gcp_enablement_setting` attribute:

- provide the argument `gemini_gcp_enablement_setting` on the command line.

This positional argument must be specified if any of the other arguments in this group are specified.

`--location` = `LOCATION`  
The location id of the geminiGcpEnablementSetting resource.

To set the `location` attribute:

- provide the argument `gemini_gcp_enablement_setting` on the command line with a fully specified name;
- provide the argument `--location` on the command line.

FLAGS

`--custom-instructions` = `CUSTOM_INSTRUCTIONS`

Contains custom instructions to be applied to the GCA agent.

`--[no-]disable-web-grounding`

Whether web grounding should be disabled. DEPRECATED: Use web_grounding_type instead. Use `--disable-web-grounding` to enable and `--no-disable-web-grounding` to disable.

`--[no-]enable-customer-data-sharing`

Not implemented. Use `--enable-customer-data-sharing` to enable and `--no-enable-customer-data-sharing` to disable.

`--gemini-enterprise-project` = `GEMINI_ENTERPRISE_PROJECT`

The Gemini enterprise project for this setting. Format: projects/{project} The `{project}` segment can be the project ID or project number.

`--[no-]mutations-enabled`

Indicates whether resource mutations are enabled. If not set, resource mutations are disabled. Use `--mutations-enabled` to enable and `--no-mutations-enabled` to disable.

`--[no-]proactive-agents-enabled`

Indicates whether proactive agents are enabled. If not set, proactive agents are disabled. Use `--proactive-agents-enabled` to enable and `--no-proactive-agents-enabled` to disable.

`--release-channel` = `RELEASE_CHANNEL`

Specifies the release channel for Gemini features. The release channel determines which set of features are available to the user. `RELEASE_CHANNEL` must be one of:

`experimental`  
Experimental release channel.

`stable`  
Stable channel.

`--request-id` = `REQUEST_ID`

An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. The server will guarantee that for at least 60 minutes since the first request.

For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments.

The request ID must be a valid UUID with the exception that zero UUID is not supported (00000000-0000-0000-0000-000000000000).

`--web-grounding-type` = `WEB_GROUNDING_TYPE`

Web grounding type. `WEB_GROUNDING_TYPE` must be one of:

`grounding-with-google-search`  
Grounding with Google Search.

`web-grounding-for-enterprise`  
Grounding with Google Search for Enterprise.

Update labels.

At most one of these can be specified:

`--labels` =\[ `LABELS` ,…\]

Set labels to new value. Labels as key value pairs.

`KEY`  
Keys must start with a lowercase character and contain only hyphens ( `-` ), underscores ( `_` ), lowercase characters, and numbers.

`VALUE`  
Values must contain only hyphens ( `-` ), underscores ( `_` ), lowercase characters, and numbers.

`Shorthand Example:`

```
--labels=string=string
```

`JSON Example:`

```
--labels='{"string": "string"}'
```

`File Example:`

```
--labels=path_to_file.(yaml|json)
```

Or at least one of these can be specified:

`--update-labels` =\[ `UPDATE_LABELS` ,…\]

Update labels value or add key value pair. Labels as key value pairs.

`KEY`  
Keys must start with a lowercase character and contain only hyphens ( `-` ), underscores ( `_` ), lowercase characters, and numbers.

`VALUE`  
Values must contain only hyphens ( `-` ), underscores ( `_` ), lowercase characters, and numbers.

`Shorthand Example:`

```
--update-labels=string=string
```

`JSON Example:`

```
--update-labels='{"string": "string"}'
```

`File Example:`

```
--update-labels=path_to_file.(yaml|json)
```

At most one of these can be specified:

`--clear-labels`  
Clear labels value and set to empty map.

`--remove-labels` = `REMOVE_LABELS`  
Remove existing value from map labels. Sets `remove_labels` value. `Shorthand Example:`

```
--remove-labels=string,string
```

`JSON Example:`

```
--remove-labels=["string"]
```

`File Example:`

```
--remove-labels=path_to_file.(yaml|json)
```

GCLOUD WIDE FLAGS

These flags are available to all commands: [`--access-token-file`](https://docs.cloud.google.com/sdk/gcloud/reference#--access-token-file) , [`--account`](https://docs.cloud.google.com/sdk/gcloud/reference#--account) , [`--billing-project`](https://docs.cloud.google.com/sdk/gcloud/reference#--billing-project) , [`--configuration`](https://docs.cloud.google.com/sdk/gcloud/reference#--configuration) , [`--flags-file`](https://docs.cloud.google.com/sdk/gcloud/reference#--flags-file) , [`--flatten`](https://docs.cloud.google.com/sdk/gcloud/reference#--flatten) , [`--format`](https://docs.cloud.google.com/sdk/gcloud/reference#--format) , [`--help`](https://docs.cloud.google.com/sdk/gcloud/reference#--help) , [`--impersonate-service-account`](https://docs.cloud.google.com/sdk/gcloud/reference#--impersonate-service-account) , [`--log-http`](https://docs.cloud.google.com/sdk/gcloud/reference#--log-http) , [`--project`](https://docs.cloud.google.com/sdk/gcloud/reference#--project) , [`--quiet`](https://docs.cloud.google.com/sdk/gcloud/reference#--quiet) , [`--trace-token`](https://docs.cloud.google.com/sdk/gcloud/reference#--trace-token) , [`--user-output-enabled`](https://docs.cloud.google.com/sdk/gcloud/reference#--user-output-enabled) , [`--verbosity`](https://docs.cloud.google.com/sdk/gcloud/reference#--verbosity) .

Run `$ `[`gcloud help`](https://docs.cloud.google.com/sdk/gcloud/reference) for details.

API REFERENCE

This command uses the `cloudaicompanion/v1` API. The full documentation for this API can be found at: <https://cloud.google.com/gemini>
