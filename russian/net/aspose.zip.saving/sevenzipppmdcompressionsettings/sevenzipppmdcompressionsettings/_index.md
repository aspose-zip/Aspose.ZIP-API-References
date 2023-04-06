---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP для справочника API .NET
description: SevenZipPPMdCompressionSettings строитель. Задает настройки для метода сжатия PPMd в архиве 7z.
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Задает настройки для метода сжатия PPMd в архиве 7z.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| maxOrder | Byte | Максимальный заказ. |
| suballocatorSize | Int32 | Размер памяти в субраспределителе МБ может потребляться. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* не находится между 2 и 32, или*suballocatorSize* не находится между 1 и 1024. |

### Примечания

Более крупные порядки моделей почти наверняка приводят к лучшему сжатию и, безусловно, к большему использованию памяти и ЦП.

Алгоритму PPMd может потребоваться много памяти, особенно при использовании с большими файлами и/или с большим заказом моделей. Если ppmd требуется больше памяти, чем вы ему даете, сжатие будет хуже.

### Примеры

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Смотрите также

* class [SevenZipPPMdCompressionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* сборка [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Задает настройки для метода сжатия PPMd в архиве 7z с порядком модели по умолчанию и размером вспомогательного распределителя.

```csharp
public SevenZipPPMdCompressionSettings()
```

### Примечания

Порядок моделей по умолчанию — 6, а размер вспомогательного распределителя — 16 МБ.

### Примеры

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Смотрите также

* class [SevenZipPPMdCompressionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* сборка [Aspose.Zip](../../../)


