# LDAP in OpenMediaVault 
The goal of using LDAP in Open Media Vault is to load Users and Groups from an LDAP Directory Service. 

It uses the Linux built-in nss_ldap service to merge the external users into the local OS, and pam_ldap
to authenticate and enable password changing against LDAP servers. All configurations are stored directly
in ldap.conf, except for the password which is placed in... TODO.
Read more on the used services here:
PAM: https://linux.die.net/man/5/pam_ldap
NSS: https://linux.die.net/man/5/nss_ldap