## script to generate key

```
openssl req -x509 -nodes -days 365 -newkey rsa:4096 -keyout tls.key -out tls.crt -subj "/CN=www.praekiko.tk"
```

so we will get `tls.key & tls.crt`
