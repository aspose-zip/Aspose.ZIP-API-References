---
title: "ProgressCancelEventArgs"
second_title: "Aspose.ZIP för Java API-referens"
description: "Klass för avbrytbara händelsedata som innehåller antalet bytes som har behandlats."
type: docs
weight: 95
url: /sv/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

Klass för avbrytbara händelsedata som innehåller antalet bytes som har behandlats.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | Initierar en ny instans av klassen [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCancel()](#getCancel--) | Hämtar ett värde som indikerar om händelsen ska avbrytas. |
| [setCancel(boolean value)](#setCancel-boolean-) | Ställer in ett värde som indikerar om händelsen ska avbrytas. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


Initierar en ny instans av klassen [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| proceededBytes | long | Antalet bytes som har behandlats. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Hämtar ett värde som indikerar om händelsen ska avbrytas.

**Returns:**
boolean - True om händelsen ska avbrytas; annars false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Ställer in ett värde som indikerar om händelsen ska avbrytas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om händelsen ska avbrytas. |

