---
title: "LzxLoadOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni con cui l'archivio è caricato da un file compresso."
type: docs
weight: 91
url: /it/java/com.aspose.zip/lzxloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzxLoadOptions
```

Opzioni con cui l'archivio è caricato da un file compresso.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LzxLoadOptions()](#LzxLoadOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Imposta un flag di cancellazione usato per annullare l'operazione di estrazione. |
### LzxLoadOptions() {#LzxLoadOptions--}
```
public LzxLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Imposta un flag di cancellazione usato per annullare l'operazione di estrazione.

Annulla l'estrazione dell'archivio ISO dopo un certo periodo di tempo.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LzxLoadOptions options = new LzxLoadOptions();
options.setCancellationFlag(cf);
try (LzxArchive a = new LzxArchive("big.lzx", options)) {
try {
a.getEntries().get(0).extract("data.bin");
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

