---
title: TarArchive.FromLZip
second_title: Aspose.ZIP für .NET-API-Referenz
description: TarArchive methode. Extrahiert das mitgelieferte lzipArchiv und setzt es zusammenTarArchive aus extrahierten Daten.
type: docs
weight: 30
url: /de/net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

Extrahiert das mitgelieferte lzip-Archiv und setzt es zusammen[`TarArchive`](../) aus extrahierten Daten.

Wichtig: Das lzip-Archiv wird bei dieser Methode vollständig entpackt, sein Inhalt bleibt intern erhalten. Vorsicht vor Speicherverbrauch.

```csharp
public static TarArchive FromLZip(Stream source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Stream | Die Quelle des Archivs. |

### Rückgabewert

Eine Instanz von[`TarArchive`](../)

### Bemerkungen

Der Lzip-Extraktionsstrom ist aufgrund der Art des Komprimierungsalgorithmus nicht durchsuchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Aufzeichnungen zu extrahieren, daher muss es einen durchsuchbaren Stream unter der Haube betreiben.

### Siehe auch

* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

Extrahiert das mitgelieferte lzip-Archiv und setzt es zusammen[`TarArchive`](../) aus extrahierten Daten.

Wichtig: Das lzip-Archiv wird bei dieser Methode vollständig entpackt, sein Inhalt bleibt intern erhalten. Vorsicht vor Speicherverbrauch.

```csharp
public static TarArchive FromLZip(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad zur Archivdatei. |

### Rückgabewert

Eine Instanz von[`TarArchive`](../)

### Bemerkungen

Der Lzip-Extraktionsstrom ist aufgrund der Art des Komprimierungsalgorithmus nicht durchsuchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Aufzeichnungen zu extrahieren, daher muss es einen durchsuchbaren Stream unter der Haube betreiben.

### Siehe auch

* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)


