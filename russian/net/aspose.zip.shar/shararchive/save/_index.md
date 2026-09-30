---
title: "SharArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод SharArchive. Сохраняет архив в указанный файл назначения"
type: docs
weight: 70
url: /ru/net/aspose.zip.shar/shararchive/save/
---
## Save(string) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *destinationFileName* — строка нулевой длины, содержит только пробелы или содержит один или несколько недопустимых символов, определённых в System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* равно null. |
| PathTooLongException | Указанный *destinationFileName*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| DirectoryNotFoundException | Указанный *destinationFileName* недействителен (например, он находится на не смонтированном диске). |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |
| UnauthorizedAccessException | *destinationFileName* указывает файл, который только для чтения, и доступ не является чтением. — или — путь указывает на каталог. — или — вызывающий процесс не имеет необходимых прав. |
| NotSupportedException | *destinationFileName* имеет недопустимый формат. |
| FileNotFoundException | Файл не найден. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Этот архив открыт для извлечения. |

## Примечания

Можно сохранить архив в тот же путь, из которого он был загружен. Однако это не рекомендуется, потому что такой подход использует копирование во временный файл.

## Примеры

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### См. также

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

Сохраняет архив в предоставленный поток.

```csharp
public void Save(Stream output)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* равен null. |
| ArgumentException | *output* недоступен для записи. - или - *output* является тем же потоком, из которого мы извлекаем. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Этот архив открыт для извлечения. |

## Примечания

*output* must be writable.

## Примеры

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### См. также

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


