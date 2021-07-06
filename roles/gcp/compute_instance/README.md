GCP Compute Instance
====================

Manage compute instance(s) on GCP with the given requirements.

Requirements
------------

* The `google.cloud` collection -- installable via `ansible-galaxy collection install google.cloud`

Role Variables
--------------

All variables can be defined in `defaults/main.yml` or overriden at the import of the role. **ALL** of the below values must be defined.

| Name              | Default Value       | Description          |
|-------------------|---------------------|----------------------|
| `gcp_project`     | `cloud-role` |  The name of previously created GCP project that must be available |
| `gcp_cred_kind`     | `serviceaccount` |  Specifies what type of credential being used |
| `gcp_cred_file`     | `~/auth.json` |  Specifies what credential file to be use. The credentials must have appropriate permissions to modify all necessary objects in the tasks. |
| `gcp_region`     | `asia-south2` |  The region to deploy objects to |
| `nodes`     | `` |  Details about the nodes to be deployed |

Dependencies
------------

N/A

Example Playbook
----------------

  ---
  - hosts: localhost
    collections:
      - cloud.roles
      - google.cloud
    vars:
      instance_action: create
    roles:
      - gcp.compute_instance

License
-------

GNU General Public License v3.0 or later

See [LICENSE](../../../LICENSE) to see the full text.
