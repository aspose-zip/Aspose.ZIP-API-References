---
title: "Lz4LoadOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties voor het laden."
type: docs
weight: 82
url: /nl/java/com.aspose.zip/lz4loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Lz4LoadOptions
```

Opties voor het laden van [Lz4Archive](../../com.aspose.zip/lz4archive).
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Lz4LoadOptions()](#Lz4LoadOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren. |
### Lz4LoadOptions() {#Lz4LoadOptions--}
```
public Lz4LoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren.

Annuleer lz4-archiefextractie na een bepaalde tijd.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
Lz4LoadOptions options = new Lz4LoadOptions();
options.setCancellationFlag(cf);
try (Lz4Archive a = new Lz4Archive(\"big.lz4\", options)) {
try {
a.extract(\"data.bin\");
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

