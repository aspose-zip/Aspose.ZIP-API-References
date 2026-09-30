---
title: "SevenZipArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод SevenZipArchive. Сохраняет 7z‑архив в предоставленный поток"
type: docs
weight: 80
url: /ru/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream, SevenZipArchiveSaveOptions) {#save}

Сохраняет архив 7z в предоставленный поток.

```csharp
public void Save(Stream output, SevenZipArchiveSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |
| saveOptions | SevenZipArchiveSaveOptions | Параметры сохранения архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *output* не поддерживает перемотку. |
| ArgumentNullException | *output* равен null. |
| InvalidOperationException | Кодировщик не смог сжать данные. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |

## Примечания

*output* must be seekable.

## Примеры

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### См. также

* class [SevenZipArchiveSaveOptions](../../../aspose.zip.saving/sevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, SevenZipArchiveSaveOptions) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, SevenZipArchiveSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| saveOptions | SevenZipArchiveSaveOptions | Параметры сохранения архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *destinationFileName* равно null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *destinationFileName* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *destinationFileName* запрещён. |
| PathTooLongException | Указанный *destinationFileName*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл в *destinationFileName* содержит двоеточие (:) в середине строки. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| InvalidOperationException | Кодировщик не смог сжать данные. |

## Примечания

Можно сохранить архив в тот же путь, из которого он был загружен. Однако это не рекомендуется, потому что такой подход использует копирование во временный файл.

## Примеры

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### См. также

* class [SevenZipArchiveSaveOptions](../../../aspose.zip.saving/sevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


