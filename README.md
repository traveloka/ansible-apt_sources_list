# shared/apt_sources_list #

Installs the optimized Ubuntu sources.list configuration for AWS.

## Requirements ##

Requires Ansible 2.0 or higher.
Requires fact gathering to be enabled in order to determine Ubuntu release.

Role Variables
--------------

    - name: apt_sources_list_aws_region
      desc: AWS region name of the ap mirror
      default: ap-southeast-1

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: shared/apt_sources_list
