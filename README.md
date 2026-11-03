# NetBird application stack for Kubernetes on Wodby

Deploy a self-hosted NetBird server, a WireGuard-based overlay network, on Kubernetes with Wodby.

This repository defines the Wodby stack manifests and default service
composition for NetBird.

<!-- wodby:generated:start -->

## Stack contract

- [NetBird stack on Wodby](https://wodby.com/stacks/netbird)
- [Browse Wodby application stacks](https://wodby.com/stacks)
- [Wodby stack documentation](https://wodby.com/docs/2.0/stacks/)
- [Stack manifest reference](https://wodby.com/docs/2.0/stacks/template/)

## Service definitions

- [NetBird service](https://github.com/wodby/service-netbird)

## What's included

| Component / service | Default configuration |
| --- | --- |
| NetBird<br>`netbird` | required; enabled by default |

Enabled optional services are selected by default but can be excluded when an
app is created. Disabled optional services are available but not selected by
default. Required services cannot be excluded.

## Validate the stack manifest

```bash
wodby stack validate-manifest stack.yml --org <org-id>
```

<!-- wodby:generated:end -->

## Connect devices

Set **Admin email** and **Admin password** when you create the app, sign in to the dashboard at the `netbird`
service's main domain, and connect each device with `netbird up --management-url https://<main domain>`. Everything
runs over HTTPS, so no ports need publishing. See the
[service README](https://github.com/wodby/service-netbird#connect-devices).
