---
title: "ArjLoadOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties waarmee een archief wordt geladen vanuit een gecomprimeerd bestand."
type: docs
weight: 39
url: /nl/java/com.aspose.zip/arjloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArjLoadOptions
```

Opties waarmee een archief wordt geladen vanuit een gecomprimeerd bestand.

In het .NET Framework 4.0 en hoger kan dit worden gebruikt om extractie te annuleren.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ArjLoadOptions()](#ArjLoadOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren. |
### ArjLoadOptions() {#ArjLoadOptions--}
```
public ArjLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren.

Annuleer het uitpakken van een ARJ-archief na een bepaalde tijd.

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

