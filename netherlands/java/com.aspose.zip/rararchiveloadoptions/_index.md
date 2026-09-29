---
title: "RarArchiveLoadOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties waarmee  wordt geladen uit een gecomprimeerd bestand."
type: docs
weight: 101
url: /nl/java/com.aspose.zip/rararchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class RarArchiveLoadOptions
```

Opties waarmee [RarArchive](../../com.aspose.zip/rararchive) wordt geladen vanuit een gecomprimeerd bestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [RarArchiveLoadOptions()](#RarArchiveLoadOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Haalt het wachtwoord op om items en itemnamen te ontsleutelen. |
| [getDictionaryStorageMode()](#getDictionaryStorageMode--) | Haalt op hoe het RAR-decompressiewoordenboek wordt opgeslagen. |
| [getTemporaryDirectory()](#getTemporaryDirectory--) | Haalt de map op die wordt gebruikt voor tijdelijke woordenboekbestanden. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Stelt het wachtwoord in om items en itemnamen te ontsleutelen. |
| [setDictionaryStorageMode(RarDictionaryStorageMode value)](#setDictionaryStorageMode-com.aspose.zip.RarDictionaryStorageMode-) | Stelt in hoe het RAR-decompressiewoordenboek wordt opgeslagen. |
| [setTemporaryDirectory(String value)](#setTemporaryDirectory-java.lang.String-) | Stelt de map in die wordt gebruikt voor tijdelijke woordenboekbestanden. |
### RarArchiveLoadOptions() {#RarArchiveLoadOptions--}
```
public RarArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Haalt het wachtwoord op om items en itemnamen te ontsleutelen.

U kunt het ontsleutelingswachtwoord één keer opgeven bij het uitpakken van het archief.

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

Annulering resulteert meestal in het niet extraheren van sommige gegevens.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | een annuleringsvlag die wordt gebruikt om de extractie‑operatie te annuleren. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Stelt het wachtwoord in om items en itemnamen te ontsleutelen.

U kunt het ontsleutelingswachtwoord één keer opgeven bij het uitpakken van het archief.

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

