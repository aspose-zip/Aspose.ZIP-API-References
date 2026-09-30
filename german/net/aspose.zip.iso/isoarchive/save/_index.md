---
title: "IsoArchive.Save"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "IsoArchive-Methode. Speichert das ISO-Image am angegebenen Pfad."
type: docs
weight: 70
url: /de/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

Speichert das ISO-Image im angegebenen Pfad.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad, an dem das ISO-Image gespeichert wird. |
| saveOptions | IsoSaveOptions | Optionen zum Speichern des ISO-Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Wird ausgelöst, wenn das Archiv nicht im Bearbeitungsmodus ist. |
| ArgumentNullException | Wird ausgelöst, wenn *path* null ist. |
| DirectoryNotFoundException | Wird ausgelöst, wenn der angegebene Pfad ungültig ist, beispielsweise weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Wird ausgelöst, wenn die Datei bereits geöffnet ist. |
| UnauthorizedAccessException | Wird ausgelöst, wenn der Zugriff auf die Datei *path* verweigert wird. |
| PathTooLongException | Wird ausgelöst, wenn der angegebene *path* die systemdefinierte Maximallänge überschreitet. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

Das folgende Beispiel zeigt, wie man ein ISO-Archiv in einer Datei speichert:

```csharp
// Erstelle ein neues leeres ISO-Archiv
using(IsoArchive isoArchive = new IsoArchive())
{
    // Füge Dateien zum ISO-Archiv hinzu
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Speichere das ISO-Archiv in einer Datei
    isoArchive.Save("new_archive.iso");
}
```

### Siehe auch

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

Speichert das ISO-Image in den angegebenen Stream.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Stream, in dem das ISO-Image gespeichert wird. |
| saveOptions | IsoSaveOptions | Optionen zum Speichern des ISO-Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Wird ausgelöst, wenn das Archiv nicht im Bearbeitungsmodus ist. |
| ArgumentNullException | Wird ausgelöst, wenn *stream* null ist. |
| ArgumentException | Wird ausgelöst, wenn der *stream* nicht beschreibbar ist. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| IOException | Ein I/O-Fehler ist aufgetreten. |

## Beispiele

Das folgende Beispiel zeigt, wie ein ISO-Archiv in einen Speicher-Stream gespeichert wird:

```csharp

 // Erstelle ein neues leeres ISO-Archiv
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // Füge Dateien zum ISO-Archiv hinzu
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // Speichere das ISO-Archiv in einen Speicher-Stream
     isoArchive.Save(memoryStream);
 }
```

### Siehe auch

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


