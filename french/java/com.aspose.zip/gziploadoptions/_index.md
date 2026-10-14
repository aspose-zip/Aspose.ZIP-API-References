---
title: "GzipLoadOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options de chargement ."
type: docs
weight: 70
url: /fr/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

Options de chargement [GzipArchive](../../com.aspose.zip/gziparchive).

Dans le .NET Framework 4.0 et supérieur, peut être utilisé pour annuler l'extraction.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | Obtient la valeur indiquant s'il faut analyser l'en-tête du flux pour déterminer les propriétés, y compris le nom. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | Définit la valeur indiquant s'il faut analyser l'en-tête du flux pour déterminer les propriétés, y compris le nom. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


Obtient la valeur indiquant s'il faut analyser l'en-tête du flux pour déterminer les propriétés, y compris le nom. Cela n'a de sens que pour un flux recherchable.

**Returns:**
booléen - la valeur indiquant s'il faut analyser l'en-tête du flux pour déterminer les propriétés, y compris le nom.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction.

Annuler l'extraction de l'archive gzip après un certain temps.

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

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

