---
post_title: DC/OS Metrics API
nav_title: Metrics
feature_maturity: experimental
menu_order: 10
---

The [DC/OS Metrics component](/docs/1.9/overview/architecture/components/#dcos-metrics) runs on all nodes in the cluster.

For more information about using DC/OS Metrics, see [Metrics](/docs/1.9/administration/metrics/).


## Routes

Access to the Metics API is proxied through the Admin Router on each node using the following route:

```
/system/v1/metrics/v1/
```

Access to the Metics API of the agent nodes is also proxied through the master nodes, so that it can be accessed from outside of the cluster:

```
/system/v1/agent/{agent_id}/metrics/v1/
```


## Format

The Metrics API request and response bodies are formatted in JSON.

Requests must include the accept header:

```
Accept: application/json
```

Responses will include the content type header:

```
Content-Type: application/json
```


## Resources

The following resources are available under both of the above routes:

<div class="swagger-section">
  <div id="message-bar" class="swagger-ui-wrap message-success" data-sw-translate=""></div>
  <div id="swagger-ui-container" class="swagger-ui-wrap" data-api="/docs/1.9/api/dcos-metrics.yaml">

  <div class="info" id="api_info">
    <div class="info_title">Loading docs...</div>
  <div class="info_description markdown"></div>
</div>
