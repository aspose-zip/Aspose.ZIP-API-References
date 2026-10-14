---
title: "SevenZipArchiveEntry.CompressionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Событие SevenZipArchiveEntry. Вызывается, когда часть необработанного потока сжата"
type: docs
weight: 70
url: /ru/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Вызывается, когда часть необработанного потока сжата.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Примечания

Отправитель события — экземпляр [`SevenZipArchiveEntry`](../).

Не вызывается в solid‑режиме и в многопоточном режиме для записей LZMA2.

## Примеры

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### См. также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)


