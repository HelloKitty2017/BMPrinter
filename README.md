# BMPrinter
BMPrinter is the first open source project from SKYSTAR and BCM

Characteristic
-------------------
1.Has Adapted most of phone with fingerprint above Android N,included XIAOMI，MEIZU，VIVO，OPPO,Samsung and google
2.Has Adapted underscreen fingerprint,include XIAOMI,VIVO,OPPO
3.Has Adapted some phone above Android L


Add to Your project
-------------------
```
Gradle:
implementation project(':bmprinter')
```

Ussage
-------------------
All code is write with kotlin,so it would be best you know kotlin and java.<br/>
1.get BMPrinter
var fingerprintUtil: IFingerprintUtil = createFingerprintUtil()

2.authenticate<br/>
fingerprintUtil?.authenticate { success, errCode, errMsg -> if(success){}}

3.FingerprintFactory
you can see some status for fingerprint authentication in FingerprintFactory.<br/>


About Android P
-------------------
It has change FingerPrint api to BiometricPrompt,and BiometricPrompt only can buid as a dialog.<br/>
BiometricPrompt api is a few, can can not judge fingerprint,so you can still use fingerprintManager but it has been deprecated.<br/>
