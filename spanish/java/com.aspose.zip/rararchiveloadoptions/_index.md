---
title: "RarArchiveLoadOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones con las que  se carga desde un archivo comprimido."
type: docs
weight: 101
url: /es/java/com.aspose.zip/rararchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class RarArchiveLoadOptions
```

Opciones con las que se carga [RarArchive](../../com.aspose.zip/rararchive) desde un archivo comprimido.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [RarArchiveLoadOptions()](#RarArchiveLoadOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Obtiene la contraseña para descifrar entradas y nombres de entradas. |
| [getDictionaryStorageMode()](#getDictionaryStorageMode--) | Obtiene cómo se almacena el diccionario de descompresión RAR. |
| [getTemporaryDirectory()](#getTemporaryDirectory--) | Obtiene el directorio utilizado para archivos de diccionario temporales. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Establece una bandera de cancelación utilizada para cancelar la operación de extracción. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Establece la contraseña para descifrar entradas y nombres de entradas. |
| [setDictionaryStorageMode(RarDictionaryStorageMode value)](#setDictionaryStorageMode-com.aspose.zip.RarDictionaryStorageMode-) | Establece cómo se almacena el diccionario de descompresión RAR. |
| [setTemporaryDirectory(String value)](#setTemporaryDirectory-java.lang.String-) | Establece el directorio utilizado para archivos de diccionario temporales. |
### RarArchiveLoadOptions() {#RarArchiveLoadOptions--}
```
public RarArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Obtiene la contraseña para descifrar entradas y nombres de entradas.

Puede proporcionar la contraseña de descifrado una vez al extraer el archivo.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.rar")) {
try (FileOutputStream extracted = new FileOutputStream(\"extracted.bin\")) {
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword(\"p@s$\");
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

try (FileInputStream fs = new FileInputStream("encrypted_archive.rar")) {
try (FileOutputStream extracted = new FileOutputStream(\"extracted.bin\")) {
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword(\"p@s$\");
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

