---
title: "RarArchiveLoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen, mit denen  aus einer komprimierten Datei geladen wird."
type: docs
weight: 101
url: /de/java/com.aspose.zip/rararchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class RarArchiveLoadOptions
```

Optionen, mit denen [RarArchive](../../com.aspose.zip/rararchive) aus einer komprimierten Datei geladen wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [RarArchiveLoadOptions()](#RarArchiveLoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Liefert das Passwort zum Entschlüsseln von Einträgen und Eintragsnamen. |
| [getDictionaryStorageMode()](#getDictionaryStorageMode--) | Ermittelt, wie das RAR-Dekompressionswörterbuch gespeichert wird. |
| [getTemporaryDirectory()](#getTemporaryDirectory--) | Ermittelt das Verzeichnis, das für temporäre Wörterbuchdateien verwendet wird. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Setzt das Passwort zum Entschlüsseln von Einträgen und Eintragsnamen. |
| [setDictionaryStorageMode(RarDictionaryStorageMode value)](#setDictionaryStorageMode-com.aspose.zip.RarDictionaryStorageMode-) | Legt fest, wie das RAR-Dekompressionswörterbuch gespeichert wird. |
| [setTemporaryDirectory(String value)](#setTemporaryDirectory-java.lang.String-) | Legt das Verzeichnis fest, das für temporäre Wörterbuchdateien verwendet wird. |
### RarArchiveLoadOptions() {#RarArchiveLoadOptions--}
```
public RarArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Liefert das Passwort zum Entschlüsseln von Einträgen und Eintragsnamen.

Sie können das Entschlüsselungspasswort einmalig bei der Archivextraktion angeben.

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

Ein Abbruch führt meistens dazu, dass einige Daten nicht extrahiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | Ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Setzt das Passwort zum Entschlüsseln von Einträgen und Eintragsnamen.

Sie können das Entschlüsselungspasswort einmalig bei der Archivextraktion angeben.

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

