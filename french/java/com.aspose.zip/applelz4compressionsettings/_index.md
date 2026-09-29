---
title: "AppleLz4CompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour la compression LZ4 dans un fichier Apple Archive .aar."
type: docs
weight: 21
url: /fr/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Paramètres pour la compression LZ4 dans un fichier Apple Archive (.aar).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | Initialise une nouvelle instance de la classe [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings). |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | Initialise une nouvelle instance de la classe [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) avec les paramètres par défaut. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Obtient la taille de chaque bloc compressé `pbz4`/`bv41`. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


Initialise une nouvelle instance de la classe [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| blockSize | int | La taille de chaque bloc compressé `pbz4`/`bv41`. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


Initialise une nouvelle instance de la classe [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) avec les paramètres par défaut.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Obtient la taille de chaque bloc compressé `pbz4`/`bv41`.

Valeur : la valeur par défaut est de 4 MiB.

**Returns:**
int - la taille de chaque bloc compressé `pbz4`/`bv41`.
