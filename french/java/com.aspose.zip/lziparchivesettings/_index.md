---
title: "LzipArchiveSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "La classe contient les paramètres d'une archive lzip particulière."
type: docs
weight: 84
url: /fr/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

La classe contient les paramètres d'une archive lzip particulière.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | Initialise une nouvelle instance de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire particulière. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | Initialise une nouvelle instance de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire particulière. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Obtient le nombre de threads de compression. |
| [getDictionarySize()](#getDictionarySize--) | Obtient la taille du dictionnaire utilisé par la compression LZMA. |
| [getFastSpeed()](#getFastSpeed--) | Obtient l'instance de la classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire égale à 1 mégaoctet dans le filtre LZMA. |
| [getFastestSpeed()](#getFastestSpeed--) | Obtient l'instance de la classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire égale à 65536 octets dans le filtre LZMA. |
| [getHighCompression()](#getHighCompression--) | Obtient l'instance de la classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire égale à 32 mégaoctets dans le filtre LZMA. |
| [getMaxMemberSize()](#getMaxMemberSize--) | Obtient la taille maximale d'un membre dans une archive lzip présentée en octets. |
| [getMaximumCompression()](#getMaximumCompression--) | Obtient l'instance de la classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire égale à 64 mégaoctets dans le filtre LZMA. |
| [getNormal()](#getNormal--) | Obtient l'instance de la classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire égale à 16 mégaoctets dans le filtre LZMA. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Définit le nombre de threads de compression. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


Initialise une nouvelle instance de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire particulière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dictionarySize | int | taille du dictionnaire pour la compression LZMA en octets |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


Initialise une nouvelle instance de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire particulière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dictionarySize | int | taille du dictionnaire pour la compression LZMA en octets |
| maxMemberSize | int | Taille maximale d'un membre dans une archive lzip présentée en octets. La valeur par défaut est de 60 Mo. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Obtient le nombre de threads de compression. Si la valeur est supérieure à 1, la compression multithread sera utilisée.

**Returns:**
int - nombre de threads de compression
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Obtient la taille du dictionnaire utilisé par la compression LZMA.

**Returns:**
int - la taille du dictionnaire utilisé par la compression LZMA
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


Obtient l'instance de la classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire égale à 1 mégaoctet dans le filtre LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


Obtient l'instance de la classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire égale à 65536 octets dans le filtre LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


Obtient l'instance de la classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire égale à 32 mégaoctets dans le filtre LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


Obtient la taille maximale d'un membre dans une archive lzip présentée en octets.

**Returns:**
long - la taille maximale d'un membre dans une archive lzip présentée en octets
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


Obtient l'instance de la classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire égale à 64 mégaoctets dans le filtre LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


Obtient l'instance de la classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) avec une taille de dictionnaire égale à 16 mégaoctets dans le filtre LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Définit le nombre de threads de compression. Si la valeur est supérieure à 1, la compression multithread sera utilisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | nombre de threads de compression |

