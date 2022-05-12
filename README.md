## Verify Signing Key

Securely download the signing key:

```
$ curl --tlsv1.3 --proto =https --max-time 180 --output ~/gr4unch3r.asc https://raw.githubusercontent.com/gr4unch3r/signing-key/master/0x45BC0540BAFE9A0E.asc
```  

Check key fingerprint without importing the key:

```$ gpg --keyid-format long --import --import-options show-only --with-fingerprint gr4unch3r.asc```  

Verify output:

```Key fingerprint = E3EF 22BC 6DE5 595D F553  89F8 45BC 0540 BAFE 9A0E```  

Import the key:

```$ gpg --import gr4unch3r.asc```  
