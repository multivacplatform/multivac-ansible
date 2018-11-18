# multivac-ansible [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/multivacplatform/multivac-ansible/blob/master/LICENSE) [![Multivac Discuss](https://img.shields.io/badge/multivac-discuss-ff69b4.svg)](https://discourse.iscpif.fr/c/multivac) [![Multivac Channel](https://img.shields.io/badge/multivac-chat-ff69b4.svg)](https://chat.iscpif.fr/channel/multivac)

## Install and config LDAP client with TLS
Role variables:

```yaml
ldap_base: dc=example,dc=com
ldap_uri: ldap://example.com
ldap_version: 3
ldap_rootbinddn: cn=admin,dc=example,dc=come
ldap_pam_password: md5
ldap_pem_file: /etc/ldap/ca_certs.pem
```

Example of role:
```yaml
roles:
  - {role: openldap_client, ldap_base: "", ldap_uri: "", ldap_version: "", ldap_rootbinddn: "", ldap_pam_password: "", ldap_pem_file: ""}
```

Example of running the playbook:

```bash
ansible-playbook --sudo ldap_client_playbook.yaml --extra-vars "target=ANSIBLE_HOSTS_OR_GROUPS"
```

## Code of Conduct

This, and all github.com/multivacplatform projects, are under the [Multivac Platform Open Source Code of Conduct](https://github.com/multivacplatform/code-of-conduct/blob/master/code-of-conduct.md). Additionally, see the [Typelevel Code of Conduct](http://typelevel.org/conduct) for specific examples of harassing behavior that are not tolerated.

## Copyright and License

Code and documentation copyright (c) 2017 [ISCPIF - CNRS](http://iscpif.fr). Code released under the [MIT license](https://github.com/multivacplatform/multivac-ansible/blob/master/LICENSE).
