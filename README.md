# Init

```
docker compose up
```

# Config User Federation

Connection URL
```
ldap://ldap:1389
```

Use Truststore SPI 
```
Never
```

Bind DN
```
cn=admin,dc=example,dc=org
```

Bind credentials
```
admin
```

Users DN
```
ou=users,dc=example,dc=org
```

uid...



# Apache Directory Studio

```
brew install apache-directory-studio
```

```
hostname=localhost
port=1389
BindDNOrUser=cn=admin,dc=example,dc=org
BindPassword=admin
```

# LDAP default attributes

https://docs.bmc.com/docs/fpsc121/ldap-attributes-and-associated-fields-495323340.html

# XPTO
- user1 vai ter o atributo regiao = norte
- user2 vai ter o atributo regiao = nordeste
- criar um group readers
- Todo mundo que é do readers, vai ter um atributo leitor = true
- microprofile-jwt como default para mapear os groups
- Criar um client scope default tambem para termos o mapeamento da regiao, ou utilizar o client scope profile