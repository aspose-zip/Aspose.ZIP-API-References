---
title: "WimLoadOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options avec lesquelles l'archive est chargée à partir d'un fichier compressé."
type: docs
weight: 135
url: /fr/java/com.aspose.zip/wimloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class WimLoadOptions
```

Options avec lesquelles l'archive est chargée à partir d'un fichier compressé.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [WimLoadOptions()](#WimLoadOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction. |
### WimLoadOptions() {#WimLoadOptions--}
```
public WimLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction.

Annuler l'extraction de l'archive WIM après un certain temps.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
WimLoadOptions options = new WimLoadOptions();
options.setCancellationFlag(cf);
try (WimArchive a = new WimArchive("big.wim", options)) {
try {
StreamSupport.stream(a.getImages().get(0).getAllEntries().spliterator(), false)
.filter(entry -> entry instanceof WimFileEntry)
.map(entry -> (WimFileEntry) entry)
.findFirst().ifPresent(entry -> entry.extract("data.bin"));
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

