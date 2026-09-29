---
title: "ArchiveSaveOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options pour enregistrer une archive ZIP."
type: docs
weight: 36
url: /fr/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

Options pour enregistrer une archive ZIP.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Obtient le commentaire facultatif pour le fichier Zip. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Obtient une valeur indiquant si les sources des entrées doivent être fermées immédiatement après qu'une entrée a été compressée. |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | Obtient les paramètres pour l'émission de Data Descriptor. |
| [getEncoding()](#getEncoding--) | Obtient l'encodage pour convertir les noms de fichiers et d'autres chaînes en octets. |
| [getEncryptionOptions()](#getEncryptionOptions--) | Obtient les paramètres de chiffrement pour l'enregistrement d'une archive ZIP existante. |
| [getEventsBag()](#getEventsBag--) | Obtient le conteneur des événements déclenchés lors de l'enregistrement de l'archive. |
| [getParallelOptions()](#getParallelOptions--) | Obtient les paramètres pour la compression parallèle. |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | Obtient les paramètres pour l'archive auto-extractible. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Définit le commentaire facultatif pour le fichier Zip. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Définit une valeur indiquant si les sources des entrées doivent être fermées immédiatement après qu'une entrée a été compressée. |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | Définit les paramètres pour l'émission de Data Descriptor. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Définit l'encodage pour convertir les noms de fichiers et d'autres chaînes en octets. |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | Définit les paramètres de chiffrement pour l'enregistrement d'une archive ZIP existante. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Définit le conteneur des événements déclenchés lors de l'enregistrement de l'archive. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | Définit les paramètres pour la compression parallèle. |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | Définit les paramètres pour l'archive auto-extractible. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


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
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


Obtient les paramètres pour l'émission de Data Descriptor.

L'option par défaut est toujours le descripteur de données présent.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Obtient l'encodage pour convertir les noms de fichiers et d'autres chaînes en octets.

Si elle n'est pas définie, la page de code 437 sera utilisée.

**Returns:**
java.nio.charset.Charset - encodage pour convertir les noms de fichiers et d'autres chaînes en octets.
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


Obtient les paramètres de chiffrement pour l'enregistrement d'une archive ZIP existante.

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

N'utilisez pas ces options pour la composition régulière d'une archive chiffrée, utilisez

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) à la place.

Non compatible avec `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) ayant la valeur [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | définit les paramètres de chiffrement pour l'enregistrement d'une archive ZIP existante. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Définit le conteneur des événements déclenchés lors de l'enregistrement de l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | conteneur des événements déclenchés lors de l'enregistrement de l'archive. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


Définit les paramètres pour la compression parallèle.

Attribuez‑le si vous souhaitez exploiter plusieurs cœurs CPU lors de la compression de plusieurs entrées d'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | paramètres pour la compression parallèle. |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


Définit les paramètres pour l'archive auto-extractible.

Attribuez‑le si vous devez créer un programme exécutable pour extraire une archive sans aucun logiciel installé sur l'ordinateur cible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | paramètres pour l'archive auto‑extrait. |

