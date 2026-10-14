---
title: "CancelEntryEventArgs"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Evenementargumenten voor annuleerbare, itemgerelateerde gebeurtenissen."
type: docs
weight: 52
url: /nl/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

Evenementargumenten voor annuleerbare, itemgerelateerde gebeurtenissen.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | Initialiseert een nieuw exemplaar van de [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCancel()](#getCancel--) | Haalt een waarde op die aangeeft of het evenement moet worden geannuleerd. |
| [setCancel(boolean value)](#setCancel-boolean-) | Stelt een waarde in die aangeeft of het evenement moet worden geannuleerd. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


Initialiseert een nieuw exemplaar van de [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Archiefitem waarvoor het evenement wordt opgehaald. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Haalt een waarde op die aangeeft of het evenement moet worden geannuleerd.

**Returns:**
boolean - true als het evenement moet worden geannuleerd; anders false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Stelt een waarde in die aangeeft of het evenement moet worden geannuleerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | true als het evenement moet worden geannuleerd; anders false. |

