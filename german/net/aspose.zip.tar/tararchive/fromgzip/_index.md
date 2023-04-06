---
title: TarArchive.FromGZip
second_title: Aspose.ZIP für .NET-API-Referenz
description: TarArchive methode. Entpackt mitgeliefertes gzipArchiv und setzt es zusammenTarArchive aus extrahierten Daten.
type: docs
weight: 20
url: /de/net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

Entpackt mitgeliefertes gzip-Archiv und setzt es zusammen[`TarArchive`](../) aus extrahierten Daten.

Wichtig: Das gzip-Archiv wird bei dieser Methode vollständig entpackt, sein Inhalt bleibt intern erhalten. Vorsicht vor Speicherverbrauch.

```csharp
public static TarArchive FromGZip(Stream source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Stream | Die Quelle des Archivs. |

### Rückgabewert

Eine Instanz von[`TarArchive`](../)

### Bemerkungen

Der GZip-Extraktionsstrom ist aufgrund des Komprimierungsalgorithmus nicht durchsuchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, daher muss es einen durchsuchbaren Strom unter der Haube betreiben.

### Siehe auch

* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

Entpackt mitgeliefertes gzip-Archiv und setzt es zusammen[`TarArchive`](../) aus extrahierten Daten.

Wichtig: Das gzip-Archiv wird bei dieser Methode vollständig entpackt, sein Inhalt bleibt intern erhalten. Vorsicht vor Speicherverbrauch.

```csharp
public static TarArchive FromGZip(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad zur Archivdatei. |

### Rückgabewert

Eine Instanz von[`TarArchive`](../)

### Bemerkungen

Der GZip-Extraktionsstrom ist aufgrund des Komprimierungsalgorithmus nicht durchsuchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, daher muss es einen durchsuchbaren Strom unter der Haube betreiben.

### Siehe auch

* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)


