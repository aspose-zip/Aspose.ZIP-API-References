---
title: "CabLoadOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options avec lesquelles l'archive est chargée à partir d'un fichier compressé."
type: docs
weight: 48
url: /fr/java/com.aspose.zip/cabloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class CabLoadOptions
```

Options avec lesquelles l'archive est chargée à partir d'un fichier compressé.

Permet d'annuler l'extraction pour .NET Framework 4.0 et supérieur.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CabLoadOptions()](#CabLoadOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction. |
### CabLoadOptions() {#CabLoadOptions--}
```
public CabLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction.

Annuler l'extraction de l'archive CAB après un certain temps.

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

