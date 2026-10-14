---
title: "GzipArchive.UncompressedSize"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "GzipArchive-Eigenschaft. Gibt die Größe einer Originaldatei zurück."
type: docs
weight: 30
url: /de/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

Liest die Größe einer Originaldatei.

```csharp
public ulong UncompressedSize { get; }
```

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Hinweise

Während der Dekompression kann diese Eigenschaft eine falsche Größe enthalten. Wenn die Größe der dekomprimierten Datei 4 GB überschreitet, liefert diese Eigenschaft aufgrund der 32‑Bit‑Begrenzung im Header einen falschen Wert.

### Siehe auch

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


