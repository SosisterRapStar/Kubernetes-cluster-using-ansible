# Kubernetes-cluster-using-ansible
Demo version for study practise (playbook will be modified)
This playbook installs all prerequisites for kubernetes cluster and starts it.
For cidr subnetwork changes, flannel file need to be configured

# VM config
- Remote system: amd64 Ubuntu server 22.04.4 (4 cores, 2Gb RAM, 14Gb disk)
- VM Network: adapter1 - host-only (Manual configuration), adapter2 - NAT (DHCP)

# Modules config
- SSH: by password
- Container runtime: containerd v1.7.16
- Container cli: nerdctl v 2.0.0-beta.4
- Cgroup driver: systemd
- Runc version: 1.1.12
- CNI plugin: flannel
- Kubernetes version: 1.29
- Ingress controller: ingress-nginx (hostnetwork approach)

# web-apps config
- fastAPI + uvicorn port 8000
