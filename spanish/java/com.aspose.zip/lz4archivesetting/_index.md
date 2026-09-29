---
title: "Lz4ArchiveSetting"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuraciones para la composición del archivo LZ4."
type: docs
weight: 81
url: /es/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

Configuraciones para la composición del archivo LZ4.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | Inicializa una nueva instancia de [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) con parámetros predeterminados. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | Obtiene un valor que indica si se debe incluir el hash xxh32 comprimido al final del bloque comprimido. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | Obtiene un valor que indica si se debe incluir el hash xxh32 del contenido al final del archivo LZ4. |
| [getIncludeContentSize()](#getIncludeContentSize--) | Obtiene un valor que indica si se debe incluir el tamaño del contenido en el marco. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | Establece un valor que indica si se debe incluir el hash xxh32 comprimido al final del bloque comprimido. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | Establece un valor que indica si se debe incluir el hash xxh32 del contenido al final del archivo LZ4. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | Establece un valor que indica si se debe incluir el tamaño del contenido en el marco. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


Inicializa una nueva instancia de [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) con parámetros predeterminados.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


Obtiene un valor que indica si se debe incluir el hash xxh32 comprimido al final del bloque comprimido.

El valor predeterminado es falso.

**Returns:**
boolean - un valor que indica si se debe incluir el hash xxh32 comprimido al final del bloque comprimido.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


Obtiene un valor que indica si se debe incluir el hash xxh32 del contenido al final del archivo LZ4.

El valor predeterminado es verdadero.

**Returns:**
boolean - un valor que indica si se debe incluir el hash xxh32 del contenido al final del archivo LZ4.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


Obtiene un valor que indica si se debe incluir el tamaño del contenido en el marco.

El valor predeterminado es false. Se aplica cuando el flujo de origen es buscable.

**Returns:**
boolean - un valor que indica si se debe incluir el tamaño del contenido en el marco.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


Establece un valor que indica si se debe incluir el hash xxh32 comprimido al final del bloque comprimido.

El valor predeterminado es falso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe incluir el hash xxh32 comprimido al final del bloque comprimido. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


Establece un valor que indica si se debe incluir el hash xxh32 del contenido al final del archivo LZ4.

El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe incluir el hash xxh32 del contenido al final del archivo LZ4. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


Establece un valor que indica si se debe incluir el tamaño del contenido en el marco.

El valor predeterminado es false. Se aplica cuando el flujo de origen es buscable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe incluir el tamaño del contenido en el marco. |

