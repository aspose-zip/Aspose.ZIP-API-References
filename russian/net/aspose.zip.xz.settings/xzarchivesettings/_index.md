---
title: "Класс XzArchiveSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Xz.Settings.XzArchiveSettings. Класс содержит набор параметров конкретного xz-архива"
type: docs
weight: 1520
url: /ru/net/aspose.zip.xz.settings/xzarchivesettings/
---
## XzArchiveSettings class

Класс содержит набор настроек конкретного архива xz.

```csharp
public class XzArchiveSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [XzArchiveSettings](xzarchivesettings/#constructor)() | Инициализирует новый экземпляр класса `XzArchiveSettings`, используя одиночную компрессию LZMA2. |
| [XzArchiveSettings](xzarchivesettings/#constructor_1)(XzFilterSettings[], long, XzCheckType) | Инициализирует новый экземпляр класса `XzArchiveSettings` с пользовательскими параметрами. |

## Свойства

| Имя | Описание |
| --- | --- |
| static [FastestSpeed](../../aspose.zip.xz.settings/xzarchivesettings/fastestspeed/) { get; } | Получает экземпляр класса `XzArchiveSettings` с размером словаря 65536 байт в фильтре LZMA2, размером блока 1 мегабайт и контрольной суммой CRC32. |
| static [FastSpeed](../../aspose.zip.xz.settings/xzarchivesettings/fastspeed/) { get; } | Получает экземпляр класса `XzArchiveSettings` с размером словаря 1 мегабайт в фильтре LZMA2, размером блока 4 мегабайта и контрольной суммой CRC32. |
| static [HighCompression](../../aspose.zip.xz.settings/xzarchivesettings/highcompression/) { get; } | Получает экземпляр класса `XzArchiveSettings` с размером словаря 32 мегабайта в фильтре LZMA2, размером блока 128 мегабайт и контрольной суммой CRC32. |
| static [MaximumCompression](../../aspose.zip.xz.settings/xzarchivesettings/maximumcompression/) { get; } | Получает экземпляр класса `XzArchiveSettings` с размером словаря 64 мегабайта в фильтре LZMA2, размером блока 256 мегабайт и контрольной суммой CRC32. |
| static [Normal](../../aspose.zip.xz.settings/xzarchivesettings/normal/) { get; } | Получает экземпляр класса `XzArchiveSettings` с размером словаря 16 мегабайт в фильтре LZMA2, размером блока 64 мегабайта и контрольной суммой CRC32. |
| [CompressionThreads](../../aspose.zip.xz.settings/xzarchivesettings/compressionthreads/) { get; set; } | Получает или задает количество потоков сжатия. Если значение больше 1, будет использоваться многопоточное сжатие. |

### См. также

* namespace [Aspose.Zip.Xz.Settings](../../aspose.zip.xz.settings/)
* assembly [Aspose.Zip](../../)


