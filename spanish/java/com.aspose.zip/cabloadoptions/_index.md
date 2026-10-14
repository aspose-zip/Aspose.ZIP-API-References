---
title: "CabLoadOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones con las que el archivo se carga desde un archivo comprimido."
type: docs
weight: 48
url: /es/java/com.aspose.zip/cabloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class CabLoadOptions
```

Opciones con las que el archivo se carga desde un archivo comprimido.

Permite cancelar la extracción para .NET Framework 4.0 y superiores.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CabLoadOptions()](#CabLoadOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Establece una bandera de cancelación utilizada para cancelar la operación de extracción. |
### CabLoadOptions() {#CabLoadOptions--}
```
public CabLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Establece una bandera de cancelación utilizada para cancelar la operación de extracción.

Cancelar la extracción del archivo CAB después de un tiempo determinado.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
CabLoadOptions options = new CabLoadOptions();
options.setCancellationFlag(cf);
try (CabArchive a = new CabArchive("big.cab", options)) {
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

