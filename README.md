## Enable FIPS on RHEL 7

Credit to Ricky Nelson (https://github.com/rickmanly-nc)

Edit the `main.yml` to update the variables and 'host'.

An Ansible role based on:

- https://access.redhat.com/solutions/137833
- https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html-single/security_guide/index#sect-Federal_Information_Processing_Standard

This role applies FIPS to an existing RHEL 7 server. Recent updates to the playbook now include systems that either have `/boot` on a separate partition or have `/boot` on the same partition as `/`.

2019-08-27:
Added support for BIOS and UEFI systems
Check if already registered
