---
title: RarArchiveLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which  is loaded from a compressed file.
type: docs
weight: 84
url: /java/com.aspose.zip/rararchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class RarArchiveLoadOptions
```

Options with which [RarArchive](../../com.aspose.zip/rararchive) is loaded from a compressed file.
## Constructors

| Constructor | Description |
| --- | --- |
| [RarArchiveLoadOptions()](#RarArchiveLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Gets the password to decrypt entries and entry names. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel the extraction operation. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Sets the password to decrypt entries and entry names. |
### RarArchiveLoadOptions() {#RarArchiveLoadOptions--}
```
public RarArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Gets the password to decrypt entries and entry names.

You can provide decryption password once on archive extraction.

```

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
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel RAR archive extraction after a certain time.

```

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

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Sets the password to decrypt entries and entry names.

You can provide decryption password once on archive extraction.

```

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

