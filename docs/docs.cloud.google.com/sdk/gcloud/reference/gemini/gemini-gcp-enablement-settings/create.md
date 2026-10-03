---
name: documents/docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create
uri: https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create
title: gcloud gemini gemini-gcp-enablement-settings create
description: Offers tools and libraries that allow you to create and manage resources across Google Cloud.
data_source: docs.cloud.google.com
---

NAME

gcloud gemini gemini-gcp-enablement-settings create - create geminiGcpEnablementSettings

SYNOPSIS

`gcloud gemini gemini-gcp-enablement-settings create` ( [`GEMINI_GCP_ENABLEMENT_SETTING`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#GEMINI_GCP_ENABLEMENT_SETTING) : [`--location`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#--location) = `LOCATION` ) \[ [`--custom-instructions`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#--custom-instructions) = `CUSTOM_INSTRUCTIONS` \] \[ [`--disable-web-grounding`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#--disable-web-grounding) \] \[ [`--enable-customer-data-sharing`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#--enable-customer-data-sharing) \] \[ [`--gemini-enterprise-project`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#--gemini-enterprise-project) = `GEMINI_ENTERPRISE_PROJECT` \] \[ [`--labels`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#--labels) =\[ `LABELS` , …\]\] \[ [`--mutations-enabled`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#--mutations-enabled) \] \[ [`--proactive-agents-enabled`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#--proactive-agents-enabled) \] \[ [`--release-channel`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#--release-channel) = `RELEASE_CHANNEL` \] \[ [`--request-id`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#--request-id) = `REQUEST_ID` \] \[ [`--web-grounding-type`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#--web-grounding-type) = `WEB_GROUNDING_TYPE` \] \[ [`GCLOUD_WIDE_FLAG`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gemini-gcp-enablement-settings/create#GCLOUD-WIDE-FLAGS)` …` \]

DESCRIPTION

Create a geminiGcpEnablementSetting

EXAMPLES

To create the geminiGcpEnablementSetting, run:

```
gcloud gemini gemini-gcp-enablement-settings create
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

`--disable-web-grounding`  
Whether web grounding should be disabled. DEPRECATED: Use web_grounding_type instead.

`--enable-customer-data-sharing`  
Not implemented.

`--gemini-enterprise-project` = `GEMINI_ENTERPRISE_PROJECT`  
The Gemini enterprise project for this setting. Format: projects/{project} The `{project}` segment can be the project ID or project number.

`--labels` =\[ `LABELS` ,…\]  
Labels as key value pairs.

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

`--mutations-enabled`  
Indicates whether resource mutations are enabled. If not set, resource mutations are disabled.

`--proactive-agents-enabled`  
Indicates whether proactive agents are enabled. If not set, proactive agents are disabled.

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

GCLOUD WIDE FLAGS

These flags are available to all commands: [`--access-token-file`](https://docs.cloud.google.com/sdk/gcloud/reference#--access-token-file) , [`--account`](https://docs.cloud.google.com/sdk/gcloud/reference#--account) , [`--billing-project`](https://docs.cloud.google.com/sdk/gcloud/reference#--billing-project) , [`--configuration`](https://docs.cloud.google.com/sdk/gcloud/reference#--configuration) , [`--flags-file`](https://docs.cloud.google.com/sdk/gcloud/reference#--flags-file) , [`--flatten`](https://docs.cloud.google.com/sdk/gcloud/reference#--flatten) , [`--format`](https://docs.cloud.google.com/sdk/gcloud/reference#--format) , [`--help`](https://docs.cloud.google.com/sdk/gcloud/reference#--help) , [`--impersonate-service-account`](https://docs.cloud.google.com/sdk/gcloud/reference#--impersonate-service-account) , [`--log-http`](https://docs.cloud.google.com/sdk/gcloud/reference#--log-http) , [`--project`](https://docs.cloud.google.com/sdk/gcloud/reference#--project) , [`--quiet`](https://docs.cloud.google.com/sdk/gcloud/reference#--quiet) , [`--trace-token`](https://docs.cloud.google.com/sdk/gcloud/reference#--trace-token) , [`--user-output-enabled`](https://docs.cloud.google.com/sdk/gcloud/reference#--user-output-enabled) , [`--verbosity`](https://docs.cloud.google.com/sdk/gcloud/reference#--verbosity) .

Run `$ `[`gcloud help`](https://docs.cloud.google.com/sdk/gcloud/reference) for details.

API REFERENCE

This command uses the `cloudaicompanion/v1` API. The full documentation for this API can be found at: <https://cloud.google.com/gemini>
