---
post_title: DC/OS Package Manager API
nav_title: Package Manager API
menu_order: 10
---

The [DC/OS Package Manager (Cosmos) component](/docs/1.9/overview/architecture/components/#dcos-package-manager-cosmos) runs on all master nodes.

For information about managing package repositories, see [Managing Package Repositories](/docs/1.9/usage/repo/).

For information about managing services, see [Managing Services](/docs/1.9/usage/managing-services/).


## Routes

Access to the `package` resource of the Package Manager API is proxied through the Admin Router on each node using the following route:

```
/package/
```

Access to the `service` resource of the Package Manager API is served up under a different path:

```
/cosmos/service/
```


## Resources

The following resources are available under both of the above routes:

<div class="swagger-section">
  <div id="message-bar" class="swagger-ui-wrap message-success" data-sw-translate=""></div>
  <div id="swagger-ui-container" class="swagger-ui-wrap" data-api="/docs/1.9/api/package-manager.yaml">

  <div class="info" id="api_info">
    <div class="info_title">Loading docs...</div>
  <div class="info_description markdown"></div>
</div>
