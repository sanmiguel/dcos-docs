---
post_title: Marathon API
nav_title: Marathon API
menu_order: 5
---

The [Marathon component](/docs/1.9/overview/architecture/components/#marathon) runs on all master nodes.

One of these instances of Marathon is elected as leader, while the rest are hot backups in case of failure. All API requests must go through the Marathon leader. To enforce this, Admin Router proxies requests from any master node to the Marathon leader.

For more information about using Marathon, see [Service Management with Marathon](/docs/1.9/usage/marathon/).


## Routes

Access to the Marathon API is proxied through the Admin Router on each master node using the following route:

```
/marathon/
```


## Resources

<div class="swagger-section">
  <div id="message-bar" class="swagger-ui-wrap message-success" data-sw-translate=""></div>
  <div id="swagger-ui-container" class="swagger-ui-wrap" data-api="/docs/1.9/api/marathon.yaml">

  <div class="info" id="api_info">
    <div class="info_title">Loading docs...</div>
  <div class="info_description markdown"></div>
</div>
