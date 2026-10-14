---
title: "GzipLoadOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones para cargar ."
type: docs
weight: 70
url: /es/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

Opciones para cargar [GzipArchive](../../com.aspose.zip/gziparchive).

En el .NET Framework 4.0 y superiores, se puede usar para cancelar la extracción.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | Obtiene el valor que indica si se debe analizar el encabezado del flujo para determinar las propiedades, incluido el nombre. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Establece una bandera de cancelación utilizada para cancelar la operación de extracción. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | Establece el valor que indica si se debe analizar el encabezado del flujo para determinar las propiedades, incluido el nombre. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


Obtiene el valor que indica si se debe analizar el encabezado del flujo para determinar las propiedades, incluido el nombre. Tiene sentido solo para flujos con capacidad de búsqueda.

**Returns:**
boolean - el valor que indica si se debe analizar el encabezado del flujo para determinar las propiedades, incluido el nombre.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Establece una bandera de cancelación utilizada para cancelar la operación de extracción.

Cancela la extracción del archivo gzip después de un tiempo determinado.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("La extracción se canceló después de 60 segundos");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

