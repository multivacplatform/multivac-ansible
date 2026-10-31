# Provisioning configuration

The LDAP role defaults to anonymous account lookup using existing directory ACLs; users authenticate with their own LDAP passwords. Configure a dedicated search identity only where required, with credentials supplied outside Git. Certificate verification remains enabled. The included public LDAP CA expires 27 October 2036; renew the server certificate before 29 October 2028. No private key or personal password belongs in this repository.

Deployment revision records may be maintained separately from the installed code snapshot.
