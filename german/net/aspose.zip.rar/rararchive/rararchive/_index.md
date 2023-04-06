---
title: RarArchive.RarArchive
second_title: Aspose.ZIP für .NET-API-Referenz
description: RarArchive constructeur. Initialisiert eine neue Instanz vonRarArchive Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.
type: docs
weight: 10
url: /de/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

Initialisiert eine neue Instanz von[`RarArchive`](../) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der vollständig qualifizierte oder der relative Pfad zur Archivdatei. |
| loadOptions | RarArchiveLoadOptions | Optionen zum Laden bestehender Archive mit. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung. |
| ArgumentException | Der*path* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*path* ist abgelehnt. |
| PathTooLongException | Die angegebene*path*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Bemerkungen

Dieser Konstruktor dekomprimiert keinen Eintrag. Sehen[`Open`](../../rararchiveentry/open/) Methode zum Dekomprimieren.

### Beispiele

Das folgende Beispiel extrahiert ein Archiv und dekomprimiert dann den ersten Eintrag in a`MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Siehe auch

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* namensraum [Aspose.Zip.Rar](../../rararchive/)
* Montage [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

Initialisiert eine neue Instanz von[`RarArchive`](../) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. |
| loadOptions | RarArchiveLoadOptions | Optionen zum Laden bestehender Archive mit. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *sourceStream* ist nicht auffindbar. |
| InvalidDataException | Falsche Signatur für Archiv. - oder - Die Datei ist kein RAR-Archiv. |
| InvalidOperationException |  |

### Bemerkungen

Dieser Konstruktor dekomprimiert keinen Eintrag. Sehen[`Open`](../../rararchiveentry/open/) Methode zum Dekomprimieren.

### Beispiele

Das folgende Beispiel entschlüsselt und dekomprimiert den ersten Eintrag in a`MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Siehe auch

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* namensraum [Aspose.Zip.Rar](../../rararchive/)
* Montage [Aspose.Zip](../../../)


