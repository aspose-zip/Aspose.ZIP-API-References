---
title: "SevenZipAESEncryptionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "7z अभिलेख में AES एन्क्रिप्शन या डिक्रिप्शन एल्गोरिदम के लिए सेटिंग्स।"
type: docs
weight: 103
url: /hi/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

7z अभिलेख में AES एन्क्रिप्शन या डिक्रिप्शन एल्गोरिदम के लिए सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | एक नया उदाहरण प्रारंभ करता है [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) क्लास का। |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | एक नया उदाहरण प्रारंभ करता है [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) क्लास का बाहरी सिफर के साथ। |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


एक नया उदाहरण प्रारंभ करता है [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) क्लास का।

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$")))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | password for encryption or decryption |

### SevenZipAESEncryptionSettings(SevenZipCipher cipher) {#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-}
```
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```


Initializes a new instance of the [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) class with external cipher.

```

``````

    SevenZipCipher cipher = composeMyCipher();
    try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher)))) {
        archive.createEntry("data.bin", "data.bin");
        archive.save("archive.7z");
    }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | कस्टम AES कार्यान्वयन |

