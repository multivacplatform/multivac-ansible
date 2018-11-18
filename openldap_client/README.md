# openldap_client

## Install and config LDAP client with TLS
Role variables:

```bash
ldap_base: dc=example,dc=com
ldap_uri: ldap://example.com
ldap_version: 3
ldap_rootbinddn: cn=admin,dc=example,dc=come
ldap_pam_password: md5
ldap_pem_file: /etc/ldap/ca_certs.pem
```

Example role:
```bash
roles:
  - {role: openldap_client, ldap_base: "", ldap_uri: "", ldap_version: "", ldap_rootbinddn: "", ldap_pam_password: "", ldap_pem_file: ""}
```

Example playbook execution:

```bash
ansible-playbook --sudo ldap_client_playbook.yaml --extra-vars "target=ANSIBLE_HOSTS_OR_GROUPS"
```
