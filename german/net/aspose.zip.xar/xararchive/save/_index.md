---
title: "XarArchive.Save"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "XarArchive-Methode. Speichert das Archiv in der angegebenen Zieldatei."
type: docs
weight: 80
url: /de/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

Speichert das Archiv in die angegebene Zieldatei.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| saveOptions | XarSaveOptions | Optionen zum Speichern des xar-Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *destinationFileName* ist null. |
| InvalidOperationException | Es ist nicht möglich, das xar-Archiv zu ändern. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| IOException | Beim Öffnen der Datei ist ein I/O-Fehler aufgetreten. |
| PathTooLongException | Der angegebene Pfad, Dateiname oder beides überschreitet die systemdefinierte maximale Länge. |
| UnauthorizedAccessException | *destinationFileName* gibt eine schreibgeschützte Datei an. -oder- *destinationFileName* gibt ein Verzeichnis an. -oder- Der Aufrufer hat nicht die erforderliche Berechtigung. |

### Siehe auch

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

Speichert das Archiv in den bereitgestellten Stream.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ausgabe | Stream | Ziel-Stream. |
| saveOptions | XarSaveOptions | Optionen zum Speichern des xar-Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *output* ist null. |
| ArgumentException | *output* ist nicht schreib-/lesbar oder nicht suchbar. |
| InvalidOperationException | Es ist nicht möglich, das xar-Archiv zu ändern. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

### Siehe auch

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


