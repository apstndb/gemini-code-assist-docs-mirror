---
name: documents/docs.cloud.google.com/sdk/gcloud/reference/gemini/code-repository-indexes/update
uri: https://docs.cloud.google.com/sdk/gcloud/reference/gemini/code-repository-indexes/update
title: gcloud gemini code-repository-indexes update
description: Offers tools and libraries that allow you to create and manage resources across Google Cloud.
data_source: docs.cloud.google.com
---

NAME

gcloud gemini code-repository-indexes update - update the configuration of a code repository index instance

SYNOPSIS

`gcloud gemini code-repository-indexes update` ( [`CODE_REPOSITORY_INDEX`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/code-repository-indexes/update#CODE_REPOSITORY_INDEX) : [`--location`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/code-repository-indexes/update#--location) = `LOCATION` ) \[ [`--async`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/code-repository-indexes/update#--async) \] \[ [`--request-id`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/code-repository-indexes/update#--request-id) = `REQUEST_ID` \] \[ [`--labels`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/code-repository-indexes/update#--labels) =\[ `LABELS` , …\] \| [`--update-labels`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/code-repository-indexes/update#--update-labels) =\[ `UPDATE_LABELS` , …\] [`--clear-labels`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/code-repository-indexes/update#--clear-labels) \| [`--remove-labels`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/code-repository-indexes/update#--remove-labels) = `REMOVE_LABELS` \] \[ [`GCLOUD_WIDE_FLAG`](https://docs.cloud.google.com/sdk/gcloud/reference/gemini/code-repository-indexes/update#GCLOUD-WIDE-FLAGS)` …` \]

DESCRIPTION

Update the configuration of a code repository index instance.

EXAMPLES

To update code repository index instance `my-instance` in project `my-project` and location `us-central1` with new labels, run:

```
gcloud gemini code-repository-indexes update `my-instance` --project=my-project --location=us-central1 --labels='{"my_label": "my_value"}'
```

POSITIONAL ARGUMENTS

CodeRepositoryIndex resource - Identifier. name of resource The arguments in this group can be used to specify the attributes of this resource. (NOTE) Some attributes are not given arguments in this group but can be set in other ways.

To set the `project` attribute:

- provide the argument `code_repository_index` on the command line with a fully specified name;
- provide the argument `--project` on the command line;
- set the property `core/project` .

This must be specified.

`CODE_REPOSITORY_INDEX`  
ID of the codeRepositoryIndex or fully qualified identifier for the codeRepositoryIndex.

To set the `code_repository_index` attribute:

- provide the argument `code_repository_index` on the command line.

This positional argument must be specified if any of the other arguments in this group are specified.

`--location` = `LOCATION`  
The location id of the codeRepositoryIndex resource.

To set the `location` attribute:

- provide the argument `code_repository_index` on the command line with a fully specified name;
- provide the argument `--location` on the command line.

FLAGS

`--async`

Return immediately, without waiting for the operation in progress to complete.

`--request-id` = `REQUEST_ID`

An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. The server will guarantee that for at least 60 minutes since the first request.

The request ID must be a valid UUID with the exception that zero UUID is not supported (00000000-0000-0000-0000-000000000000).

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
