---
title: "SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор SevenZipPPMdCompressionSettings. Создает настройки для метода сжатия PPMd в архиве 7z"
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Создаёт параметры метода сжатия PPMd в 7z‑архиве.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| maxOrder | Byte | Максимальный порядок. |
| suballocatorSize | Int32 | Размер памяти в МБ, который может потреблять субаллокация. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* не находится в диапазоне от 2 до 32, или *suballocatorSize* не находится в диапазоне от 1 до 1024. |

## Примечания

Более высокие порядки модели почти наверняка приводят к лучшему сжатию и, безусловно, к большему использованию памяти и процессора.

Алгоритм PPMd может требовать много памяти, особенно при работе с большими файлами и/или при использовании большого порядка модели. Если ppmd потребует больше памяти, чем вы предоставляете, сжатие будет хуже.

## Примеры

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### См. также

* class [SevenZipPPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Создаёт параметры метода сжатия PPMd в 7z‑архиве с порядком модели по умолчанию и размером субаллокации.

```csharp
public SevenZipPPMdCompressionSettings()
```

## Примечания

Порядок модели по умолчанию равен 6, а размер субаллокации — 16 МБ.

## Примеры

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### См. также

* class [SevenZipPPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)


