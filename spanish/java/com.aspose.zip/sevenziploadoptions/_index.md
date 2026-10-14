---
title: "SevenZipLoadOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones con las que  se carga desde un archivo comprimido."
type: docs
weight: 116
url: /es/java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

Opciones con las que se carga [SevenZipArchive](../../com.aspose.zip/sevenziparchive) desde un archivo comprimido.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Obtiene la contraseña para descifrar entradas y nombres de entradas. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Establece una bandera de cancelación utilizada para cancelar la operación de extracción. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Establece la contraseña para descifrar entradas y nombres de entradas. |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Obtiene la contraseña para descifrar entradas y nombres de entradas.

Puede proporcionar la contraseña de descifrado una vez al extraer el archivo.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.7z");
FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword(\"p@s$\");
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

La cancelación generalmente resulta en que algunos datos no se extraigan.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | una bandera de cancelación utilizada para cancelar la operación de extracción. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Establece la contraseña para descifrar entradas y nombres de entradas.

Puede proporcionar la contraseña de descifrado una vez al extraer el archivo.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.7z");
FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword(\"p@s$\");
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

