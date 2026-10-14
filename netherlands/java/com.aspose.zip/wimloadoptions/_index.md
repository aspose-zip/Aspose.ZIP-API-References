---
title: "WimLoadOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties waarmee een archief wordt geladen vanuit een gecomprimeerd bestand."
type: docs
weight: 135
url: /nl/java/com.aspose.zip/wimloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class WimLoadOptions
```

Opties waarmee een archief wordt geladen vanuit een gecomprimeerd bestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [WimLoadOptions()](#WimLoadOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren. |
### WimLoadOptions() {#WimLoadOptions--}
```
public WimLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren.

Annuleer het uitpakken van een WIM-archief na een bepaalde tijd.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
WimLoadOptions options = new WimLoadOptions();
options.setCancellationFlag(cf);
try (WimArchive a = new WimArchive(\"big.wim\", options)) {
try {
StreamSupport.stream(a.getImages().get(0).getAllEntries().spliterator(), false)
.filter(entry -> entry instanceof WimFileEntry)
.map(entry -> (WimFileEntry) entry)
.findFirst().ifPresent(entry -> entry.extract(\"data.bin\"));
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

