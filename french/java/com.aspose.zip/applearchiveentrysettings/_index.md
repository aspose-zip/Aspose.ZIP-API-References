---
title: "AppleArchiveEntrySettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres utilisés pour composer des entrées à l'intérieur de ."
type: docs
weight: 18
url: /fr/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

Paramètres utilisés pour composer des entrées à l'intérieur de [AppleArchive](../../com.aspose.zip/applearchive).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | Initialise une nouvelle instance de la classe [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Obtient les paramètres de compression appliqués à la charge utile Apple Archive composée. |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | Obtient une valeur indiquant si les champs de somme de contrôle CRC32 sont inclus pour les entrées de fichiers composées. |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | Définit une valeur indiquant si les champs de somme de contrôle CRC32 sont inclus pour les entrées de fichiers composées. |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


Initialise une nouvelle instance de la classe [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | Paramètres de compression appliqués à la charge utile Apple Archive composée. |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


Obtient les paramètres de compression appliqués à la charge utile Apple Archive composée.

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


Obtient une valeur indiquant si les champs de somme de contrôle CRC32 sont inclus pour les entrées de fichiers composées.

**Returns:**
booléen - une valeur indiquant si les champs de somme de contrôle CRC32 sont inclus pour les entrées de fichiers composées.
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


Définit une valeur indiquant si les champs de somme de contrôle CRC32 sont inclus pour les entrées de fichiers composées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les champs de somme de contrôle CRC32 sont inclus pour les entrées de fichiers composées. |

