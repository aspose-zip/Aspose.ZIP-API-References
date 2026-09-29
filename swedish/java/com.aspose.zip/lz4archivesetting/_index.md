---
title: "Lz4ArchiveSetting"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för LZ4-arkivkomposition."
type: docs
weight: 81
url: /sv/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

Inställningar för LZ4-arkivkomposition.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | Initierar en ny instans av [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) med standardparametrar. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | Hämtar ett värde som indikerar om den komprimerade xxh32-hashen ska inkluderas i slutet av det komprimerade blocket. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | Hämtar ett värde som indikerar om innehålls-xxh32-hashen ska inkluderas i slutet av LZ4-arkivet. |
| [getIncludeContentSize()](#getIncludeContentSize--) | Hämtar ett värde som indikerar om innehållsstorleken ska inkluderas i ramen. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | Ställer in ett värde som indikerar om den komprimerade xxh32-hashen ska inkluderas i slutet av det komprimerade blocket. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | Ställer in ett värde som indikerar om innehålls-xxh32-hashen ska inkluderas i slutet av LZ4-arkivet. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | Ställer in ett värde som indikerar om innehållsstorleken ska inkluderas i ramen. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


Initierar en ny instans av [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) med standardparametrar.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


Hämtar ett värde som indikerar om den komprimerade xxh32-hashen ska inkluderas i slutet av det komprimerade blocket.

Standard är falskt.

**Returns:**
boolean - ett värde som indikerar om den komprimerade xxh32-hashen ska inkluderas i slutet av det komprimerade blocket.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


Hämtar ett värde som indikerar om innehålls-xxh32-hashen ska inkluderas i slutet av LZ4-arkivet.

Standard är sant.

**Returns:**
boolean - ett värde som indikerar om innehålls-xxh32-hash ska inkluderas i slutet av LZ4-arkivet.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


Hämtar ett värde som indikerar om innehållsstorleken ska inkluderas i ramen.

Standard är falskt. Tillämpas när källströmmen är sökbar.

**Returns:**
boolean - ett värde som indikerar om innehållsstorleken ska inkluderas i ramen.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


Ställer in ett värde som indikerar om den komprimerade xxh32-hashen ska inkluderas i slutet av det komprimerade blocket.

Standard är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om komprimerad xxh32-hash ska inkluderas i slutet av det komprimerade blocket. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


Ställer in ett värde som indikerar om innehålls-xxh32-hashen ska inkluderas i slutet av LZ4-arkivet.

Standard är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om innehålls-xxh32-hash ska inkluderas i slutet av LZ4-arkivet. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


Ställer in ett värde som indikerar om innehållsstorleken ska inkluderas i ramen.

Standard är falskt. Tillämpas när källströmmen är sökbar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om innehållsstorleken ska inkluderas i ramen. |

