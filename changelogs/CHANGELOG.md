# x86\_39\.vm\_utils Release Notes

**Topics**

- <a href="#v8-1-0">v8\.1\.0</a>
    - <a href="#release-summary">Release Summary</a>
    - <a href="#major-changes">Major Changes</a>
- <a href="#v8-0-1">v8\.0\.1</a>
    - <a href="#bugfixes">Bugfixes</a>
- <a href="#v8-0-0">v8\.0\.0</a>
    - <a href="#release-summary-1">Release Summary</a>
    - <a href="#major-changes-1">Major Changes</a>
- <a href="#v7-0-0">v7\.0\.0</a>
    - <a href="#major-changes-2">Major Changes</a>
- <a href="#v6-1-0">v6\.1\.0</a>
    - <a href="#bugfixes-1">Bugfixes</a>
- <a href="#v6-0-0">v6\.0\.0</a>
    - <a href="#release-summary-2">Release Summary</a>
    - <a href="#major-changes-3">Major Changes</a>
- <a href="#v5-1-0">v5\.1\.0</a>
    - <a href="#release-summary-3">Release Summary</a>
- <a href="#v5-0-0">v5\.0\.0</a>
    - <a href="#release-summary-4">Release Summary</a>
    - <a href="#major-changes-4">Major Changes</a>
- <a href="#v4-1-0">v4\.1\.0</a>
    - <a href="#release-summary-5">Release Summary</a>
    - <a href="#bugfixes-2">Bugfixes</a>
- <a href="#v4-0-1">v4\.0\.1</a>
    - <a href="#release-summary-6">Release Summary</a>
    - <a href="#bugfixes-3">Bugfixes</a>
- <a href="#v4-0-0">v4\.0\.0</a>
    - <a href="#release-summary-7">Release Summary</a>
    - <a href="#major-changes-5">Major Changes</a>
- <a href="#v3-1-0">v3\.1\.0</a>
    - <a href="#release-summary-8">Release Summary</a>
    - <a href="#minor-changes">Minor Changes</a>
- <a href="#v3-0-0">v3\.0\.0</a>
    - <a href="#release-summary-9">Release Summary</a>
    - <a href="#major-changes-6">Major Changes</a>
    - <a href="#breaking-changes--porting-guide">Breaking Changes / Porting Guide</a>
- <a href="#v2-0-0">v2\.0\.0</a>
    - <a href="#release-summary-10">Release Summary</a>
    - <a href="#major-changes-7">Major Changes</a>
- <a href="#v1-0-0">v1\.0\.0</a>
    - <a href="#release-summary-11">Release Summary</a>
    - <a href="#major-changes-8">Major Changes</a>

<a id="v8-1-0"></a>
## v8\.1\.0

<a id="release-summary"></a>
### Release Summary

New namespace\: x86\_39

<a id="major-changes"></a>
### Major Changes

* Move repo to github\.com/x86\-39

<a id="v8-0-1"></a>
## v8\.0\.1

<a id="bugfixes"></a>
### Bugfixes

* Fix changing remote backend

<a id="v8-0-0"></a>
## v8\.0\.0

<a id="release-summary-1"></a>
### Release Summary

Overhaul terraform\_remote\_backend\.yml

<a id="major-changes-1"></a>
### Major Changes

* Add new variables to terraform\_remote\_backend\.yml

<a id="v7-0-0"></a>
## v7\.0\.0

<a id="major-changes-2"></a>
### Major Changes

* Allow getting variables from env vars for certain options in playbooks\. Check playbook documentation for more information\.

<a id="v6-1-0"></a>
## v6\.1\.0

<a id="bugfixes-1"></a>
### Bugfixes

* Fix handler in terraform\_remote\_backend\.yml

<a id="v6-0-0"></a>
## v6\.0\.0

<a id="release-summary-2"></a>
### Release Summary

This release adds a new playbook terraform\_remote\_backend\.yml and reworks terraform\_inv\_mgt\.yml

<a id="major-changes-3"></a>
### Major Changes

* Add terraform\_remote\_backend\.yml playbook
* Rework terraform\_inv\_mgt\.yml playbook to place the whole file instead of modifying in place

<a id="v5-1-0"></a>
## v5\.1\.0

<a id="release-summary-3"></a>
### Release Summary

Fix handling for subdomains for /etc/hosts

<a id="v5-0-0"></a>
## v5\.0\.0

<a id="release-summary-4"></a>
### Release Summary

Complete overhaul of all playbooks

<a id="major-changes-4"></a>
### Major Changes

* Added new variables \(check playbook docs\)
* Changed default terraform path to /terraform/\<purpose\>/\<provider\>
* Changed default tfvars path to /tfvars/\<purpose\>/\<provider\>/\<env\>\.tfvars
* Changed variable precedence to prefer shortcuts

<a id="v4-1-0"></a>
## v4\.1\.0

<a id="release-summary-5"></a>
### Release Summary

Fix removing hostnames

<a id="bugfixes-2"></a>
### Bugfixes

* Fix removing hostnames

<a id="v4-0-1"></a>
## v4\.0\.1

<a id="release-summary-6"></a>
### Release Summary

Fix vyos compile

<a id="bugfixes-3"></a>
### Bugfixes

* Fix typo in vyos compile

<a id="v4-0-0"></a>
## v4\.0\.0

<a id="release-summary-7"></a>
### Release Summary

Add workspaces support for a smaller setup footprint

<a id="major-changes-5"></a>
### Major Changes

* Add workspaces support
* Change variables\, check documentation

<a id="v3-1-0"></a>
## v3\.1\.0

<a id="release-summary-8"></a>
### Release Summary

Minor changes to terraform\_inv\_mgt

<a id="minor-changes"></a>
### Minor Changes

* Make inventory\_path overridable in terraform\_inv\_mgt
* Update README\.md

<a id="v3-0-0"></a>
## v3\.0\.0

<a id="release-summary-9"></a>
### Release Summary

This release adds workspace support to terraform playbooks\. It also requires my fork of cloud\.terraform collection\.

<a id="major-changes-6"></a>
### Major Changes

* add workspace support in terraform playbooks

<a id="breaking-changes--porting-guide"></a>
### Breaking Changes / Porting Guide

* now requires my fork of cloud\.terraform collection
* workspace now defaults to provider\-env\, instead of \"default\"

<a id="v2-0-0"></a>
## v2\.0\.0

<a id="release-summary-10"></a>
### Release Summary

This release is a major overhaul of the terraform\_vms playbook\. It is now much more flexible and can be used to create and destroy VMs in a much more dynamic way\.

<a id="major-changes-7"></a>
### Major Changes

* Added new playbook terraform\_dns for changing DNS records through Ansible w/ Terraform
* Added new playbook terraform\_inv\_mgt for changing inventory sources
* Rewrote terraform\_vms playbook\, CHECK NEW DOCUMENTATION

<a id="v1-0-0"></a>
## v1\.0\.0

<a id="release-summary-11"></a>
### Release Summary

initial release

<a id="major-changes-8"></a>
### Major Changes

* add terraform\_vms playbook
* add vyos\_qcow2\_image role
