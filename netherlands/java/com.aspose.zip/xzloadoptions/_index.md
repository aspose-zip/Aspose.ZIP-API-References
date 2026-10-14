---
title: "XzLoadOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties voor het laden."
type: docs
weight: 152
url: /nl/java/com.aspose.zip/xzloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XzLoadOptions
```

Opties voor het laden van [XzArchive](../../com.aspose.zip/xzarchive).

In het .NET Framework 4.0 en hoger kan dit worden gebruikt om extractie te annuleren.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [XzLoadOptions()](#XzLoadOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren. |
### XzLoadOptions() {#XzLoadOptions--}
```
public XzLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren.

Annuleer de extractie van het lzip‑archief na een bepaalde tijd.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
XzLoadOptions options = new XzLoadOptions();
options.setCancellationFlag(cf);
try (XzArchive a = new XzArchive("big.xz", options)) {
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

