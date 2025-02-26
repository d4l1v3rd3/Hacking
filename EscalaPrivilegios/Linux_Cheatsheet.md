# Introducción

En este .md ire añadiendo comandos y rutas importantes que me parecen a la hora de escalar privilegios en Linux (Mi experiencia, mis comandos)

Dejo este repositorio para Enumeración de Linux en /tmp automáticamente

```
https://github.com/rebootuser/LinEnum.git
```

Dejo por aquí el comando principal a la hora de entrar en una máquina linux

```
id
```

## /etc/shadow

### Lectura

```
ls -l /etc/shadow
cat /etc/shadow
```

Si encontramos un usuario o hash pass podemos utilizar john

```
john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt
```

### Escritura

```
ls -l /etc/shadow
mkpasswd -m sha-512 pass
```

O otra

````
openssl passwd newpasswordhere
```







