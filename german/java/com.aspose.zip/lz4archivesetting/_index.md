---
title: "Lz4ArchiveSetting"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für die Zusammensetzung von LZ4-Archiven."
type: docs
weight: 81
url: /de/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

Einstellungen für die Zusammensetzung von LZ4-Archiven.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | Initialisiert eine neue Instanz von [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) mit Standardparametern. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | Gibt einen Wert zurück, der angibt, ob der komprimierte xxh32-Hash am Ende des komprimierten Blocks eingefügt werden soll. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | Gibt einen Wert zurück, der angibt, ob der Inhalts-xxh32-Hash am Ende des LZ4-Archivs eingefügt werden soll. |
| [getIncludeContentSize()](#getIncludeContentSize--) | Gibt einen Wert zurück, der angibt, ob die Inhaltsgröße im Frame enthalten sein soll. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | Setzt einen Wert, der angibt, ob der komprimierte xxh32-Hash am Ende des komprimierten Blocks eingefügt werden soll. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | Setzt einen Wert, der angibt, ob der Inhalts-xxh32-Hash am Ende des LZ4-Archivs eingefügt werden soll. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | Setzt einen Wert, der angibt, ob die Inhaltsgröße im Frame enthalten sein soll. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


Initialisiert eine neue Instanz von [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) mit Standardparametern.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


Gibt einen Wert zurück, der angibt, ob der komprimierte xxh32-Hash am Ende des komprimierten Blocks eingefügt werden soll.

Standard ist false.

**Returns:**
boolean – ein Wert, der angibt, ob der komprimierte xxh32-Hash am Ende des komprimierten Blocks eingefügt werden soll.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


Gibt einen Wert zurück, der angibt, ob der Inhalts-xxh32-Hash am Ende des LZ4-Archivs eingefügt werden soll.

Standard ist true.

**Returns:**
boolean - ein Wert, der angibt, ob der Inhalt-xxh32-Hash am Ende des LZ4-Archivs enthalten sein soll.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


Gibt einen Wert zurück, der angibt, ob die Inhaltsgröße im Frame enthalten sein soll.

Standard ist false. Wird angewendet, wenn der Quell-Stream suchbar ist.

**Returns:**
boolean - ein Wert, der angibt, ob die Inhaltsgröße im Frame enthalten sein soll.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


Setzt einen Wert, der angibt, ob der komprimierte xxh32-Hash am Ende des komprimierten Blocks eingefügt werden soll.

Standard ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob der komprimierte xxh32-Hash am Ende des komprimierten Blocks enthalten sein soll. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


Setzt einen Wert, der angibt, ob der Inhalts-xxh32-Hash am Ende des LZ4-Archivs eingefügt werden soll.

Standard ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob der Inhalt-xxh32-Hash am Ende des LZ4-Archivs enthalten sein soll. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


Setzt einen Wert, der angibt, ob die Inhaltsgröße im Frame enthalten sein soll.

Standard ist false. Wird angewendet, wenn der Quell-Stream suchbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob die Inhaltsgröße im Frame enthalten sein soll. |

