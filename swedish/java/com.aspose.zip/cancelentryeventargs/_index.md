---
title: "CancelEntryEventArgs"
second_title: "Aspose.ZIP för Java API-referens"
description: "Händelseargument för avbrytbara händelser relaterade till poster."
type: docs
weight: 52
url: /sv/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

Händelseargument för avbrytbara händelser relaterade till poster.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | Initierar en ny instans av klassen [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCancel()](#getCancel--) | Hämtar ett värde som indikerar om händelsen ska avbrytas. |
| [setCancel(boolean value)](#setCancel-boolean-) | Ställer in ett värde som indikerar om händelsen ska avbrytas. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


Initierar en ny instans av klassen [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Arkivposten som händelsen utlöses för. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Hämtar ett värde som indikerar om händelsen ska avbrytas.

**Returns:**
boolean - true om händelsen ska avbrytas; annars false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Ställer in ett värde som indikerar om händelsen ska avbrytas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | true om händelsen ska avbrytas; annars false. |

