---
title: "LzipLoadOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones para cargar ."
type: docs
weight: 85
url: /es/java/com.aspose.zip/lziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzipLoadOptions
```

Opciones para cargar [LzipArchive](../../com.aspose.zip/lziparchive).

En el .NET Framework 4.0 y superiores, se puede usar para cancelar la extracción.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LzipLoadOptions()](#LzipLoadOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Establece una bandera de cancelación utilizada para cancelar la operación de extracción. |
### LzipLoadOptions() {#LzipLoadOptions--}
```
public LzipLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Establece una bandera de cancelación utilizada para cancelar la operación de extracción.

Cancelar la extracción del archivo lzip después de un tiempo determinado.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LzipLoadOptions options = new LzipLoadOptions();
options.setCancellationFlag(cf);
try (LzipArchive a = new LzipArchive("big.lz", options)) {
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

