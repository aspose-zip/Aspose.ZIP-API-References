---
title: "CancellationFlag"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "De vlag die het annuleren van bewerkingen mogelijk maakt."
type: docs
weight: 54
url: /nl/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

De vlag die het annuleren van bewerkingen mogelijk maakt.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | Construeert een CancellationFlag‑instantie. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [cancel()](#cancel--) | Annuleert de bewerking die aan deze [CancellationFlag](../../com.aspose.zip/cancellationflag)‑instantie is gekoppeld. |
| [cancelAfter(long delay)](#cancelAfter-long-) | Annuleert de bewerking na een opgegeven vertraging in milliseconden. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | Annuleert de bewerking na een opgegeven vertraging in de opgegeven tijdseenheid. |
| [close()](#close--) | Sluit de [CancellationFlag](../../com.aspose.zip/cancellationflag)‑instantie en geeft alle eraan gekoppelde bronnen vrij. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


Construeert een CancellationFlag‑instantie.

### cancel() {#cancel--}
```
public void cancel()
```


Annuleert de bewerking die aan deze [CancellationFlag](../../com.aspose.zip/cancellationflag)‑instantie is gekoppeld.

Als de bewerking al geannuleerd is, doet deze methode niets.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


Annuleert de bewerking na een opgegeven vertraging in milliseconden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| delay | long | De vertraging in milliseconden waarna de bewerking wordt geannuleerd. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


Annuleert de bewerking na een opgegeven vertraging in de opgegeven tijdseenheid.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| delay | long | De vertraging waarna de bewerking wordt geannuleerd. |
| unit | java.util.concurrent.TimeUnit | De tijdseenheid van de vertragingparameter. |

### close() {#close--}
```
public void close()
```


Sluit de [CancellationFlag](../../com.aspose.zip/cancellationflag)‑instantie en geeft alle eraan gekoppelde bronnen vrij.

