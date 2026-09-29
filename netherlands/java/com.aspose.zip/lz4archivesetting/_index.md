---
title: "Lz4ArchiveSetting"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor de samenstelling van een LZ4-archief."
type: docs
weight: 81
url: /nl/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

Instellingen voor de samenstelling van een LZ4-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | Initialiseert een nieuw exemplaar van de [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) met standaardparameters. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | Haalt een waarde op die aangeeft of de gecomprimeerde xxh32-hash moet worden opgenomen aan het einde van het gecomprimeerde blok. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | Haalt een waarde op die aangeeft of de inhouds-xxh32-hash moet worden opgenomen aan het einde van het LZ4-archief. |
| [getIncludeContentSize()](#getIncludeContentSize--) | Haalt een waarde op die aangeeft of de inhoudsgrootte moet worden opgenomen in het frame. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | Stelt een waarde in die aangeeft of de gecomprimeerde xxh32-hash moet worden opgenomen aan het einde van het gecomprimeerde blok. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | Stelt een waarde in die aangeeft of de inhouds-xxh32-hash moet worden opgenomen aan het einde van het LZ4-archief. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | Stelt een waarde in die aangeeft of de inhoudsgrootte moet worden opgenomen in het frame. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


Initialiseert een nieuw exemplaar van de [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) met standaardparameters.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


Haalt een waarde op die aangeeft of de gecomprimeerde xxh32-hash moet worden opgenomen aan het einde van het gecomprimeerde blok.

Standaard is false.

**Returns:**
boolean - een waarde die aangeeft of de gecomprimeerde xxh32-hash moet worden opgenomen aan het einde van het gecomprimeerde blok.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


Haalt een waarde op die aangeeft of de inhouds-xxh32-hash moet worden opgenomen aan het einde van het LZ4-archief.

Standaard is true.

**Returns:**
boolean - een waarde die aangeeft of de inhouds‑xxh32‑hash aan het einde van het LZ4‑archief moet worden opgenomen.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


Haalt een waarde op die aangeeft of de inhoudsgrootte moet worden opgenomen in het frame.

Standaard is false. Toegepast wanneer de bronstroom doorzoekbaar is.

**Returns:**
boolean - een waarde die aangeeft of de inhoudsgrootte in het frame moet worden opgenomen.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


Stelt een waarde in die aangeeft of de gecomprimeerde xxh32-hash moet worden opgenomen aan het einde van het gecomprimeerde blok.

Standaard is false.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de gecomprimeerde xxh32‑hash aan het einde van het gecomprimeerde blok moet worden opgenomen. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


Stelt een waarde in die aangeeft of de inhouds-xxh32-hash moet worden opgenomen aan het einde van het LZ4-archief.

Standaard is true.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de inhouds‑xxh32‑hash aan het einde van het LZ4‑archief moet worden opgenomen. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


Stelt een waarde in die aangeeft of de inhoudsgrootte moet worden opgenomen in het frame.

Standaard is false. Toegepast wanneer de bronstroom doorzoekbaar is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de inhoudsgrootte in het frame moet worden opgenomen. |

