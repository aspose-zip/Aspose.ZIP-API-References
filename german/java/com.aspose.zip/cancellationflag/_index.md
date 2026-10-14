---
title: "CancellationFlag"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Das Flag, das die Abbruch von Vorgängen ermöglicht."
type: docs
weight: 54
url: /de/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

Das Flag, das die Abbruch von Vorgängen ermöglicht.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | Erstellt eine CancellationFlag-Instanz. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [cancel()](#cancel--) | Bricht die mit dieser [CancellationFlag](../../com.aspose.zip/cancellationflag)-Instanz verbundene Operation ab. |
| [cancelAfter(long delay)](#cancelAfter-long-) | Bricht die Operation nach einer angegebenen Verzögerung in Millisekunden ab. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | Bricht die Operation nach einer angegebenen Verzögerung in der angegebenen Zeiteinheit ab. |
| [close()](#close--) | Schließt die [CancellationFlag](../../com.aspose.zip/cancellationflag)-Instanz und gibt alle damit verbundenen Ressourcen frei. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


Erstellt eine CancellationFlag-Instanz.

### cancel() {#cancel--}
```
public void cancel()
```


Bricht die mit dieser [CancellationFlag](../../com.aspose.zip/cancellationflag)-Instanz verbundene Operation ab.

Wenn die Operation bereits abgebrochen ist, tut diese Methode nichts.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


Bricht die Operation nach einer angegebenen Verzögerung in Millisekunden ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| delay | long | Die Verzögerung in Millisekunden, nach der die Operation abgebrochen wird. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


Bricht die Operation nach einer angegebenen Verzögerung in der angegebenen Zeiteinheit ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| delay | long | Die Verzögerung, nach der die Operation abgebrochen wird. |
| unit | java.util.concurrent.TimeUnit | Die Zeiteinheit des Verzögerungsparameters. |

### close() {#close--}
```
public void close()
```


Schließt die [CancellationFlag](../../com.aspose.zip/cancellationflag)-Instanz und gibt alle damit verbundenen Ressourcen frei.

