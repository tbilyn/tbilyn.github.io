Generate RSA private key 2048 bit, and store in file private.pem
```
openssl genrsa -out private.pem 2048
```

Generate PEM public key based on private key in file private.pem and store it in public.pem
```
openssl rsa -pubout -in private.pem -out public.pem -outform PEM
```

View the md5 hash of the modulus of the private key
```
openssl rsa -noout -modulus -in key.key | openssl md5
```

View the md5 hash of the modulus of the CSR
```
openssl req -noout -modulus -in mycsr.csr | openssl md5
```

View the md5 hash of the modulus of the certificate
```
openssl x509 -noout -modulus -in mycert.crt | openssl md5
```
