---
title: "CancellationFlag"
second_title: "Aspose.ZIP för Java API-referens"
description: "Flaggan som tillåter avbrytning av operationer."
type: docs
weight: 54
url: /sv/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

Flaggan som tillåter avbrytning av operationer.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | Skapar en CancellationFlag-instans. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [cancel()](#cancel--) | Avbryter operationen som är associerad med denna [CancellationFlag](../../com.aspose.zip/cancellationflag)-instans. |
| [cancelAfter(long delay)](#cancelAfter-long-) | Avbryter operationen efter en specificerad fördröjning i millisekunder. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | Avbryter operationen efter en specificerad fördröjning i den angivna tidsenheten. |
| [close()](#close--) | Stänger [CancellationFlag](../../com.aspose.zip/cancellationflag)-instansen och frigör alla resurser som är associerade med den. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


Skapar en CancellationFlag-instans.

### cancel() {#cancel--}
```
public void cancel()
```


Avbryter operationen som är associerad med denna [CancellationFlag](../../com.aspose.zip/cancellationflag)-instans.

Om operationen redan är avbruten gör denna metod inget.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


Avbryter operationen efter en specificerad fördröjning i millisekunder.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| delay | long | Fördröjningen i millisekunder efter vilken operationen kommer att avbrytas. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


Avbryter operationen efter en specificerad fördröjning i den angivna tidsenheten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| delay | long | Fördröjningen efter vilken operationen kommer att avbrytas. |
| enhet | java.util.concurrent.TimeUnit | Tidsenheten för fördröjningsparametern. |

### close() {#close--}
```
public void close()
```


Stänger [CancellationFlag](../../com.aspose.zip/cancellationflag)-instansen och frigör alla resurser som är associerade med den.

