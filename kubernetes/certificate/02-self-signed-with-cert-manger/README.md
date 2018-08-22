## script to generate key

```
openssl genrsa -out ca.key 2048
```

so we will get `ca.key`

```
openssl req -x509 -new -nodes -key ca.key -sha256 -subj "/CN=www.praekiko.tk" -days 365 -out ca.crt
```

so we will get `ca.crt`
