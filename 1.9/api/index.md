---
post_title: DC/OS API
nav_title: API
menu_order: 4
---

The DC/OS API is a collection of microservice component APIs made available through [Admin Router](/docs/1.9/overview/architecture/components/#admin-router), an API gateway.


## Topology

A version of Admin Router runs on every DC/OS node.

**Admin Router** runs on the master nodes and serves as the primary API gateway to interact with DC/OS components.

For a list of routes available on master nodes, see [Master Routes](/docs/1.9/api/master-routes/).

**Admin Router Agent** runs on the agent nodes and provides routes for monitoring, debugging, and administration.

Some agent routes, like logs and metrics, are proxied through the master Admin Router to allow external access.
Other routes, like component health and management, are for internal use only.

For a list of routes available on agent nodes, see [Agent Routes](/docs/1.9/api/agent-routes/).


## Route Types

Routes are generally one of three types:

**Backend** routes proxy to a component API.

**File** routes serve up static files.

**Redirect** routes return a permanent (301) or temporary (302) HTTP redirect to another route.


## Component APIs

Many of the DC/OS components have their own APIs.

The primary method of reaching the component APIs is through the Admin Router [Master API](/docs/1.9/api/master-api/).

- Cluster Management
  - [Apache Mesos](https://mesos.apache.org/documentation/latest/endpoints/)
  - [Exhibitor](https://github.com/soabase/exhibitor/wiki/REST-Introduction)
- Container Orchestration
  - [Marathon](/docs/1.9/api/marathon/)
  - [DC/OS Jobs (Metronome)](https://dcos.github.io/metronome/docs/generated/api.html)
- Logging and Metrics
  - [DC/OS Diagnostics (3DT)](/docs/1.9/administration/monitoring/#system-health-http-api-endpoint)
  - [DC/OS Log](/docs/1.9/api/dcos-log/)
  - [DC/OS Metrics](/docs/1.9/api/dcos-metrics/)
  - [DC/OS History](https://github.com/dcos/dcos/tree/master/packages/dcos-history/extra#api)
- Networking
  - [Mesos DNS](/docs/1.9/usage/service-discovery/mesos-dns/http-interface/)
  - Navstar (Coming Soon)
- Package Management
  - [DC/OS Package Manager (Cosmos)](https://github.com/dcos/cosmos#api-method-version-compatibility)
  - [DC/OS Component Package Manager (Pkgpanda)](/docs/1.9/administration/component-management/)
- IAM and Security
  - [DC/OS Authentication](#dcos-authentication)

For more about the components and their function, see [Components](/docs/1.9/overview/architecture/components/).
