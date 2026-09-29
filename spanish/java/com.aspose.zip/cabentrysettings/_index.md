---
title: "CabEntrySettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración que controla cómo se escribe una entrada CAB."
type: docs
weight: 47
url: /es/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

Configuración que controla cómo se escribe una entrada CAB.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | Inicializa la configuración con un perfil de compresión específico. |
| [CabEntrySettings()](#CabEntrySettings--) | Inicializa la configuración con la compresión MSZip predeterminada. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Obtiene la configuración de compresión aplicada a la entrada. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


Inicializa la configuración con un perfil de compresión específico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | Configuración de compresión a usar. |

Puede ser uno de estos: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


Inicializa la configuración con la compresión MSZip predeterminada.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


Obtiene la configuración de compresión aplicada a la entrada.

Puede ser uno de estos:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
