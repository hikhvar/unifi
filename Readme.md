# Unifi Controller Helm Chart

This is a highly opinionated helm chart to run the [unifi controller docker image](https://hub.docker.com/r/jacobalberty/unifi) on my k3s cluster in the basement. It assumes [metallb](https://metallb.universe.tf/) for providing a LoadBalancer with the same IP for both TCP und UDP.
Application updates will cause downtime since this chart runs only a single replica of the controller. The target system is really small SOHO deployments accepting to trade downtime for symplicity.
