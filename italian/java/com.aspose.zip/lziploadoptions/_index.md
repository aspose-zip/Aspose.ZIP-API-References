---
title: "LzipLoadOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni per il caricamento ."
type: docs
weight: 85
url: /it/java/com.aspose.zip/lziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzipLoadOptions
```

Opzioni per il caricamento di [LzipArchive](../../com.aspose.zip/lziparchive).

Nel .NET Framework 4.0 e versioni successive, può essere usato per annullare l'estrazione.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LzipLoadOptions()](#LzipLoadOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Imposta un flag di cancellazione usato per annullare l'operazione di estrazione. |
### LzipLoadOptions() {#LzipLoadOptions--}
```
public LzipLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Imposta un flag di cancellazione usato per annullare l'operazione di estrazione.

Annulla l'estrazione dell'archivio lzip dopo un certo periodo di tempo.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LzipLoadOptions options = new LzipLoadOptions();
options.setCancellationFlag(cf);
try (LzipArchive a = new LzipArchive(\"big.lz\", options)) {
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

