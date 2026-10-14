---
title: "ArchiveLoadOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "विकल्प जिनके साथ ZIP अभिलेख संकुचित फ़ाइल से लोड किया जाता है।"
type: docs
weight: 35
url: /hi/java/com.aspose.zip/archiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveLoadOptions
```

विकल्प जिनके साथ ZIP अभिलेख संकुचित फ़ाइल से लोड किया जाता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ArchiveLoadOptions()](#ArchiveLoadOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | एंट्रीज़ को डिक्रिप्ट करने के लिए पासवर्ड प्राप्त करता है। |
| [getEncoding()](#getEncoding--) | एंट्रीज़ के नामों के लिए एन्कोडिंग प्राप्त करता है। |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | जब कुछ बाइट्स निकाले गए हों तो उठाए जाने वाले इवेंट को प्राप्त करता है। |
| [getEntryListed()](#getEntryListed--) | जब सामग्री तालिका में सूचीबद्ध कोई एंट्री हो तो उठाए जाने वाले इवेंट को प्राप्त करता है। |
| [getForwardOnly()](#getForwardOnly--) | यह दर्शाने वाले फ़्लैग को प्राप्त करता है कि आर्काइव केवल-रीड स्ट्रीम से निकाला गया है। |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | यह दर्शाने वाले मान को प्राप्त करता है कि ZIP एंट्रीज़ की चेकसम सत्यापन को छोड़ दिया जाए और असंगतियों को अनदेखा किया जाए। |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | निष्कर्षण संचालन को रद्द करने के लिए उपयोग किए जाने वाले रद्दीकरण फ़्लैग को सेट करता है। |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | एंट्रीज़ को डिक्रिप्ट करने के लिए पासवर्ड सेट करता है। |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | एंट्रीज़ के नामों के लिए एन्कोडिंग सेट करता है। |
| [setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | जब कुछ बाइट्स निकाले गए हों तो उठाए जाने वाले इवेंट को सेट करता है। |
| [setEntryListed(Event&lt;EntryEventArgs&gt; value)](#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | जब सामग्री तालिका में सूचीबद्ध कोई एंट्री हो तो उठाए जाने वाले इवेंट को सेट करता है। |
| [setForwardOnly(boolean value)](#setForwardOnly-boolean-) | यह दर्शाने वाले फ़्लैग को सेट करता है कि आर्काइव केवल-रीड स्ट्रीम से निकाला गया है। |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | यह दर्शाने वाले मान को सेट करता है कि ZIP एंट्रीज़ की चेकसम सत्यापन को छोड़ दिया जाए और असंगतियों को अनदेखा किया जाए। |
### ArchiveLoadOptions() {#ArchiveLoadOptions--}
```
public ArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


एंट्रीज़ को डिक्रिप्ट करने के लिए पासवर्ड प्राप्त करता है।


आप आर्काइव निकाले जाने पर एक बार डिक्रिप्शन पासवर्ड प्रदान कर सकते हैं।

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.zip")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
}
} catch (IOException ex) {
}
 
```



**Returns:**
java.lang.String - the password to decrypt entries
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Gets the encoding for entries' names.


Entry name composed using specified encoding regardless of zip file properties.

```

``````

    try (FileInputStream fs = new FileInputStream("archive.zip")) {
        ArchiveLoadOptions options = new ArchiveLoadOptions();
        options.setEncoding(Charset.forName("MS932"));
        try (Archive archive = new Archive(fs, options)) {
            String name = archive.getEntries().get(0).getName();
        }
    } catch (IOException ex) {
    }
 
```



**Returns:**
java.nio.charset.Charset - प्रविष्टियों के नामों के लिए एन्कोडिंग
### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getEntryExtractionProgressed()
```


जब कुछ बाइट्स निकाले गए हों तो उठाए जाने वाले इवेंट को प्राप्त करता है।

एक प्रविष्टि निष्कर्षण की प्रगति को ट्रैक करें।

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
Archive archive = new Archive(\"archive.zip\", options);
 
```

Cancel an entry extraction after a certain time.

```

``````

     long startTime = System.nanoTime();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setEntryExtractionProgressed((s, e) -> {
         if ((System.nanoTime() - startTime) / 1_000_000 > 1000)
             e.setCancel(true);
     });
     try (Archive a = new Archive("big.zip", options)) {
         a.getEntries().get(0).extract("first.bin");
     }
 
```

Event sender वह [ArchiveEntry](../../com.aspose.zip/archiveentry) इंस्टेंस है जिसका निष्कर्षण प्रगति पर है।

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### getEntryListed() {#getEntryListed--}
```
public final Event<EntryEventArgs> getEntryListed()
```


जब सामग्री तालिका में सूचीबद्ध कोई एंट्री हो तो उठाए जाने वाले इवेंट को प्राप्त करता है।

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryListed(new Event<EntryEventArgs>() {
public void invoke(Object sender, EntryEventArgs entryEventArgs) {
System.out.println(entryEventArgs.getEntry().getName());
}
});
Archive archive = new Archive(\"archive.zip\", options);
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when an entry listed within table of content
### getForwardOnly() {#getForwardOnly--}
```
public final boolean getForwardOnly()
```


Gets the flag that indicating that archive is extracted from read-only stream.

**Returns:**
boolean - true, if archive's stream is rean-only, false elsewhere.
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public final boolean getSkipChecksumVerification()
```


Gets a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored. Default is false.

**Returns:**
boolean - a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel ZIP archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         ArchiveLoadOptions options = new ArchiveLoadOptions();
         options.setCancellationFlag(cf);
         try (Archive a = new Archive("big.zip", options)) {
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


एंट्रीज़ को डिक्रिप्ट करने के लिए पासवर्ड सेट करता है।


आप आर्काइव निकाले जाने पर एक बार डिक्रिप्शन पासवर्ड प्रदान कर सकते हैं।

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.zip")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the password to decrypt entries |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets the encoding for entries' names.


Entry name composed using specified encoding regardless of zip file properties.

```

``````

    try (FileInputStream fs = new FileInputStream("archive.zip")) {
        ArchiveLoadOptions options = new ArchiveLoadOptions();
        options.setEncoding(Charset.forName("MS932"));
        try (Archive archive = new Archive(fs, options)) {
            String name = archive.getEntries().get(0).getName();
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.nio.charset.Charset | प्रविष्टियों के नामों के लिए एन्कोडिंग |

### setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


जब कुछ बाइट्स निकाले गए हों तो उठाए जाने वाले इवेंट को सेट करता है।

एक प्रविष्टि निष्कर्षण की प्रगति को ट्रैक करें।

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
Archive archive = new Archive(\"archive.zip\", options);
 
```

Cancel an entry extraction after a certain time.

```

``````

     long startTime = System.nanoTime();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setEntryExtractionProgressed((s, e) -> {
         if ((System.nanoTime() - startTime) / 1_000_000 > 1000)
             e.setCancel(true);
     });
     try (Archive a = new Archive("big.zip", options)) {
         a.getEntries().get(0).extract("first.bin");
     }
 
```

Event sender वह [ArchiveEntry](../../com.aspose.zip/archiveentry) इंस्टेंस है जिसका निष्कर्षण प्रगति पर है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | एक इवेंट जो तब उठाया जाता है जब कुछ बाइट्स निकाले जा चुके होते हैं |

### setEntryListed(Event&lt;EntryEventArgs&gt; value) {#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public final void setEntryListed(Event<EntryEventArgs> value)
```


जब सामग्री तालिका में सूचीबद्ध कोई एंट्री हो तो उठाए जाने वाले इवेंट को सेट करता है।

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryListed(new Event<EntryEventArgs>() {
public void invoke(Object sender, EntryEventArgs entryEventArgs) {
System.out.println(entryEventArgs.getEntry().getName());
}
});
Archive archive = new Archive(\"archive.zip\", options);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | an event that is raised when an entry listed within table of content |

### setForwardOnly(boolean value) {#setForwardOnly-boolean-}
```
public final void setForwardOnly(boolean value)
```


Sets the flag that indicating that archive is extracted from read-only stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | true, if archive's stream is rean-only, false elsewhere. |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public final void setSkipChecksumVerification(boolean value)
```


Sets a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored. Default is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored |

