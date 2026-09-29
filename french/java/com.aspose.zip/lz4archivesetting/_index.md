---
title: "Lz4ArchiveSetting"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres de composition d'une archive LZ4."
type: docs
weight: 81
url: /fr/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

Paramètres de composition d'une archive LZ4.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | Initialise une nouvelle instance de [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) avec les paramètres par défaut. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | Obtient une valeur indiquant s'il faut inclure le hachage xxh32 compressé à la fin du bloc compressé. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | Obtient une valeur indiquant s'il faut inclure le hachage xxh32 du contenu à la fin de l'archive LZ4. |
| [getIncludeContentSize()](#getIncludeContentSize--) | Obtient une valeur indiquant s'il faut inclure la taille du contenu dans la trame. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | Définit une valeur indiquant s'il faut inclure le hachage xxh32 compressé à la fin du bloc compressé. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | Définit une valeur indiquant s'il faut inclure le hachage xxh32 du contenu à la fin de l'archive LZ4. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | Définit une valeur indiquant s'il faut inclure la taille du contenu dans la trame. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


Initialise une nouvelle instance de [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) avec les paramètres par défaut.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


Obtient une valeur indiquant s'il faut inclure le hachage xxh32 compressé à la fin du bloc compressé.

La valeur par défaut est false.

**Returns:**
booléen - une valeur indiquant s'il faut inclure le hachage xxh32 compressé à la fin du bloc compressé.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


Obtient une valeur indiquant s'il faut inclure le hachage xxh32 du contenu à la fin de l'archive LZ4.

La valeur par défaut est true.

**Returns:**
booléen - une valeur indiquant s'il faut inclure le hachage xxh32 du contenu à la fin de l'archive LZ4.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


Obtient une valeur indiquant s'il faut inclure la taille du contenu dans la trame.

Par défaut, la valeur est false. Appliqué lorsque le flux source est recherchable.

**Returns:**
booléen - une valeur indiquant s'il faut inclure la taille du contenu dans le cadre.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


Définit une valeur indiquant s'il faut inclure le hachage xxh32 compressé à la fin du bloc compressé.

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut inclure le hachage xxh32 compressé à la fin du bloc compressé. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


Définit une valeur indiquant s'il faut inclure le hachage xxh32 du contenu à la fin de l'archive LZ4.

La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut inclure le hachage xxh32 du contenu à la fin de l'archive LZ4. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


Définit une valeur indiquant s'il faut inclure la taille du contenu dans la trame.

Par défaut, la valeur est false. Appliqué lorsque le flux source est recherchable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut inclure la taille du contenu dans le cadre. |

