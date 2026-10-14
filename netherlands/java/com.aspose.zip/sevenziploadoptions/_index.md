---
title: "SevenZipLoadOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties waarmee  wordt geladen uit een gecomprimeerd bestand."
type: docs
weight: 116
url: /nl/java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

Opties waarmee [SevenZipArchive](../../com.aspose.zip/sevenziparchive) wordt geladen vanuit een gecomprimeerd bestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Haalt het wachtwoord op om items en itemnamen te ontsleutelen. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Stelt het wachtwoord in om items en itemnamen te ontsleutelen. |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Haalt het wachtwoord op om items en itemnamen te ontsleutelen.

U kunt het ontsleutelingswachtwoord één keer opgeven bij het uitpakken van het archief.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.7z");
FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
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

try (FileInputStream fs = new FileInputStream("encrypted_archive.7z");
FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
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

