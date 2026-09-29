---
title: "RarArchiveLoadOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "कम्प्रेस्ड फ़ाइल से  लोड करने के विकल्प।"
type: docs
weight: 101
url: /hi/java/com.aspose.zip/rararchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class RarArchiveLoadOptions
```

विकल्प जिनके साथ [RarArchive](../../com.aspose.zip/rararchive) को संकुचित फ़ाइल से लोड किया जाता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [RarArchiveLoadOptions()](#RarArchiveLoadOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | एंट्रीज़ और एंट्री नामों को डिक्रिप्ट करने के लिए पासवर्ड प्राप्त करता है। |
| [getDictionaryStorageMode()](#getDictionaryStorageMode--) | RAR डिकम्प्रेशन शब्दकोश के संग्रहण के तरीके को प्राप्त करता है। |
| [getTemporaryDirectory()](#getTemporaryDirectory--) | अस्थायी शब्दकोश फ़ाइलों के लिए उपयोग की जाने वाली निर्देशिका को प्राप्त करता है। |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है। |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | एंट्रीज़ और एंट्री नामों को डिक्रिप्ट करने के लिए पासवर्ड सेट करता है। |
| [setDictionaryStorageMode(RarDictionaryStorageMode value)](#setDictionaryStorageMode-com.aspose.zip.RarDictionaryStorageMode-) | RAR डिकम्प्रेशन शब्दकोश के संग्रहण के तरीके को सेट करता है। |
| [setTemporaryDirectory(String value)](#setTemporaryDirectory-java.lang.String-) | अस्थायी शब्दकोश फ़ाइलों के लिए उपयोग की जाने वाली निर्देशिका को सेट करता है। |
### RarArchiveLoadOptions() {#RarArchiveLoadOptions--}
```
public RarArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


एंट्रीज़ और एंट्री नामों को डिक्रिप्ट करने के लिए पासवर्ड प्राप्त करता है।

आप आर्काइव निकाले जाने पर एक बार डिक्रिप्शन पासवर्ड प्रदान कर सकते हैं।

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.rar")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
}
} catch (IOException ex) {
}
 
```



**Returns:**
java.lang.String - the password to decrypt entries and entry names.
### getDictionaryStorageMode() {#getDictionaryStorageMode--}
```
public final RarDictionaryStorageMode getDictionaryStorageMode()
```


Gets how the RAR decompression dictionary is stored.

**Returns:**
[RarDictionaryStorageMode](../../com.aspose.zip/rardictionarystoragemode) - the dictionary storage mode
### getTemporaryDirectory() {#getTemporaryDirectory--}
```
public final String getTemporaryDirectory()
```


Gets the directory used for temporary dictionary files.

**Returns:**
java.lang.String - the temporary directory; the system temporary directory is used by default
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel RAR archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         RarArchiveLoadOptions options = new RarArchiveLoadOptions();
         options.setCancellationFlag(cf);
         try (RarArchive a = new RarArchive("big.rar", options)) {
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

try (FileInputStream fs = new FileInputStream("encrypted_archive.rar")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the password to decrypt entries and entry names. |

### setDictionaryStorageMode(RarDictionaryStorageMode value) {#setDictionaryStorageMode-com.aspose.zip.RarDictionaryStorageMode-}
```
public final void setDictionaryStorageMode(RarDictionaryStorageMode value)
```


Sets how the RAR decompression dictionary is stored.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RarDictionaryStorageMode](../../com.aspose.zip/rardictionarystoragemode) | the dictionary storage mode |

### setTemporaryDirectory(String value) {#setTemporaryDirectory-java.lang.String-}
```
public final void setTemporaryDirectory(String value)
```


Sets the directory used for temporary dictionary files. A null or empty value selects the system temporary directory.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the temporary directory |

