---
title: "CancelEntryEventArgsXar"
second_title: "Aspose.ZIP för Java API-referens"
description: "Händelseargument för avbrytbara händelser relaterade till poster."
type: docs
weight: 53
url: /sv/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

Händelseargument för avbrytbara händelser relaterade till poster.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | Initierar en ny instans av klassen [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCancel()](#getCancel--) | Hämtar ett värde som indikerar om händelsen ska avbrytas. |
| [setCancel(boolean value)](#setCancel-boolean-) | Ställer in ett värde som indikerar om händelsen ska avbrytas. |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


Initierar en ny instans av klassen [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | arkivposten som händelsen utlöses för |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Hämtar ett värde som indikerar om händelsen ska avbrytas.

**Returns:**
boolean - true om händelsen ska avbrytas; annars false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Ställer in ett värde som indikerar om händelsen ska avbrytas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | true om händelsen ska avbrytas; annars false |

