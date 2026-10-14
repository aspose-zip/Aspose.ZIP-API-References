---
title: "ArchiveLoadOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الخيارات التي يتم من خلالها تحميل أرشيف ZIP من ملف مضغوط."
type: docs
weight: 35
url: /ar/java/com.aspose.zip/archiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveLoadOptions
```

الخيارات التي يتم من خلالها تحميل أرشيف ZIP من ملف مضغوط.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [ArchiveLoadOptions()](#ArchiveLoadOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | يحصل على كلمة المرور لفك تشفير العناصر. |
| [getEncoding()](#getEncoding--) | يحصل على الترميز لأسماء العناصر. |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | يحصل على حدث يتم إطلاقه عندما يتم استخراج بعض البايتات. |
| [getEntryListed()](#getEntryListed--) | يحصل على حدث يتم إطلاقه عندما يتم إدراج عنصر ضمن جدول المحتويات. |
| [getForwardOnly()](#getForwardOnly--) | يحصل على العلامة التي تشير إلى أن الأرشيف مستخرج من تدفق للقراءة فقط. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | يحصل على قيمة تشير إلى ما إذا كان يجب تخطي التحقق من مجموع التحقق للمدخلات ZIP وتجاهل عدم التطابق. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | يضبط كلمة المرور لفك تشفير العناصر. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | يضبط الترميز لأسماء العناصر. |
| [setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | يضبط حدثًا يتم إطلاقه عندما يتم استخراج بعض البايتات. |
| [setEntryListed(Event&lt;EntryEventArgs&gt; value)](#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | يضبط حدثًا يتم إطلاقه عندما يتم إدراج عنصر ضمن جدول المحتويات. |
| [setForwardOnly(boolean value)](#setForwardOnly-boolean-) | يضبط العلامة التي تشير إلى أن الأرشيف مستخرج من تدفق للقراءة فقط. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تخطي التحقق من مجموع التحقق للمدخلات ZIP وتجاهل عدم التطابق. |
### ArchiveLoadOptions() {#ArchiveLoadOptions--}
```
public ArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


يحصل على كلمة المرور لفك تشفير العناصر.


يمكنك توفير كلمة مرور فك التشفير مرة واحدة عند استخراج الأرشيف.

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
java.nio.charset.Charset - الترميز لأسماء الإدخالات
### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getEntryExtractionProgressed()
```


يحصل على حدث يتم إطلاقه عندما يتم استخراج بعض البايتات.

تتبع تقدم استخراج إدخال.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
Archive archive = new Archive("archive.zip", options);
 
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

Event sender هو الكائن [ArchiveEntry](../../com.aspose.zip/archiveentry) الذي يتم تقدم استخراجّه.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### getEntryListed() {#getEntryListed--}
```
public final Event<EntryEventArgs> getEntryListed()
```


يحصل على حدث يتم إطلاقه عندما يتم إدراج عنصر ضمن جدول المحتويات.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryListed(new Event<EntryEventArgs>() {
public void invoke(Object sender, EntryEventArgs entryEventArgs) {
System.out.println(entryEventArgs.getEntry().getName());
}
});
Archive archive = new Archive("archive.zip", options);
 
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

الإلغاء غالبًا ما يؤدي إلى عدم استخراج بعض البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | علامة إلغاء تُستخدم لإلغاء عملية الاستخراج. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


يضبط كلمة المرور لفك تشفير العناصر.


يمكنك توفير كلمة مرور فك التشفير مرة واحدة عند استخراج الأرشيف.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | java.nio.charset.Charset | الترميز لأسماء الإدخالات |

### setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


يضبط حدثًا يتم إطلاقه عندما يتم استخراج بعض البايتات.

تتبع تقدم استخراج إدخال.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
Archive archive = new Archive("archive.zip", options);
 
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

Event sender هو الكائن [ArchiveEntry](../../com.aspose.zip/archiveentry) الذي يتم تقدم استخراجّه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | حدث يُرفع عندما يتم استخراج بعض البايتات |

### setEntryListed(Event&lt;EntryEventArgs&gt; value) {#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public final void setEntryListed(Event<EntryEventArgs> value)
```


يضبط حدثًا يتم إطلاقه عندما يتم إدراج عنصر ضمن جدول المحتويات.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryListed(new Event<EntryEventArgs>() {
public void invoke(Object sender, EntryEventArgs entryEventArgs) {
System.out.println(entryEventArgs.getEntry().getName());
}
});
Archive archive = new Archive("archive.zip", options);
 
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

