---
title: CpioArchive.CpioArchive
second_title: Aspose.ZIP für .NET-API-Referenz
description: CpioArchive constructeur. Initialisiert eine neue Instanz vonCpioArchive Klasse.
type: docs
weight: 10
url: /de/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Initialisiert eine neue Instanz von[`CpioArchive`](../) Klasse.

```csharp
public CpioArchive()
```

### Beispiele

Das folgende Beispiel zeigt, wie eine Datei komprimiert wird.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Siehe auch

* class [CpioArchive](../)
* namensraum [Aspose.Zip.Cpio](../../cpioarchive/)
* Montage [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Initialisiert eine neue Instanz von[`CpioArchive`](../) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public CpioArchive(Stream sourceStream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. Es muss auffindbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *sourceStream* ist Null. |
| ArgumentException | *sourceStream* ist nicht auffindbar. |
| InvalidDataException | *sourceStream* ist kein gültiges cpio-Archiv. |

### Bemerkungen

Dieser Konstruktor entpackt keinen Eintrag. Sehen[`Open`](../../cpioentry/open/)Methode zum Entpacken.

### Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Siehe auch

* class [CpioArchive](../)
* namensraum [Aspose.Zip.Cpio](../../cpioarchive/)
* Montage [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Initialisiert eine neue Instanz von[`CpioArchive`](../) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden.

```csharp
public CpioArchive(string path)
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

Dieser Konstruktor entpackt keinen Eintrag. Sehen[`Open`](../../cpioentry/open/)Methode zum Entpacken.

### Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Siehe auch

* class [CpioArchive](../)
* namensraum [Aspose.Zip.Cpio](../../cpioarchive/)
* Montage [Aspose.Zip](../../../)


