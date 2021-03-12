# [Draft] Ansible role to install RKE2

## What is RKE2?

RKE2, also known as RKE Government, is Rancher's next-generation Kubernetes distribution.

It is a fully conformant Kubernetes distribution that focuses on security and compliance within the U.S. Federal Government sector.

To meet these goals, RKE2 does the following:

    Provides defaults and configuration options that allow clusters to pass the CIS Kubernetes Benchmark with minimal operator intervention
    Enables FIPS 140-2 compliance
    Regularly scans components for CVEs using trivy in our build pipeline

## Prerequisites

Ubuntu, Ansible 2.8

## Run playbook

```sh
ansible-playbook -u root --key-file=~/.ssh/id_rsa -i inventory/hosts.ini -l cluster cluster.yaml
```
