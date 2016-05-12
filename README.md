ninfo-plugin-ldap
=================

LDAP plugin for ninfo: https://github.com/JustinAzoff/ninfo


Configuration:

```
[plugin:ldap]
user   = foo
pw     = bar
server = ldaps://ldap.example.com:636
dsn    = ou=People,dc=example,dc=com
```

and optionally:
```
ignore_cert = true
fields = list,of,ldap,fields
strip = text_to_delete_from_output
```

for Active Directory you will want something like:

```
searchpre = sAMAccountName
```
