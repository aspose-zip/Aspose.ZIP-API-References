---
title: "XarArchive.CreateEntry"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "XarArchive-Methode. Erstellt einen einzelnen Eintrag im Archiv."
type: docs
weight: 40
url: /de/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

Erstellt einen einzelnen Eintrag im Archiv.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| fileInfo | FileInfo | Die Metadaten der zu komprimierenden Datei oder des Ordners. |
| openImmediately | Boolean | True, wenn die Datei sofort geöffnet werden soll, andernfalls wird die Datei beim Speichern des Archivs geöffnet. |
| compressionSettings | XarCompressionSettings | Die Kompressionseinstellungen, die für das hinzugefügte [`XarEntry`](../../xarentry/)-Element verwendet werden. |

### Rückgabewert

Xar-Eintrag-Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *name* ist null. |
| ArgumentException | *name* ist leer. |
| ArgumentNullException | *fileInfo* ist null. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Hinweise

Wenn die Datei sofort mit dem Parameter *openImmediately* geöffnet wird, wird sie blockiert, bis das Archiv freigegeben wird.

## Beispiele

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### Siehe auch

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

Erstellt einen einzelnen Eintrag im Archiv.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| sourcePath | String | Pfad zur zu komprimierenden Datei. |
| openImmediately | Boolean | True, wenn die Datei sofort geöffnet werden soll, andernfalls wird die Datei beim Speichern des Archivs geöffnet. |
| compressionSettings | XarCompressionSettings | Die Kompressionseinstellungen, die für das hinzugefügte [`XarEntry`](../../xarentry/)-Element verwendet werden. |

### Rückgabewert

Xar-Eintrag-Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *sourcePath* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *sourcePath* ist leer, enthält nur Leerzeichen oder enthält ungültige Zeichen. - oder - Der Dateiname, als Teil von *name*, überschreitet 100 Zeichen. |
| UnauthorizedAccessException | Zugriff auf die Datei *sourcePath* wurde verweigert. |
| PathTooLongException | Der angegebene *sourcePath*, Dateiname oder beide überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. - oder - *name* ist für xar zu lang. |
| NotSupportedException | Datei bei *sourcePath* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| InvalidOperationException | Es ist nicht möglich, das xar-Archiv zu ändern. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Hinweise

Der Eintragsname wird ausschließlich über den Parameter *name* festgelegt. Der im Parameter *sourcePath* angegebene Dateiname beeinflusst den Eintragsnamen nicht.

Wenn die Datei sofort mit dem Parameter *openImmediately* geöffnet wird, wird sie blockiert, bis das Archiv freigegeben wird.

## Beispiele

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### Siehe auch

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

Erstellt einen einzelnen Eintrag im Archiv.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| Quelle | Stream | Der Eingabestream für den Eintrag. |
| compressionSettings | XarCompressionSettings | Die Kompressionseinstellungen, die für das hinzugefügte [`XarEntry`](../../xarentry/)-Element verwendet werden. |

### Rückgabewert

Xar-Eintrag-Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *name* ist null. |
| ArgumentNullException | *source* ist null. |
| ArgumentException | *name* ist leer. |
| InvalidOperationException | Es ist nicht möglich, das xar-Archiv zu ändern. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### Siehe auch

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


