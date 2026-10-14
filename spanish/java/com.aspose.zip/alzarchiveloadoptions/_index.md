---
title: "AlzArchiveLoadOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones con las que se carga un archivo ALZ desde un archivo comprimido."
type: docs
weight: 12
url: /es/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

Opciones con las que se carga un archivo ALZ desde un archivo comprimido.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Obtiene la contraseña utilizada para descifrar las entradas. |
| [getEncoding()](#getEncoding--) | Obtiene la codificación utilizada para los nombres de entrada. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Obtiene si se omite la verificación de suma de comprobación de las entradas ALZ. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Establece una bandera de cancelación utilizada para cancelar la extracción. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Establece la contraseña utilizada para descifrar las entradas. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Establece la codificación utilizada para los nombres de entrada. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Establece si se omite la verificación de suma de comprobación de las entradas ALZ. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Obtiene la contraseña utilizada para descifrar las entradas.

**Returns:**
java.lang.String - contraseña utilizada para descifrar las entradas, o `null` cuando no se configura ninguna.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Obtiene la codificación utilizada para los nombres de entrada. El valor predeterminado es la página de códigos coreana de Windows 949 (CP949). Los archivos ALZ históricamente almacenan los nombres de archivo usando la página de códigos ANSI de Windows coreano.

**Returns:**
java.nio.charset.Charset - codificación utilizada para los nombres de entrada
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


Obtiene si se omite la verificación de suma de comprobación de las entradas ALZ. El valor predeterminado es `false`.

**Returns:**
boolean - si se omite la verificación de suma de comprobación
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Establece una bandera de cancelación utilizada para cancelar la extracción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | bandera de cancelación, o `null` para desactivar la cancelación |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Establece la contraseña utilizada para descifrar las entradas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | contraseña utilizada para descifrar las entradas |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Establece la codificación utilizada para los nombres de entrada. Los archivos ALZ históricamente almacenan los nombres de archivo usando la página de códigos ANSI de Windows coreano.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.nio.charset.Charset | codificación utilizada para los nombres de entrada |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


Establece si se omite la verificación de suma de comprobación de las entradas ALZ.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | si se omite la verificación de suma de comprobación |

