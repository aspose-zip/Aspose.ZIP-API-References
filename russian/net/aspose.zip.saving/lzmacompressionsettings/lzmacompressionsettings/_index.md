---
title: "LzmaCompressionSettings.LzmaCompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор LzmaCompressionSettings. Инициализирует новый экземпляр класса LzmaCompressionSettings с параметрами по умолчанию."
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings() {#constructor}

Инициализирует новый экземпляр класса [`LzmaCompressionSettings`](../) с параметрами по умолчанию.

```csharp
public LzmaCompressionSettings()
```

## Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### См. также

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## LzmaCompressionSettings(int, int, int) {#constructor_2}

Инициализирует новый экземпляр класса [`LzmaCompressionSettings`](../) с указанным размером словаря, количеством быстрых байтов и количеством битов контекста литералов.

```csharp
public LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dictionarySize | Int32 | Размер словаря (буфера истории) в байтах. Должен быть от 4096 до 1073741824. |
| numberOfFastBytes | Int32 | Количество байтов, используемых для быстрого поиска совпадений в алгоритме LZMA. Может находиться в диапазоне от 5 до 273. |
| literalContextBits | Int32 | Устанавливает количество битов контекста литерала (старшие биты предыдущего литерала). Может принимать значения от 0 до 8. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | Выбрасывается, когда любой из аргументов находится за пределами допустимого диапазона значений. |

### См. также

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## LzmaCompressionSettings(int) {#constructor_1}

Инициализирует новый экземпляр класса [`LzmaCompressionSettings`](../) с указанным размером словаря, количеством быстрых байтов по умолчанию, равным 32, и количеством битов контекста литерала, равным 3.

```csharp
public LzmaCompressionSettings(int dictionarySize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dictionarySize | Int32 | Размер словаря (буфера истории) в байтах. Должен быть от 4096 до 1073741824. |

### См. также

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


