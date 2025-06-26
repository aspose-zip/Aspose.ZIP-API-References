---
title: SevenZipLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which  is loaded from a compressed file.
type: docs
weight: 90
url: /java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

Options with which [SevenZipArchive](../../com.aspose.zip/sevenziparchive) is loaded from a compressed file.
## Constructors

| Constructor | Description |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Gets the password to decrypt entries and entry names. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel the extraction operation. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Sets the password to decrypt entries and entry names. |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Gets the password to decrypt entries and entry names.

You can provide decryption password once on archive extraction.

```

 using (FileStream fs = File.OpenRead("encrypted_archive.7z"))
 {
     using (var extracted = File.Create("extracted.bin"))
     {
         using (SevenZipArchive archive = new SevenZipArchive(fs, new SevenZipLoadOptions() { DecryptionPassword = "p@s$" }))
         {
             using (var decompressed = archive.Entries[0].Open())
             {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 &lt; (bytesRead = decompressed.Read(b, 0, b.Length)))
                     extracted.Write(b, 0, bytesRead);
             }
         }
     }
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

 using (FileStream fs = File.OpenRead("encrypted_archive.7z"))
 {
     using (var extracted = File.Create("extracted.bin"))
     {
         using (SevenZipArchive archive = new SevenZipArchive(fs, new SevenZipLoadOptions() { DecryptionPassword = "p@s$" }))
         {
             using (var decompressed = archive.Entries[0].Open())
             {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 &lt; (bytesRead = decompressed.Read(b, 0, b.Length)))
                     extracted.Write(b, 0, bytesRead);
             }
         }
     }
 }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the password to decrypt entries and entry names. |

