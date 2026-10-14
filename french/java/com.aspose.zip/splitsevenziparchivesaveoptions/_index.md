---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options pour enregistrer une archive 7-zip multi-volume."
type: docs
weight: 123
url: /fr/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

Options pour enregistrer une archive 7-zip multi-volume.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | Instancie les paramètres pour enregistrer une archive 7z multi‑volume. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getFileName()](#getFileName--) | Obtient le nom des segments sans extension. |
| [getSegmentSize()](#getSegmentSize--) | Obtient la taille du segment. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


Instancie les paramètres pour enregistrer une archive 7z multi‑volume.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | fileName | java.lang.String | nom pour les volumes. Peut être avec ou sans l’extension .7z. |

Les noms de fichiers seront les suivants : `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | taille du volume. |

Certains volumes peuvent être inférieurs à `segmentSize`. Dans la plupart des cas, le dernier segment sera plus petit, mais il arrive rarement que des segments réguliers le soient aussi. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Obtient le nom des segments sans extension.

**Returns:**
java.lang.String - le nom des segments sans extension
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Obtient la taille du segment.

**Returns:**
long - la taille du segment.
