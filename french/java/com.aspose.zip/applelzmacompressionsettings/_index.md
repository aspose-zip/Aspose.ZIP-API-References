---
title: "AppleLzmaCompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour la compression LZMA dans un fichier Apple Archive .aar."
type: docs
weight: 23
url: /fr/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Paramètres pour la compression LZMA dans un fichier Apple Archive (.aar).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | Initialise une nouvelle instance de la classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | Initialise une nouvelle instance de la classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | Initialise une nouvelle instance de la classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | Initialise une nouvelle instance de la classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) avec les paramètres par défaut. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Obtient la taille de chaque bloc de données avant la compression. |
| [getDictionarySize()](#getDictionarySize--) | Obtient la taille du dictionnaire utilisée pour la compression. |
| [getFastBytes()](#getFastBytes--) | Obtient le nombre d'octets rapides utilisés pour la compression. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


Initialise une nouvelle instance de la classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| blockSize | int | La taille de chaque bloc de données avant la compression. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


Initialise une nouvelle instance de la classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| blockSize | int | La taille de chaque bloc de données avant la compression. |
| dictionarySize | int | La taille du dictionnaire utilisée pour la compression. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


Initialise une nouvelle instance de la classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| blockSize | int | La taille de chaque bloc de données avant la compression. |
| dictionarySize | int | La taille du dictionnaire utilisée pour la compression. |
| fastBytes | int | Le nombre d'octets rapides utilisés pour la compression. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


Initialise une nouvelle instance de la classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) avec les paramètres par défaut.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Obtient la taille de chaque bloc de données avant la compression.

Valeur : la valeur par défaut est de 4 MiB.

**Returns:**
int - la taille de chaque bloc de données avant la compression.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Obtient la taille du dictionnaire utilisée pour la compression.

Valeur : la valeur par défaut est de 8 MiB.

**Returns:**
int - la taille du dictionnaire utilisée pour la compression.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Obtient le nombre d'octets rapides utilisés pour la compression.

Valeur : la valeur par défaut est 32.

**Returns:**
int - le nombre d'octets rapides utilisés pour la compression.
