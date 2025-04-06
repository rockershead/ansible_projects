format to put the ssh key before encrypting:

- ssh_private_key: |
  -----BEGIN RSA PRIVATE KEY-----
  ''
  ''
  -----END RSA PRIVATE KEY-----

command to encrypt:
- ansible-vault encrypt secret.yaml

command to run:

- ansible-playbook playbooks/site.yml -i ./inventory/int --vault-password-file .vault_pass