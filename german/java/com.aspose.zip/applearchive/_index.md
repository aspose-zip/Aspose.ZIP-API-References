---
title: "AppleArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse repräsentiert eine Apple Archive .aar-Datei."
type: docs
weight: 16
url: /de/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

Diese Klasse repräsentiert eine Apple Archive (.aar)-Datei. Verwenden Sie sie, um Apple Archive-Dateien zu erstellen.

Apple und Apple Archive sind Marken von Apple Inc.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) mit den für zusammengesetzte Einträge verwendeten Einstellungen. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) mit den für zusammengesetzte Einträge verwendeten Einstellungen. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [dispose()](#dispose--) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis. |
| [getEntries()](#getEntries--) | Liefert die Einträge, die das Archiv bilden. |
| [getFileEntries()](#getFileEntries--) | Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Liefert die für neu erstellte Einträge verwendeten Einstellungen. |
| [isSolid()](#isSolid--) | Liefert einen Wert, der angibt, ob das Archiv eine Solid-Kompression verwendet. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Speichert das Archiv in den angegebenen Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das Archiv in die angegebene Zieldatei. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) mit den für zusammengesetzte Einträge verwendeten Einstellungen.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) mit den für zusammengesetzte Einträge verwendeten Einstellungen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | Einstellungen, die beim Erstellen eines neuen Apple Archive verwendet werden. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | Die Quelle des Archivs. |

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methoden [extractToDirectory(String)](../../com.aspose.zip/applearchive\\#extractToDirectory-String-) und [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\\#open--) zum Dekomprimieren. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Die Quelle des Archivs. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methoden [extractToDirectory(String)](../../com.aspose.zip/applearchive\\#extractToDirectory-String-) und [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\\#open--) zum Dekomprimieren. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | path | java.lang.String | Der vollqualifizierte oder relative Pfad zur Archivdatei. |

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methoden [extractToDirectory(String)](../../com.aspose.zip/applearchive\\#extractToDirectory-String-) und [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\\#open--) zum Dekomprimieren. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


Initialisiert eine neue Instanz der Klasse [AppleArchive](../../com.aspose.zip/applearchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der vollqualifizierte oder relative Pfad zur Archivdatei. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methoden [extractToDirectory(String)](../../com.aspose.zip/applearchive\\#extractToDirectory-String-) und [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\\#open--) zum Dekomprimieren. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verzeichnis | java.io.File | Verzeichnis zum Komprimieren. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verzeichnis | java.io.File | Verzeichnis zum Komprimieren. |
| includeRootDirectory | boolean | Gibt an, ob das Stammverzeichnis selbst einbezogen werden soll oder nicht. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


Erstellt einen einzelnen Eintrag im Archiv.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Eintrags. |
| fileInfo | java.io.File | Die Metadaten der zu komprimierenden Datei. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


Erstellt einen einzelnen Eintrag im Archiv.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Eintrags. |
| fileInfo | java.io.File | Die Metadaten der zu komprimierenden Datei. |
| openImmediately | boolean | True, wenn die Datei sofort geöffnet wird, andernfalls wird die Datei beim Speichern des Archivs geöffnet. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


Erstellt einen einzelnen Eintrag im Archiv.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Eintrags. |
| source | java.io.InputStream | Der Eingabestream für den Eintrag. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


Erstellt einen einzelnen Eintrag im Archiv.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Eintrags. |
| path | java.lang.String | Der Pfad zur zu komprimierenden Datei. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Erstellt einen einzelnen Eintrag im Archiv.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Eintrags. |
| path | java.lang.String | Der Pfad zur zu komprimierenden Datei. |
| openImmediately | boolean | True, wenn die Datei sofort geöffnet wird, andernfalls wird die Datei beim Speichern des Archivs geöffnet. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Der Pfad zum Verzeichnis, in dem die extrahierten Dateien abgelegt werden sollen. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


Liefert die Einträge, die das Archiv bilden.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - Einträge, die das Archiv bilden.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das Archiv bilden
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Liefert das Archivformat.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


Liefert die für neu erstellte Einträge verwendeten Einstellungen.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


Liefert einen Wert, der angibt, ob das Archiv eine Solid-Kompression verwendet. Im Solid-Modus werden alle Eintragsdaten als ein einziger Strom komprimiert und das Extrahieren einzelner Einträge ist nicht möglich. Verwenden Sie stattdessen [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\\#ExtractToDirectory--).

**Returns:**
boolean - ein Wert, der angibt, ob das Archiv eine Solid-Kompression verwendet.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Speichert das Archiv in den angegebenen Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Ausgabe | java.io.OutputStream | Ziel-Stream. |

`output` muss beschreibbar sein. Einige Kompressionseinstellungen, wie LZ4, erfordern ebenfalls einen suchbaren Stream. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Speichert das Archiv in die angegebene Zieldatei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | java.lang.String | Der Pfad des zu erstellenden Archivs. |

