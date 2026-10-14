---
title: "TraditionalEncryptionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ZIP संग्रह के भीतर पारंपरिक ZipCrypto एल्गोरिदम के लिए सेटिंग्स।"
type: docs
weight: 127
url: /hi/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

ZIP संग्रह के भीतर पारंपरिक ZipCrypto एल्गोरिदम के लिए सेटिंग्स।

देखें अनुभाग 6.0 ZIP फ़ॉर्मेट विवरण में: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | एक नया उदाहरण प्रारंभ करता है [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) क्लास का। |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | उपयोगकर्ता द्वारा परिभाषित एन्कोडिंग के साथ [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) क्लास का एक नया उदाहरण प्रारंभ करता है। |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | पासवर्ड के बिना [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) क्लास का एक नया उदाहरण प्रारंभ करता है। |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


एक नया उदाहरण प्रारंभ करता है [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) क्लास का।

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$")))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Password for encryption. |

### TraditionalEncryptionSettings(String password, Charset encoding) {#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-}
```
public TraditionalEncryptionSettings(String password, Charset encoding)
```


Initializes a new instance of the [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) class with user defined encoding.

```

``````

    try (Archive archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", StandardCharsets.US_ASCII)))) {
        archive.createEntry("data.bin", "data.bin");
        archive.save(zipFile);
    }
 
```

इस कंस्ट्रक्टर का उपयोग करने की सलाह नहीं दी जाती है। एन्कोडिंग सेट करना मानक के विरुद्ध हो सकता है और असंगत आर्काइव उत्पन्न कर सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| पासवर्ड | java.lang.String | एन्क्रिप्शन के लिए पासवर्ड। |
| एन्कोडिंग | java.nio.charset.Charset | पासवर्ड अक्षरों के लिए एन्कोडिंग। |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


पासवर्ड के बिना [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) क्लास का एक नया उदाहरण प्रारंभ करता है।

