---
name: documents/docs.cloud.google.com/sdk/gcloud/reference/gemini/release-channel-settings/delete
uri: https://docs.cloud.google.com/sdk/gcloud/reference/gemini/release-channel-settings/delete
title: gcloud gemini release-channel-settings delete
description: Offers tools and libraries that allow you to create and manage resources across Google Cloud.
data_source: docs.cloud.google.com
---

NAME

gcloud gemini release-channel-settings delete - delete releaseChannelSettings

SYNOPSIS

`gcloud gemini release-channel-settings delete` ( [`RELEASE_CHANNEL_SETTING`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/release-channel-settings/delete#RELEASE_CHANNEL_SETTING) : [`--location`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/release-channel-settings/delete#--location) = `LOCATION` ) \[ [`--request-id`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/release-channel-settings/delete#--request-id) = `REQUEST_ID` \] \[ [`GCLOUD_WIDE_FLAG`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/release-channel-settings/delete#GCLOUD-WIDE-FLAGS)` …` \]

DESCRIPTION

Delete a releaseChannelSetting

EXAMPLES

To delete the releaseChannelSetting, run:

```
gcloud gemini release-channel-settings delete
```

POSITIONAL ARGUMENTS

ReleaseChannelSetting resource - Name of the resource The arguments in this group can be used to specify the attributes of this resource. (NOTE) Some attributes are not given arguments in this group but can be set in other ways.

To set the `project` attribute:

- provide the argument `release_channel_setting` on the command line with a fully specified name;
- provide the argument `--project` on the command line;
- set the property `core/project` .

This must be specified.

`RELEASE_CHANNEL_SETTING`  
ID of the releaseChannelSetting or fully qualified identifier for the releaseChannelSetting.

To set the `release_channel_setting` attribute:

- provide the argument `release_channel_setting` on the command line.

This positional argument must be specified if any of the other arguments in this group are specified.

`--location` = `LOCATION`  
The location id of the releaseChannelSetting resource.

To set the `location` attribute:

- provide the argument `release_channel_setting` on the command line with a fully specified name;
- provide the argument `--location` on the command line.

FLAGS

`--request-id` = `REQUEST_ID`  
An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. The server will guarantee that for at least 60 minutes after the first request.

For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments.

The request ID must be a valid UUID with the exception that zero UUID is not supported (00000000-0000-0000-0000-000000000000).

GCLOUD WIDE FLAGS

These flags are available to all commands: [`--access-token-file`](https://docs.cloud.google.com/sdk/gcloud/reference#--access-token-file) , [`--account`](https://docs.cloud.google.com/sdk/gcloud/reference#--account) , [`--billing-project`](https://docs.cloud.google.com/sdk/gcloud/reference#--billing-project) , [`--configuration`](https://docs.cloud.google.com/sdk/gcloud/reference#--configuration) , [`--flags-file`](https://docs.cloud.google.com/sdk/gcloud/reference#--flags-file) , [`--flatten`](https://docs.cloud.google.com/sdk/gcloud/reference#--flatten) , [`--format`](https://docs.cloud.google.com/sdk/gcloud/reference#--format) , [`--help`](https://docs.cloud.google.com/sdk/gcloud/reference#--help) , [`--impersonate-service-account`](https://docs.cloud.google.com/sdk/gcloud/reference#--impersonate-service-account) , [`--log-http`](https://docs.cloud.google.com/sdk/gcloud/reference#--log-http) , [`--project`](https://docs.cloud.google.com/sdk/gcloud/reference#--project) , [`--quiet`](https://docs.cloud.google.com/sdk/gcloud/reference#--quiet) , [`--trace-token`](https://docs.cloud.google.com/sdk/gcloud/reference#--trace-token) , [`--user-output-enabled`](https://docs.cloud.google.com/sdk/gcloud/reference#--user-output-enabled) , [`--verbosity`](https://docs.cloud.google.com/sdk/gcloud/reference#--verbosity) .

Run `$ `[`gcloud help`](https://docs.cloud.google.com/sdk/gcloud/reference) for details.

API REFERENCE

This command uses the `cloudaicompanion/v1` API. The full documentation for this API can be found at: <https://cloud.google.com/gemini>
