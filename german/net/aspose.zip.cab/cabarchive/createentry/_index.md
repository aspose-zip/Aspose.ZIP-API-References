---
title: "CabArchive.CreateEntry"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "CabArchive-Methode. Erstellt einen einzelnen Eintrag im Archiv."
type: docs
weight: 40
url: /de/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

Erstellt einen einzelnen Eintrag im Archiv.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| Pfad | String | Der vollständig qualifizierte Name der neuen Datei oder der relative Dateiname, der komprimiert werden soll. |
| newEntrySettings | CabEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen, die für das hinzugefügte [`CabEntry`](../../cabentry/)‑Element verwendet werden. |

### Rückgabewert

Cab‑Eintrag‑Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| InvalidOperationException | Das Archiv ist für die Extraktion vorbereitet und kann keine Einträge hinzufügen. |

## Hinweise

Der Eintragsname wird ausschließlich über den Parameter *name* festgelegt. Der im Parameter *path* angegebene Dateiname beeinflusst den Eintragsnamen nicht.

## Beispiele

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### Siehe auch

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

Erstellt einen einzelnen Eintrag im Archiv.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| Quelle | Stream | Der Eingabestream für den Eintrag. |
| newEntrySettings | CabEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen, die für das hinzugefügte [`CabEntry`](../../cabentry/)‑Element verwendet werden. |

### Rückgabewert

Cab‑Eintrag‑Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| InvalidOperationException | Das Archiv ist für die Extraktion vorbereitet und kann keine Einträge hinzufügen. |
| ArgumentNullException | *name* ist null. |

## Beispiele

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### Siehe auch

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

Erstellt einen einzelnen Eintrag im Archiv.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| fileInfo | FileInfo | Die Metadaten der zu komprimierenden Datei. |
| newEntrySettings | CabEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen, die für das hinzugefügte [`CabEntry`](../../cabentry/)‑Element verwendet werden. |

### Rückgabewert

CAB‑Eintrag‑Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* ist schreibgeschützt oder ein Verzeichnis. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |
| FileNotFoundException | *fileInfo* stellt eine Datei dar, die nicht gefunden werden kann. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung, auf *fileInfo* zuzugreifen. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| InvalidOperationException | Das Archiv ist für die Extraktion vorbereitet und kann keine Einträge hinzufügen. |
| ArgumentNullException | *name* ist null. |

## Hinweise

Der Eintragsname wird ausschließlich über den Parameter *name* festgelegt. Der im Parameter *fileInfo* angegebene Dateiname beeinflusst den Eintragsnamen nicht.

## Beispiele

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### Siehe auch

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

Erstellt einen einzelnen Eintrag im Archiv.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| streamProvider | Func`1 | Die Methode, die den Eingabestream für den Eintrag bereitstellt. |
| newEntrySettings | CabEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen, die für das hinzugefügte [`CabEntry`](../../cabentry/)‑Element verwendet werden. |

### Rückgabewert

CAB‑Eintrag‑Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Das Archiv wird für die Dekompression instanziiert. - oder - Die maximale Dateianzahl wurde erreicht. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentException | Der *name* ist null oder leer. |

## Beispiele

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### Siehe auch

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


