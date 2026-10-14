---
title: "SevenZipLoadOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "कम्प्रेस्ड फ़ाइल से  लोड करने के विकल्प।"
type: docs
weight: 116
url: /hi/java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

संकुचित फ़ाइल से [SevenZipArchive](../../com.aspose.zip/sevenziparchive) को लोड करने के विकल्प।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | एंट्रीज़ और एंट्री नामों को डिक्रिप्ट करने के लिए पासवर्ड प्राप्त करता है। |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है। |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | एंट्रीज़ और एंट्री नामों को डिक्रिप्ट करने के लिए पासवर्ड सेट करता है। |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


एंट्रीज़ और एंट्री नामों को डिक्रिप्ट करने के लिए पासवर्ड प्राप्त करता है।

आप आर्काइव निकाले जाने पर एक बार डिक्रिप्शन पासवर्ड प्रदान कर सकते हैं।

```

``````

try (FileInputStream fs = new FileInputStream(\"encrypted_archive.7z\"));
FileOutputStream extracted = new FileOutputStream(\"extracted.bin\")) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("p@s$");
try (SevenZipArchive archive = new SevenZipArchive(fs, options);
InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```



**Returns:**
java.lang.String - the password to decrypt entries and entry names.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel 7Z archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         SevenZipLoadOptions options = new SevenZipLoadOptions();
         options.setCancellationFlag(cf);
         try (SevenZipArchive a = new SevenZipArchive("big.7z", options)) {
             try {
                 a.getEntries().get(0).extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

रद्दीकरण अक्सर कुछ डेटा के निष्कर्षण न होने का परिणाम देता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | एक रद्दीकरण फ़्लैग जो निष्कर्षण ऑपरेशन को रद्द करने के लिए उपयोग किया जाता है। |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


एंट्रीज़ और एंट्री नामों को डिक्रिप्ट करने के लिए पासवर्ड सेट करता है।

आप आर्काइव निकाले जाने पर एक बार डिक्रिप्शन पासवर्ड प्रदान कर सकते हैं।

```

``````

try (FileInputStream fs = new FileInputStream(\"encrypted_archive.7z\"));
FileOutputStream extracted = new FileOutputStream(\"extracted.bin\")) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("p@s$");
try (SevenZipArchive archive = new SevenZipArchive(fs, options);
InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the password to decrypt entries and entry names. |

