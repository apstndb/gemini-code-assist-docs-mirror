---
name: documents/docs.cloud.google.com/sdk/gcloud/reference/gemini/gda-observability-settings/setting-bindings/describe
uri: https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gda-observability-settings/setting-bindings/describe
title: gcloud gemini gda-observability-settings setting-bindings describe
description: Offers tools and libraries that allow you to create and manage resources across Google Cloud.
data_source: docs.cloud.google.com
---

NAME

gcloud gemini gda-observability-settings setting-bindings describe - describe settingBindings

SYNOPSIS

`gcloud gemini gda-observability-settings setting-bindings describe` ( [`SETTING_BINDING`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gda-observability-settings/setting-bindings/describe#SETTING_BINDING) : [`--gda-observability-setting`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gda-observability-settings/setting-bindings/describe#--gda-observability-setting) = `GDA_OBSERVABILITY_SETTING` [`--location`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gda-observability-settings/setting-bindings/describe#--location) = `LOCATION` ) \[ [`GCLOUD_WIDE_FLAG`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/gda-observability-settings/setting-bindings/describe#GCLOUD-WIDE-FLAGS)` …` \]

DESCRIPTION

Describe a settingBinding

EXAMPLES

To describe the settingBinding, run:

```
gcloud gemini gda-observability-settings setting-bindings describe
```

POSITIONAL ARGUMENTS

SettingBinding resource - Name of the resource. The arguments in this group can be used to specify the attributes of this resource. (NOTE) Some attributes are not given arguments in this group but can be set in other ways.

To set the `project` attribute:

- provide the argument `setting_binding` on the command line with a fully specified name;
- provide the argument `--project` on the command line;
- set the property `core/project` .

This must be specified.

`SETTING_BINDING`  
ID of the settingBinding or fully qualified identifier for the settingBinding.

To set the `setting_binding` attribute:

- provide the argument `setting_binding` on the command line.

This positional argument must be specified if any of the other arguments in this group are specified.

`--gda-observability-setting` = `GDA_OBSERVABILITY_SETTING`  
The gdaObservabilitySetting id of the settingBinding resource.

To set the `gda-observability-setting` attribute:

- provide the argument `setting_binding` on the command line with a fully specified name;
- provide the argument `--gda-observability-setting` on the command line.

`--location` = `LOCATION`  
The location id of the settingBinding resource.

To set the `location` attribute:

- provide the argument `setting_binding` on the command line with a fully specified name;
- provide the argument `--location` on the command line.

GCLOUD WIDE FLAGS

These flags are available to all commands: [`--access-token-file`](https://docs.cloud.google.com/sdk/gcloud/reference#--access-token-file) , [`--account`](https://docs.cloud.google.com/sdk/gcloud/reference#--account) , [`--billing-project`](https://docs.cloud.google.com/sdk/gcloud/reference#--billing-project) , [`--configuration`](https://docs.cloud.google.com/sdk/gcloud/reference#--configuration) , [`--flags-file`](https://docs.cloud.google.com/sdk/gcloud/reference#--flags-file) , [`--flatten`](https://docs.cloud.google.com/sdk/gcloud/reference#--flatten) , [`--format`](https://docs.cloud.google.com/sdk/gcloud/reference#--format) , [`--help`](https://docs.cloud.google.com/sdk/gcloud/reference#--help) , [`--impersonate-service-account`](https://docs.cloud.google.com/sdk/gcloud/reference#--impersonate-service-account) , [`--log-http`](https://docs.cloud.google.com/sdk/gcloud/reference#--log-http) , [`--project`](https://docs.cloud.google.com/sdk/gcloud/reference#--project) , [`--quiet`](https://docs.cloud.google.com/sdk/gcloud/reference#--quiet) , [`--trace-token`](https://docs.cloud.google.com/sdk/gcloud/reference#--trace-token) , [`--user-output-enabled`](https://docs.cloud.google.com/sdk/gcloud/reference#--user-output-enabled) , [`--verbosity`](https://docs.cloud.google.com/sdk/gcloud/reference#--verbosity) .

Run `$ `[`gcloud help`](https://docs.cloud.google.com/sdk/gcloud/reference) for details.

API REFERENCE

This command uses the `cloudaicompanion/v1` API. The full documentation for this API can be found at: <https://cloud.google.com/gemini>
