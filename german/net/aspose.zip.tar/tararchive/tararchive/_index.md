---
title: TarArchive.TarArchive
second_title: Aspose.ZIP für .NET-API-Referenz
description: TarArchive constructeur. Initialisiert eine neue Instanz vonTarArchive Klasse.
type: docs
weight: 10
url: /de/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Initialisiert eine neue Instanz von[`TarArchive`](../) Klasse.

```csharp
public TarArchive()
```

### Beispiele

Das folgende Beispiel zeigt, wie eine Datei komprimiert wird.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Siehe auch

* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

Initialisiert eine neue Instanz von[`Archive`](../../../aspose.zip/archive/) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public TarArchive(Stream sourceStream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. Es muss auffindbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidDataException | *sourceStream* ist nicht auffindbar. |

### Bemerkungen

Dieser Konstruktor entpackt keinen Eintrag. Sehen[`Open`](../../tarentry/open/)Methode zum Entpacken.

### Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Siehe auch

* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

Initialisiert eine neue Instanz von[`TarArchive`](../) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public TarArchive(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad zur Archivdatei. |

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

Dieser Konstruktor entpackt keinen Eintrag. Sehen[`Open`](../../tarentry/open/)Methode zum Entpacken.

### Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Siehe auch

* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)


