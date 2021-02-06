openssl s_client -connect $INGRESS:443 -servername "marketplace.boutiquestore.com" -CAfile root.crt

CONNECTED(00000003)
depth=1 O = boutiquestore Inc., CN = boutiquestore.com
verify return:1
depth=0 CN = marketplace.boutiquestore.com, O = boutique store
verify return:1
---
Certificate chain
 0 s:CN = marketplace.boutiquestore.com, O = boutique store
   i:O = boutiquestore Inc., CN = boutiquestore.com
---
Server certificate
-----BEGIN CERTIFICATE-----
MIIC7jCCAdYCAQAwDQYJKoZIhvcNAQELBQAwOTEbMBkGA1UECgwSYm91dGlxdWVz
dG9yZSBJbmMuMRowGAYDVQQDDBFib3V0aXF1ZXN0b3JlLmNvbTAeFw0yMTAyMDYx
MDU0MzVaFw0yMjAyMDYxMDU0MzVaMEExJjAkBgNVBAMMHW1hcmtldHBsYWNlLmJv
dXRpcXVlc3RvcmUuY29tMRcwFQYDVQQKDA5ib3V0aXF1ZSBzdG9yZTCCASIwDQYJ
KoZIhvcNAQEBBQADggEPADCCAQoCggEBAJZNbAkfjg3Z/swIh+qv5yaq86WKwBx0
yi39wwbPtIo2LgzmBgMXgWava6sGTY//LeUyqzLo43DOM14juG40kpBtlf+OTCE3
orBIvSJsARAlhnB7bF1u8R7XyW48cuFr4zwh/JYQzXpOPOHg4jxK+/YuDSWb7HTH
IvPRGyTC7GWEIiQqn23giDdezFSGs1vkVAwrlHXItBw2tZglSQikP8xGR5/1PXbW
QWBf+k/Rm0z4qXfmOFqXC5uqqYvxY7teydBQ7OCHZCe/GrT87KwHQAATKp6vHhVc
/MGrKD4iPa3vrSk65fk/i9iYYQ1aVhouPsSns9nojnNWkFISx6mww1cCAwEAATAN
BgkqhkiG9w0BAQsFAAOCAQEA1FfMfIHSL1m66j2XUZPL3rrAeqfatiBUdxR3hl2D
dlhRg6sE+N/9ijyBbr3ZmmJwXSaneOoRrEdpWR0YowDKxyDXsHeqWfZGMYMRs/c4
6ZGWR07hBLBhgFtqwOsRgpnrQARwx1Pl8ZpVHuI5FyuSHyCpHZ2WbMDGIbW9fZDd
Z9hFN+oMacDaM1AGKTxdaFRWhs7O5oAK3aCWGm3VFngSRcYG2OtIEwnm9rn1nKJV
tjw4+APGB3rrKBm5u8+kTzFt5qNSUvtYPd8YEFPVxfJJpECcsgkVlERITvgZb2fP
loozy1UBtJjsDZ500M/iCweFP48vLgPo+rEmtI5RKTwDCA==
-----END CERTIFICATE-----
subject=CN = marketplace.boutiquestore.com, O = boutique store

issuer=O = boutiquestore Inc., CN = boutiquestore.com

---
No client certificate CA names sent
Peer signing digest: SHA256
Peer signature type: RSA-PSS
Server Temp Key: X25519, 253 bits
---
SSL handshake has read 1244 bytes and written 401 bytes
Verification: OK
---
New, TLSv1.3, Cipher is TLS_AES_256_GCM_SHA384
Server public key is 2048 bit
Secure Renegotiation IS NOT supported
Compression: NONE
Expansion: NONE
No ALPN negotiated
Early data was not sent
Verify return code: 0 (ok)
---