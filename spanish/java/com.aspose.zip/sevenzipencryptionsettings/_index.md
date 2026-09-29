---
title: "SevenZipEncryptionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Clase base para la configuración de varios métodos de cifrado 7z."
type: docs
weight: 112
url: /es/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

Clase base para la configuración de varios métodos de cifrado 7z.

El AES-256 es el único método de cifrado posible para archivos 7z. Por lo tanto, el [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) es la única implementación.
## Métodos

| Método | Descripción |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | Obtiene un valor que indica el cifrado del encabezado. |
| [getPassword()](#getPassword--) | Obtiene la contraseña para el cifrado o descifrado. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | Establece un valor que indica el cifrado del encabezado. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Establece la contraseña para el cifrado o descifrado. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


Obtiene un valor que indica el cifrado del encabezado.

Esta configuración es equivalente al interruptor `-mhe=on` de la herramienta 7-Zip. Actualmente, es incompatible con la compresión del encabezado.

**Returns:**
boolean - un valor que indica el cifrado del encabezado
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Obtiene la contraseña para el cifrado o descifrado.

**Returns:**
java.lang.String - contraseña para el cifrado o descifrado
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


Establece un valor que indica el cifrado del encabezado.

Esta configuración es equivalente al interruptor `-mhe=on` de la herramienta 7-Zip. Actualmente, es incompatible con la compresión del encabezado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica el cifrado del encabezado |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Establece la contraseña para el cifrado o descifrado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | contraseña para el cifrado o descifrado |

