---
title: ArchiveLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which archive is loaded from a compressed file.
type: docs
weight: 19
url: /java/com.aspose.zip/archiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveLoadOptions
```

Options with which archive is loaded from a compressed file.
## Constructors

| Constructor | Description |
| --- | --- |
| [ArchiveLoadOptions()](#ArchiveLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Gets the password to decrypt entries. |
| [getEncoding()](#getEncoding--) | Gets the encoding for entries' names. |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Gets an event that is raised when some bytes have been extracted. |
| [getEntryListed()](#getEntryListed--) | Gets an event that is raised when an entry listed within table of content. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Gets a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel the extraction operation. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Sets the password to decrypt entries. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Sets the encoding for entries' names. |
| [setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Sets an event that is raised when some bytes have been extracted. |
| [setEntryListed(Event&lt;EntryEventArgs&gt; value)](#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Sets an event that is raised when an entry listed within table of content. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Sets a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored. |
### ArchiveLoadOptions() {#ArchiveLoadOptions--}
```
public ArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Gets the password to decrypt entries.


You can provide decryption password once on archive extraction.

```

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
java.nio.charset.Charset - the encoding for entries' names
### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getEntryExtractionProgressed()
```


Gets an event that is raised when some bytes have been extracted.

Track the progress of an entry extraction.

```

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

Event sender is the [ArchiveEntry](../../com.aspose.zip/archiveentry) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### getEntryListed() {#getEntryListed--}
```
public final Event<EntryEventArgs> getEntryListed()
```


Gets an event that is raised when an entry listed within table of content.

```

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

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Sets the password to decrypt entries.


You can provide decryption password once on archive extraction.

```

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
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.nio.charset.Charset | the encoding for entries' names |

### setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Sets an event that is raised when some bytes have been extracted.

Track the progress of an entry extraction.

```

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

Event sender is the [ArchiveEntry](../../com.aspose.zip/archiveentry) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | an event that is raised when some bytes have been extracted |

### setEntryListed(Event&lt;EntryEventArgs&gt; value) {#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public final void setEntryListed(Event<EntryEventArgs> value)
```


Sets an event that is raised when an entry listed within table of content.

```

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

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public final void setSkipChecksumVerification(boolean value)
```


Sets a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored. Default is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored |

