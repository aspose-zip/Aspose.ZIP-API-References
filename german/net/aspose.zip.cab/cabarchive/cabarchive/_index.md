---
title: CabArchive.CabArchive
second_title: Aspose.ZIP für .NET-API-Referenz
description: CabArchive constructeur. Initialisiert eine neue Instanz vonCabArchive Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.
type: docs
weight: 10
url: /de/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(Stream) {#constructor}

Initialisiert eine neue Instanz von[`CabArchive`](../) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public CabArchive(Stream sourceStream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. Es muss auffindbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *sourceStream* ist Null. |
| ArgumentException | *sourceStream* ist nicht auffindbar. |
| InvalidDataException | *sourceStream* ist kein gültiges cab-Archiv. |

### Bemerkungen

Dieser Konstruktor entpackt keinen Eintrag. Sehen[`Open`](../../cabentry/open/)Methode zum Entpacken.

### Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Siehe auch

* class [CabArchive](../)
* namensraum [Aspose.Zip.Cab](../../cabarchive/)
* Montage [Aspose.Zip](../../../)

---

## CabArchive(string) {#constructor_1}

Initialisiert eine neue Instanz von[`CabArchive`](../) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public CabArchive(string path)
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

Dieser Konstruktor entpackt keinen Eintrag. Sehen[`Open`](../../cabentry/open/)Methode zum Entpacken.

### Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden.

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Siehe auch

* class [CabArchive](../)
* namensraum [Aspose.Zip.Cab](../../cabarchive/)
* Montage [Aspose.Zip](../../../)


