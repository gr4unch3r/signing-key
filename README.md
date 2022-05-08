## Verify Signing Key

Securely download the signing key:

```
$ curl --tlsv1.3 --proto =https --max-time 180 --output ~/gr4unch3r.asc https://raw.githubusercontent.com/gr4unch3r/signing-key/master/gr4unch3r.asc
```  

Check key fingerprint without importing the key:

```$ gpg --keyid-format long --import --import-options show-only --with-fingerprint gr4unch3r.asc```  

Verify output:

```Key fingerprint = 4FC8 DF42 3A4D 4F21 80E6  4F58 0537 CE27 BFE2 24D1```  

Import the key:

```$ gpg --import gr4unch3r.asc```  
