---
title: "LzipLoadOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options de chargement ."
type: docs
weight: 85
url: /fr/java/com.aspose.zip/lziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzipLoadOptions
```

Options de chargement de [LzipArchive](../../com.aspose.zip/lziparchive).

Dans le .NET Framework 4.0 et supérieur, peut être utilisé pour annuler l'extraction.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LzipLoadOptions()](#LzipLoadOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction. |
### LzipLoadOptions() {#LzipLoadOptions--}
```
public LzipLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction.

Annuler l'extraction de l'archive lzip après un certain temps.

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
System.out.println("L'extraction a été annulée après 60 secondes");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

