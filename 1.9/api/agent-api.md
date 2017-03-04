---
post_title: Agent API
menu_order: 2
---

Admin Router Agent runs on DC/OS agent nodes and exposes the following API routes, grouped by the component to which they proxy or relate.

- [DC/OS Component Package Manager (Pkgpanda)](#dcos-component-package-manager)
- [DC/OS Diagnostics (3DT)](#dcos-diagnostics)
- [DC/OS Log](#dcos-log)
- [DC/OS Metrics](#dcos-metrics)


<a name="dcos-component-package-manager"></a>
## DC/OS Component Package Manager (Pkgpanda)

|   |
|---|
| Path: `/pkgpanda/`<br/>Backend: `http://pkgpanda/` |

<a name="dcos-diagnostics"></a>
## DC/OS Diagnostics (3DT)

|   |
|---|
| Path: `/system/health/v1`<br/>Backend: `http://<socket>`<br/>Socket: `/run/dcos/3dt.sock` |

## DC/OS Log

|   |
|---|
| Path: `/system/v1/logs/v1/`<br/>Backend: `http://log/` |

## DC/OS Metrics

|   |
|---|
| Path: `/system/v1/metrics/`<br/>Backend: `http://<socket>/`<br/>Socket: `/run/dcos/dcos-metrics-agent.sock` |
