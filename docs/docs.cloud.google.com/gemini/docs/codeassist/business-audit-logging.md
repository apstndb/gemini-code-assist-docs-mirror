---
name: documents/docs.cloud.google.com/gemini/docs/codeassist/business-audit-logging
uri: https://docs.cloud.google.com/gemini/docs/codeassist/business-audit-logging
title: Business AI Code audit logging
description: Reference documentation for Business AI Code audit logs.
data_source: docs.cloud.google.com
---

This document lists the audited methods for Business AI Code. Google Cloud services generate audit logs that record administrative and access activities within your Google Cloud resources. For more information about Cloud Audit Logs, see the following:

  - [Types of audit logs](https://docs.cloud.google.com/logging/docs/audit#types)
  - [Audit log entry structure](https://docs.cloud.google.com/logging/docs/audit#audit_log_entry_structure)
  - [Storing and routing audit logs](https://docs.cloud.google.com/logging/docs/audit#storing_and_routing_audit_logs)
  - [Cloud Logging pricing summary](https://docs.cloud.google.com/stackdriver/pricing#logs-pricing-summary)
  - [Enable Data Access audit logs](https://docs.cloud.google.com/logging/docs/audit/configure-data-access)

## Service name

To view the Business AI Code audit logs, do the following:

1.  In the Google Cloud console, go to the Logs Explorer page:

2.  Copy and paste the following query into the **Query** field of the Logs Explorer, and then click **Run query** .
    
    ``` 
        protoPayload.serviceName="businessaicode.googleapis.com"
      
    ```

## Methods by permission type

Each IAM permission has a `type` property, whose value is an enum that can be one of four values: `ADMIN_READ` , `ADMIN_WRITE` , `DATA_READ` , or `DATA_WRITE` . When you call a method, Business AI Code generates an audit log whose category is dependent on the `type` property of the permission required to perform the method. Methods that require an IAM permission with the `type` property value of `DATA_READ` , `DATA_WRITE` , or `ADMIN_READ` generate [Data Access](https://docs.cloud.google.com/logging/docs/audit#data-access) audit logs. Methods that require an IAM permission with the `type` property value of `ADMIN_WRITE` generate [Admin Activity](https://docs.cloud.google.com/logging/docs/audit#admin-activity) audit logs.

API methods in the following list that are marked with (LRO) are long-running operations (LROs). These methods usually generate two audit log entries: one when the operation starts and another when it ends. For more information see [Audit logs for long-running operations](https://docs.cloud.google.com/logging/docs/audit/understanding-audit-logs#lro) .

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Permission type</th>
<th>Methods</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><code dir="ltr" translate="no">DATA_READ</code></td>
<td><code dir="ltr" translate="no">google.cloud.businessaicode.v1alpha.PredictionService.GenerateContent</code><br />
<code dir="ltr" translate="no">google.cloud.businessaicode.v1alpha.PredictionService.QueryConfig</code><br />
<code dir="ltr" translate="no">google.cloud.businessaicode.v1beta.PredictionService.GenerateContent</code><br />
<code dir="ltr" translate="no">google.cloud.businessaicode.v1beta.PredictionService.QueryConfig</code></td>
</tr>
<tr class="even">
<td><code dir="ltr" translate="no">DATA_WRITE</code></td>
<td><code dir="ltr" translate="no">google.cloud.businessaicode.v1alpha.PredictionService.SendTelemetry</code><br />
<code dir="ltr" translate="no">google.cloud.businessaicode.v1beta.PredictionService.SendTelemetry</code></td>
</tr>
</tbody>
</table>

## API interface audit logs

For information about how and which permissions are evaluated for each method, see the Identity and Access Management documentation for Business AI Code.

### `google.cloud.businessaicode.v1alpha.PredictionService`

The following audit logs are associated with methods belonging to `google.cloud.businessaicode.v1alpha.PredictionService` .

#### `GenerateContent`

  - **Method** : `google.cloud.businessaicode.v1alpha.PredictionService.GenerateContent`  
  - **Audit log type** : [Data access](https://docs.cloud.google.com/logging/docs/audit#data-access)  
  - **Permissions** :
      - `businessaicode.locations.generateContent - DATA_READ`
  - **Method is a long-running or streaming operation** : No.  
  - **Filter for this method** : `protoPayload.methodName="google.cloud.businessaicode.v1alpha.PredictionService.GenerateContent"`  

#### `QueryConfig`

  - **Method** : `google.cloud.businessaicode.v1alpha.PredictionService.QueryConfig`  
  - **Audit log type** : [Data access](https://docs.cloud.google.com/logging/docs/audit#data-access)  
  - **Permissions** :
      - `businessaicode.locations.queryConfiguration - DATA_READ`
  - **Method is a long-running or streaming operation** : No.  
  - **Filter for this method** : `protoPayload.methodName="google.cloud.businessaicode.v1alpha.PredictionService.QueryConfig"`  

#### `SendTelemetry`

  - **Method** : `google.cloud.businessaicode.v1alpha.PredictionService.SendTelemetry`  
  - **Audit log type** : [Data access](https://docs.cloud.google.com/logging/docs/audit#data-access)  
  - **Permissions** :
      - `businessaicode.locations.sendTelemetry - DATA_WRITE`
  - **Method is a long-running or streaming operation** : No.  
  - **Filter for this method** : `protoPayload.methodName="google.cloud.businessaicode.v1alpha.PredictionService.SendTelemetry"`  

### `google.cloud.businessaicode.v1beta.PredictionService`

The following audit logs are associated with methods belonging to `google.cloud.businessaicode.v1beta.PredictionService` .

#### `GenerateContent`

  - **Method** : `google.cloud.businessaicode.v1beta.PredictionService.GenerateContent`  
  - **Audit log type** : [Data access](https://docs.cloud.google.com/logging/docs/audit#data-access)  
  - **Permissions** :
      - `businessaicode.locations.generateContent - DATA_READ`
  - **Method is a long-running or streaming operation** : No.  
  - **Filter for this method** : `protoPayload.methodName="google.cloud.businessaicode.v1beta.PredictionService.GenerateContent"`  

#### `QueryConfig`

  - **Method** : `google.cloud.businessaicode.v1beta.PredictionService.QueryConfig`  
  - **Audit log type** : [Data access](https://docs.cloud.google.com/logging/docs/audit#data-access)  
  - **Permissions** :
      - `businessaicode.locations.queryConfiguration - DATA_READ`
  - **Method is a long-running or streaming operation** : No.  
  - **Filter for this method** : `protoPayload.methodName="google.cloud.businessaicode.v1beta.PredictionService.QueryConfig"`  

#### `SendTelemetry`

  - **Method** : `google.cloud.businessaicode.v1beta.PredictionService.SendTelemetry`  
  - **Audit log type** : [Data access](https://docs.cloud.google.com/logging/docs/audit#data-access)  
  - **Permissions** :
      - `businessaicode.locations.sendTelemetry - DATA_WRITE`
  - **Method is a long-running or streaming operation** : No.  
  - **Filter for this method** : `protoPayload.methodName="google.cloud.businessaicode.v1beta.PredictionService.SendTelemetry"`
