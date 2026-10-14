---
title: "LhaLoadOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones con las que el archivo se carga desde un archivo comprimido."
type: docs
weight: 78
url: /es/java/com.aspose.zip/lhaloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LhaLoadOptions
```

Opciones con las que el archivo se carga desde un archivo comprimido.

En el .NET Framework 4.0 y superiores, se puede usar para cancelar la extracción.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LhaLoadOptions()](#LhaLoadOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Establece una bandera de cancelación utilizada para cancelar la operación de extracción. |
### LhaLoadOptions() {#LhaLoadOptions--}
```
public LhaLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Establece una bandera de cancelación utilizada para cancelar la operación de extracción.

Cancelar la extracción del archivo LHA después de un tiempo determinado.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LhaLoadOptions options = new LhaLoadOptions();
options.setCancellationFlag(cf);
try (LhaArchive a = new LhaArchive("big.lha", options)) {
try {
a.getEntries().get(0).extract("data.bin");
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

