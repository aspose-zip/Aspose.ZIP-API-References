---
title: "CabLoadOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties waarmee een archief wordt geladen vanuit een gecomprimeerd bestand."
type: docs
weight: 48
url: /nl/java/com.aspose.zip/cabloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class CabLoadOptions
```

Opties waarmee een archief wordt geladen vanuit een gecomprimeerd bestand.

Staat toe om extractie te annuleren voor .NET Framework 4.0 en hoger.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CabLoadOptions()](#CabLoadOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren. |
### CabLoadOptions() {#CabLoadOptions--}
```
public CabLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren.

Annuleer CAB-archiefextractie na een bepaalde tijd.

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
System.out.println(\"Extractie werd geannuleerd na 60 seconden\");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

