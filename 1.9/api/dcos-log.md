---
post_title: DC/OS Log API
nav_title: Log
menu_order: 10
feature_maturity: experimental
---

The [DC/OS Log component](/docs/1.9/overview/architecture/components/#dcos-log) runs on all nodes in the cluster.

For more information about using DC/OS Log, see [Logging](/docs/1.9/administration/logging/).


## Routes

Access to the Log API is proxied through the Admin Router on each node using the following route:

```
/system/v1/logs/v1/
```

Access to the Log API of the agent nodes is also proxied through the master nodes, so that it can be accessed from outside of the cluster:

```
/system/v1/agent/{agent_id}/logs/v1/
```

## Resources

The following resources are available under both of the above routes:

<div class="swagger-section">
  <div id="message-bar" class="swagger-ui-wrap message-success" data-sw-translate=""></div>
  <div id="swagger-ui-container" class="swagger-ui-wrap" data-api="/docs/1.9/api/dcos-log.yaml">

  <div class="info" id="api_info">
    <div class="info_title">Loading docs...</div>
  <div class="info_description markdown"></div>
</div>
