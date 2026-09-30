---
title: "CpioArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CpioArchive. Сохраняет архив в указанный файл назначения."
type: docs
weight: 80
url: /ru/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *destinationFileName* — строка нулевой длины, содержит только пробелы или содержит один или несколько недопустимых символов, определённых в System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* равно null. |
| PathTooLongException | Указанный *destinationFileName*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| DirectoryNotFoundException | Указанный *destinationFileName* недействителен (например, он находится на не смонтированном диске). |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |
| UnauthorizedAccessException | *destinationFileName*Указан файл только для чтения и доступ не является чтением.-или- путь указывает на каталог.-или- вызывающий процесс не имеет необходимых прав. |
| NotSupportedException | *destinationFileName* имеет недопустимый формат. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

Можно сохранить архив в тот же путь, из которого он был загружен. Однако это не рекомендуется, потому что такой подход использует копирование во временный файл.

## Примеры

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### См. также

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Сохраняет архив в предоставленный поток.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* равен null. |
| ArgumentException | *output* не доступен для записи. - или - *output* является тем же потоком, из которого мы извлекаем. - ИЛИ - Невозможно сохранить архив в *cpioFormat* из‑за ограничений формата. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

*output* must be writable.

## Примеры

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### См. также

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


