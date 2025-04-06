I have put 2 environments for the inventory.One is integration and the other is pre-prod. There are group_vars and secret.yaml(ssh_key) associated for the different machines.

format to put the ssh key before encrypting:

- ssh_private_key: |
  - -----BEGIN RSA PRIVATE KEY-----
  - ''
  - ''
  - -----END RSA PRIVATE KEY-----

command to encrypt:
- ansible-vault encrypt secret.yaml

command to run:

- ansible-playbook playbooks/site.yml -i ./inventory/int --vault-password-file .vault_pass