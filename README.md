# cipher_test

### Description 
This script will test a SSL/TLS endpoint with the ciphers supported by `openssl s_client`. The script will output a pass/fail notification for all ciphers. 

### Example use
``` 
./cipher.sh redhat.com:443
Obtaining cipher list from LibreSSL 2.8.3.
Testing ECDHE-RSA-AES256-GCM-SHA384...YES
Testing ECDHE-ECDSA-AES256-GCM-SHA384...NO (sslv3 alert handshake failure)
Testing ECDHE-RSA-AES256-SHA384...YES
Testing ECDHE-ECDSA-AES256-SHA384...NO (sslv3 alert handshake failure)
Testing ECDHE-RSA-AES256-SHA...YES
Testing ECDHE-ECDSA-AES256-SHA...NO (sslv3 alert handshake failure)
Testing DHE-RSA-AES256-GCM-SHA384...NO (sslv3 alert handshake failure)
Testing DHE-RSA-AES256-SHA256...YES
Testing DHE-RSA-AES256-SHA...YES
Testing ECDHE-ECDSA-CHACHA20-POLY1305...NO (sslv3 alert handshake failure)
Testing ECDHE-RSA-CHACHA20-POLY1305...NO (sslv3 alert handshake failure)
Testing DHE-RSA-CHACHA20-POLY1305...NO (sslv3 alert handshake failure)
Testing GOST2012256-GOST89-GOST89...NO (sslv3 alert handshake failure)
Testing DHE-RSA-CAMELLIA256-SHA256...NO (sslv3 alert handshake failure)
Testing DHE-RSA-CAMELLIA256-SHA...NO (sslv3 alert handshake failure)
Testing GOST2001-GOST89-GOST89...NO (sslv3 alert handshake failure)
Testing AECDH-AES256-SHA...NO (sslv3 alert handshake failure)
Testing ADH-AES256-GCM-SHA384...NO (sslv3 alert handshake failure)
Testing ADH-AES256-SHA256...NO (sslv3 alert handshake failure)
Testing ADH-AES256-SHA...NO (sslv3 alert handshake failure)
<output truncated>
```
