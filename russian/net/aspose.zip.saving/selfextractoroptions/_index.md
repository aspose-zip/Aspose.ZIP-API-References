---
title: "Класс SelfExtractorOptions"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Saving.SelfExtractorOptions. Параметры создания самораспаковывающегося исполняемого архива"
type: docs
weight: 1000
url: /ru/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

Параметры создания самораспаковывающегося исполняемого архива.

```csharp
public class SelfExtractorOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | Возвращает или задает значение, указывающее, должно ли окно извлекателя закрываться после распаковки. |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | Возвращает или задает заголовок окна извлекателя. |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | Возвращает или задает программу, которая будет выполнена после завершения извлечения архива. |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | Возвращает или задает путь к значку заголовка для главных окон приложения‑извлекателя. |

## Примеры

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictogram.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### См. также

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


