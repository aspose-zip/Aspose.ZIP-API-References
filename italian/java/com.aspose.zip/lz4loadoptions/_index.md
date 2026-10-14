---
title: "Lz4LoadOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni per il caricamento ."
type: docs
weight: 82
url: /it/java/com.aspose.zip/lz4loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Lz4LoadOptions
```

Opzioni per il caricamento di [Lz4Archive](../../com.aspose.zip/lz4archive).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Lz4LoadOptions()](#Lz4LoadOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Imposta un flag di cancellazione usato per annullare l'operazione di estrazione. |
### Lz4LoadOptions() {#Lz4LoadOptions--}
```
public Lz4LoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Imposta un flag di cancellazione usato per annullare l'operazione di estrazione.

Annulla l'estrazione dell'archivio lz4 dopo un certo periodo di tempo.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
Lz4LoadOptions options = new Lz4LoadOptions();
options.setCancellationFlag(cf);
try (Lz4Archive a = new Lz4Archive("big.lz4", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("L'estrazione è stata annullata dopo 60 secondi");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

