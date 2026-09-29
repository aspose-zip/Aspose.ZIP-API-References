---
title: "SplitArchiveSaveOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options pour enregistrer une archive ZIP multi-volume."
type: docs
weight: 122
url: /fr/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

Options pour enregistrer une archive ZIP multi-volume.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | Instancie les paramètres pour enregistrer une archive ZIP multi‑volumes. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Obtient le commentaire facultatif pour le fichier Zip. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Obtient une valeur indiquant si les sources des entrées doivent être fermées immédiatement après qu'une entrée a été compressée. |
| [getEncoding()](#getEncoding--) | Obtient l'encodage pour convertir les noms de fichiers et d'autres chaînes en octets. |
| [getEventsBag()](#getEventsBag--) | Obtient le conteneur des événements déclenchés lors de l'enregistrement de l'archive. |
| [getFileName()](#getFileName--) | Obtient le nom des segments sans extension. |
| [getSegmentSize()](#getSegmentSize--) | Obtient la taille du segment. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Définit le commentaire facultatif pour le fichier Zip. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Définit une valeur indiquant si les sources des entrées doivent être fermées immédiatement après qu'une entrée a été compressée. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Définit l'encodage pour convertir les noms de fichiers et d'autres chaînes en octets. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Définit le conteneur des événements déclenchés lors de l'enregistrement de l'archive. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


Instancie les paramètres pour enregistrer une archive ZIP multi‑volumes.

Certains volumes peuvent être inférieurs à `segmentSize`. Dans la plupart des cas, le dernier segment sera plus petit, mais il arrive rarement que les segments réguliers le soient également.

Les noms de fichiers seront les suivants : `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Nom des volumes. Peut être avec ou sans l'extension .zip. |
| segmentSize | long | Taille du volume. |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Obtient le commentaire facultatif pour le fichier Zip.

**Returns:**
java.lang.String - commentaire optionnel pour le fichier Zip.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Obtient une valeur indiquant si les sources des entrées doivent être fermées immédiatement après qu'une entrée a été compressée.

**Returns:**
boolean - une valeur indiquant si les sources des entrées doivent être fermées immédiatement après qu'une entrée a été compressée.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Obtient l'encodage pour convertir les noms de fichiers et d'autres chaînes en octets.

Si elle n'est pas définie, la page de code 437 sera utilisée.

**Returns:**
java.nio.charset.Charset - encodage pour convertir les noms de fichiers et d'autres chaînes en octets.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Obtient le conteneur des événements déclenchés lors de l'enregistrement de l'archive.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Obtient le nom des segments sans extension.

**Returns:**
java.lang.String - le nom des segments sans extension.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Obtient la taille du segment.

**Returns:**
long - la taille du segment.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Définit le commentaire facultatif pour le fichier Zip.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | commentaire optionnel pour le fichier Zip. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Définit une valeur indiquant si les sources des entrées doivent être fermées immédiatement après qu'une entrée a été compressée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les sources des entrées doivent être fermées immédiatement après qu'une entrée a été compressée. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Définit l'encodage pour convertir les noms de fichiers et d'autres chaînes en octets.

Si elle n'est pas définie, la page de code 437 sera utilisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.nio.charset.Charset | encodage pour convertir les noms de fichiers et autres chaînes en octets. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Définit le conteneur des événements déclenchés lors de l'enregistrement de l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | conteneur des événements déclenchés lors de l'enregistrement de l'archive. |

