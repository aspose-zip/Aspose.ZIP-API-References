---
title: "AppleArchive.CreateEntry"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "AppleArchive-Methode. Erstellt einen einzelnen Eintrag im Archiv"
type: docs
weight: 60
url: /de/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

Erstellt einen einzelnen Eintrag im Archiv.

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| Pfad | String | Der Pfad zur zu komprimierenden Datei. |
| openImmediately | Boolean | True, wenn die Datei sofort geöffnet werden soll, andernfalls wird die Datei beim Speichern des Archivs geöffnet. |

### Rückgabewert

Apple-Archiv-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben. |
| ArgumentException | *name* ist leer. |
| ArgumentNullException | *path* ist `null`. |

### Siehe auch

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Erstellt einen einzelnen Eintrag im Archiv.

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| Quelle | Stream | Der Eingabestream für den Eintrag. |

### Rückgabewert

Apple-Archiv-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben. |
| ArgumentException | *name* ist leer. |
| ArgumentNullException | *source* ist `null`. |

### Siehe auch

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Erstellt einen einzelnen Eintrag im Archiv.

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| fileInfo | FileInfo | Die Metadaten der zu komprimierenden Datei. |
| openImmediately | Boolean | True, wenn die Datei sofort geöffnet werden soll, andernfalls wird die Datei beim Speichern des Archivs geöffnet. |

### Rückgabewert

Apple-Archiv-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben. |
| ArgumentException | *name* ist leer. |
| ArgumentNullException | *fileInfo* ist `null`. |

### Siehe auch

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


