---
title: "SevenZipLoadOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni con cui  è caricato da un file compresso."
type: docs
weight: 116
url: /it/java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

Opzioni con cui [SevenZipArchive](../../com.aspose.zip/sevenziparchive) viene caricato da un file compresso.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Restituisce la password per decrittare le voci e i nomi delle voci. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Imposta un flag di cancellazione usato per annullare l'operazione di estrazione. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Imposta la password per decrittare le voci e i nomi delle voci. |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Restituisce la password per decrittare le voci e i nomi delle voci.

È possibile fornire la password di decrittazione una sola volta durante l'estrazione dell'archivio.

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

La cancellazione di solito comporta che alcuni dati non vengano estratti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | un flag di cancellazione utilizzato per annullare l'operazione di estrazione. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Imposta la password per decrittare le voci e i nomi delle voci.

È possibile fornire la password di decrittazione una sola volta durante l'estrazione dell'archivio.

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

