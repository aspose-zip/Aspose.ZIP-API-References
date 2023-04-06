---
title: XarArchive.XarArchive
second_title: Aspose.ZIP für .NET-API-Referenz
description: XarArchive constructeur. Initialisiert eine neue Instanz vonXarArchive Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.
type: docs
weight: 10
url: /de/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(Stream) {#constructor}

Initialisiert eine neue Instanz von[`XarArchive`](../) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public XarArchive(Stream sourceStream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. Es muss auffindbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *sourceStream* ist Null. |
| ArgumentException | *sourceStream* ist nicht auffindbar. |
| InvalidDataException | *sourceStream* ist kein gültiges xar-Archiv. |

### Bemerkungen

Dieser Konstruktor entpackt keinen Eintrag. Sehen[`Open`](../../xarfileentry/open/)Methode zum Entpacken.

### Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Siehe auch

* class [XarArchive](../)
* namensraum [Aspose.Zip.Xar](../../xararchive/)
* Montage [Aspose.Zip](../../../)

---

## XarArchive(string) {#constructor_1}

Initialisiert eine neue Instanz von[`XarArchive`](../) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public XarArchive(string path)
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

Dieser Konstruktor entpackt keinen Eintrag. Sehen[`Open`](../../xarfileentry/open/)Methode zum Entpacken.

### Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Siehe auch

* class [XarArchive](../)
* namensraum [Aspose.Zip.Xar](../../xararchive/)
* Montage [Aspose.Zip](../../../)


