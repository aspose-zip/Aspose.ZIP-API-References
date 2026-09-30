---
title: "SevenZipArchive.SaveSplit"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод SevenZipArchive. Сохраняет многотомный архив в указанную целевую директорию"
type: docs
weight: 90
url: /ru/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Сохраняет многотомный архив в указанный каталог назначения.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | String | Путь к директории, в которой будут создаваться сегменты архива. |
| параметры | SplitSevenZipArchiveSaveOptions | Параметры сохранения архива, включая имя файла. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *destinationDirectory* равно null. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к директории. |
| ArgumentException | *destinationDirectory* содержит недопустимые символы, такие как \", &gt;, &lt;, или &#x7C;. |
| PathTooLongException | Указанный путь превышает системно определённую максимальную длину. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |

## Примечания

Этот метод собирает несколько (`n`) файлов filename.7z.001, filename.7z.002, ..., filename.7z.(n).

## Примеры

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### См. также

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


