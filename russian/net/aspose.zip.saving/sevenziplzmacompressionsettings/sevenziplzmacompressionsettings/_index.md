---
title: "SevenZipLZMACompressionSettings.SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "SevenZipLZMACompressionSettings конструктор. Инициализирует новый экземпляр класса SevenZipLZMACompressionSettings с параметрами по умолчанию"
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/sevenziplzmacompressionsettings/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings() {#constructor}

Инициализирует новый экземпляр класса [`SevenZipLZMACompressionSettings`](../) с параметрами по умолчанию.

```csharp
public SevenZipLZMACompressionSettings()
```

## Примеры

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save("result.7z");
}
```

### См. также

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMACompressionSettings(int, int, int) {#constructor_2}

Инициализирует новый экземпляр класса [`SevenZipLZMACompressionSettings`](../) с указанным размером словаря, количеством быстрых байтов и количеством битов контекста литералов.

```csharp
public SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, 
    int literalContextBits)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dictionarySize | Int32 | Размер словаря (буфера истории) в байтах. Должен быть от 4096 до 1073741824 или равен нулю для автоматического определения на основе размера записи. |
| numberOfFastBytes | Int32 | Количество байтов, используемых для быстрого поиска совпадений в алгоритме LZMA. Может находиться в диапазоне от 5 до 273. |
| literalContextBits | Int32 | Устанавливает количество битов контекста литерала (старшие биты предыдущего литерала). Может принимать значения от 0 до 8. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | Выбрасывается, когда любой из аргументов находится за пределами допустимого диапазона значений. |

### См. также

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMACompressionSettings(int) {#constructor_1}

Инициализирует новый экземпляр класса [`SevenZipLZMACompressionSettings`](../) с указанным размером словаря, количеством быстрых байтов, равным 32, и количеством битов контекста литералов, равным 3.

```csharp
public SevenZipLZMACompressionSettings(int dictionarySize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dictionarySize | Int32 | Размер словаря (буфера истории) в байтах. Должен быть от 4096 до 1073741824 или равен нулю для автоматического определения на основе размера записи. |

### См. также

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


