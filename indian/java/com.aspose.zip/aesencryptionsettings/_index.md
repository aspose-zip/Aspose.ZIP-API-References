---
title: "AesEncryptionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ZIP संग्रह के भीतर AES एन्क्रिप्शन और डिक्रिप्शन एल्गोरिदम के लिए सेटिंग्स।"
type: docs
weight: 10
url: /hi/java/com.aspose.zip/aesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class AesEncryptionSettings extends EncryptionSettings
```

ZIP संग्रह के भीतर AES एन्क्रिप्शन और डिक्रिप्शन एल्गोरिदम के लिए सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [AesEncryptionSettings(String password, EncryptionMethod method)](#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-) | नया उदाहरण प्रारंभ करता है [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) वर्ग का। |
| [AesEncryptionSettings(EncryptionMethod method)](#AesEncryptionSettings-com.aspose.zip.EncryptionMethod-) | नया उदाहरण प्रारंभ करता है [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) वर्ग का बिना पासवर्ड के। |
### AesEncryptionSettings(String password, EncryptionMethod method) {#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-}
```
public AesEncryptionSettings(String password, EncryptionMethod method)
```


नया उदाहरण प्रारंभ करता है [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) वर्ग का।

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Password for encryption or decryption. |
| method | [EncryptionMethod](../../com.aspose.zip/encryptionmethod) | Algorithm option indicating block size of cipher. |

### AesEncryptionSettings(EncryptionMethod method) {#AesEncryptionSettings-com.aspose.zip.EncryptionMethod-}
```
public AesEncryptionSettings(EncryptionMethod method)
```


Initializes a new instance of the [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) class without a password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| method | [EncryptionMethod](../../com.aspose.zip/encryptionmethod) | Algorithm option indicating block size of cipher. |

