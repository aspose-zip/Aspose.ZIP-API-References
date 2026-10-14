---
title: "ArjLoadOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options avec lesquelles l'archive est chargée à partir d'un fichier compressé."
type: docs
weight: 39
url: /fr/java/com.aspose.zip/arjloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArjLoadOptions
```

Options avec lesquelles l'archive est chargée à partir d'un fichier compressé.

Dans le .NET Framework 4.0 et supérieur, peut être utilisé pour annuler l'extraction.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ArjLoadOptions()](#ArjLoadOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction. |
### ArjLoadOptions() {#ArjLoadOptions--}
```
public ArjLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction.

Annuler l'extraction de l'archive ARJ après un certain temps.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
ArjLoadOptions options = new ArjLoadOptions();
options.setCancellationFlag(cf);
try (ArjArchive a = new ArjArchive("big.arj", options)) {
try {
a.getEntries().get(0).extract("data.bin");
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

