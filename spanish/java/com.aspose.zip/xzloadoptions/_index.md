---
title: "XzLoadOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones para cargar ."
type: docs
weight: 152
url: /es/java/com.aspose.zip/xzloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XzLoadOptions
```

Opciones para cargar [XzArchive](../../com.aspose.zip/xzarchive).

En el .NET Framework 4.0 y superiores, se puede usar para cancelar la extracción.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [XzLoadOptions()](#XzLoadOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Establece una bandera de cancelación utilizada para cancelar la operación de extracción. |
### XzLoadOptions() {#XzLoadOptions--}
```
public XzLoadOptions()
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
XzLoadOptions options = new XzLoadOptions();
options.setCancellationFlag(cf);
try (XzArchive a = new XzArchive("big.xz", options)) {
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

