---
title: "PPMdCompressionSettings.PPMdCompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор PPMdCompressionSettings. Инициализирует новый экземпляр класса PPMdCompressionSettings"
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

Инициализирует новый экземпляр класса [`PPMdCompressionSettings`](../).

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| modelOrder | Int32 | Порядок модели. |
| suballocatorSize | Int32 | Размер памяти в МБ, который может потреблять субаллокация. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* не находится в диапазоне от 2 до 16. - или - *suballocatorSize* не находится в диапазоне от 1 до 256. |

## Примечания

Более высокие порядки модели почти наверняка приводят к лучшему сжатию и, безусловно, к большему использованию памяти и процессора.

Алгоритм PPMd может требовать много памяти, особенно при работе с большими файлами и/или при использовании большого порядка модели. Если ppmd потребует больше памяти, чем вы предоставляете, сжатие будет хуже.

## Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### См. также

* class [PPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

Инициализирует новый экземпляр класса [`PPMdCompressionSettings`](../) с порядком модели по умолчанию и размером субаллокации.

```csharp
public PPMdCompressionSettings()
```

## Примечания

Порядок модели по умолчанию равен 8, а размер субаллокации — 50 МБ.

## Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### См. также

* class [PPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)


