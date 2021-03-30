# fedora-ostree-pruner

Source code that prunes OSTree repos based on policy.

It is run in Fedora's Openshift instances (prod, stg). The
playbook and the source yaml files to run it are located under
the following two source code directories in the Fedora Infra
ansible repo:

- https://infrastructure.fedoraproject.org/cgit/ansible.git/tree/playbooks/openshift-apps/fedora-ostree-pruner.yml
- https://infrastructure.fedoraproject.org/cgit/ansible.git/tree/roles/openshift-apps/fedora-ostree-pruner/templates
