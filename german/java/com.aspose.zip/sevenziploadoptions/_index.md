---
title: "SevenZipLoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen, mit denen  aus einer komprimierten Datei geladen wird."
type: docs
weight: 116
url: /de/java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

Optionen, mit denen [SevenZipArchive](../../com.aspose.zip/sevenziparchive) aus einer komprimierten Datei geladen wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Liefert das Passwort zum Entschlüsseln von Einträgen und Eintragsnamen. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Setzt das Passwort zum Entschlüsseln von Einträgen und Eintragsnamen. |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Liefert das Passwort zum Entschlüsseln von Einträgen und Eintragsnamen.

Sie können das Entschlüsselungspasswort einmalig bei der Archivextraktion angeben.

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

