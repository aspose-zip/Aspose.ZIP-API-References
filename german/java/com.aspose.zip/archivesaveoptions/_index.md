---
title: "ArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen zum Speichern eines ZIP-Archivs."
type: docs
weight: 36
url: /de/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

Optionen zum Speichern eines ZIP-Archivs.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Liefert optionalen Kommentar für die Zip-Datei. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Liefert einen Wert, der angibt, ob die Quellen der Einträge unmittelbar nach dem Komprimieren eines Eintrags geschlossen werden sollen. |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | Liefert Einstellungen für die Ausgabe des Data Descriptors. |
| [getEncoding()](#getEncoding--) | Liefert die Kodierung zum Konvertieren von Dateinamen und anderen Zeichenketten in Bytes. |
| [getEncryptionOptions()](#getEncryptionOptions--) | Liefert Verschlüsselungseinstellungen zum Speichern eines bestehenden ZIP-Archivs. |
| [getEventsBag()](#getEventsBag--) | Liefert den Container von Ereignissen, die beim Speichern des Archivs ausgelöst werden. |
| [getParallelOptions()](#getParallelOptions--) | Liefert Einstellungen für die parallele Kompression. |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | Liefert Einstellungen für ein selbstextrahierendes Archiv. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Setzt optionalen Kommentar für die Zip-Datei. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Setzt einen Wert, der angibt, ob die Quellen der Einträge unmittelbar nach dem Komprimieren eines Eintrags geschlossen werden sollen. |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | Setzt Einstellungen für die Ausgabe des Data Descriptors. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Setzt die Kodierung zum Konvertieren von Dateinamen und anderen Zeichenketten in Bytes. |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | Setzt Verschlüsselungseinstellungen zum Speichern eines bestehenden ZIP-Archivs. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Setzt den Container von Ereignissen, die beim Speichern des Archivs ausgelöst werden. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | Setzt Einstellungen für die parallele Kompression. |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | Setzt Einstellungen für ein selbstextrahierendes Archiv. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Liefert optionalen Kommentar für die Zip-Datei.

**Returns:**
java.lang.String - optionaler Kommentar für die Zip-Datei.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Liefert einen Wert, der angibt, ob die Quellen der Einträge unmittelbar nach dem Komprimieren eines Eintrags geschlossen werden sollen.

**Returns:**
boolean - ein Wert, der angibt, ob die Quellen der Einträge unmittelbar nach der Komprimierung eines Eintrags geschlossen werden sollen.
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


Liefert Einstellungen für die Ausgabe des Data Descriptors.

Standardoption ist immer ein vorhandener Daten-Deskriptor.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Liefert die Kodierung zum Konvertieren von Dateinamen und anderen Zeichenketten in Bytes.

Falls nicht gesetzt, wird Codepage 437 verwendet.

**Returns:**
java.nio.charset.Charset - Kodierung zum Konvertieren von Dateinamen und anderen Zeichenketten in Bytes.
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


Liefert Verschlüsselungseinstellungen zum Speichern eines bestehenden ZIP-Archivs.

```

``````

try (Archive archive = new Archive("plain.zip")) {
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
archive.save("encripted.zip", options);
}
 
```

Do not use this options for regular composition of encrypted archive, use

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) instead.

Not compatible with `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) having value [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - encryption settings for saving existing ZIP archive.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Gets container of events raising on archive saving.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getParallelOptions() {#getParallelOptions--}
```
public final ParallelOptions getParallelOptions()
```


Gets settings for parallel compression.

Assign it if you want to utilize several CPU cores while compressing several archive entries.

**Returns:**
[ParallelOptions](../../com.aspose.zip/paralleloptions) - settings for parallel compression.
### getSelfExtractorOptions() {#getSelfExtractorOptions--}
```
public final SelfExtractorOptions getSelfExtractorOptions()
```


Gets settings for self extracted archive.

Assign it if you need to compose executable program to extract an archive without any software installed on the target computer.

**Returns:**
[SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) - settings for self extracted archive.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Sets optional comment for the Zip file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | optional comment for the Zip file. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Sets a value indicating whether entries' sources should be closed right after an entry has been compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether entries' sources should be closed right after an entry has been compressed. |

### setDataDescriptorPolicy(ZipDataDescriptorPolicy value) {#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-}
```
public final void setDataDescriptorPolicy(ZipDataDescriptorPolicy value)
```


Sets settings for Data Descriptor emission.

Default option is always present data descriptor.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) | settings for Data Descriptor emission. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets encoding for converting file names and other strings to bytes.

If not set, code page 437 will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.nio.charset.Charset | encoding for converting file names and other strings to bytes. |

### setEncryptionOptions(EncryptionSettings value) {#setEncryptionOptions-com.aspose.zip.EncryptionSettings-}
```
public final void setEncryptionOptions(EncryptionSettings value)
```


Sets encryption settings for saving existing ZIP archive.

```

``````

    try (Archive archive = new Archive("plain.zip")) {
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
        archive.save("encripted.zip", options);
    }
 
```

Verwenden Sie diese Optionen nicht für die reguläre Erstellung eines verschlüsselten Archivs, verwenden Sie

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) stattdessen.

Nicht kompatibel mit `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)), das den Wert [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) hat

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | der Verschlüsselungseinstellungen zum Speichern eines bestehenden ZIP-Archivs. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Setzt den Container von Ereignissen, die beim Speichern des Archivs ausgelöst werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | Container für Ereignisse, die beim Speichern des Archivs ausgelöst werden. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


Setzt Einstellungen für die parallele Kompression.

Weisen Sie es zu, wenn Sie mehrere CPU-Kerne beim Komprimieren mehrerer Archiveinträge nutzen möchten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | Einstellungen für parallele Kompression. |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


Setzt Einstellungen für ein selbstextrahierendes Archiv.

Weisen Sie es zu, wenn Sie ein ausführbares Programm erstellen müssen, um ein Archiv zu extrahieren, ohne dass auf dem Zielcomputer Software installiert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | Einstellungen für selbstextrahierendes Archiv. |

