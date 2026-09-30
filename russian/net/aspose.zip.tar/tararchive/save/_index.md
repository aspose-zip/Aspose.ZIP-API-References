---
title: "TarArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод TarArchive. Сохраняет архив в предоставленный поток"
type: docs
weight: 150
url: /ru/net/aspose.zip.tar/tararchive/save/
---
## Save(Stream, TarFormat?) {#save}

Сохраняет архив в предоставленный поток.

```csharp
public void Save(Stream output, TarFormat? format = default)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |
| формат | Nullable`1 | Определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *output* недоступен для записи. — или — *output* является тем же потоком, из которого мы извлекаем. Архив был освобождён и не может быть использован — ИЛИ — Невозможно сохранить архив в *format* из‑за ограничений формата. |

## Примечания

*output* must be writable.

## Примеры

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry1", "data.bin");
        archive.Save(tarFile);
    }
}       
```

### См. также

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, TarFormat?) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, TarFormat? format = default)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| формат | Nullable`1 | Определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно. |

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
| ObjectDisposedException | Архив был освобождён и не может быть использован |

## Примечания

Можно сохранить архив в тот же путь, из которого он был загружен. Однако это не рекомендуется, потому что такой подход использует копирование во временный файл.

## Примеры

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("myarchive.tar");
}       
```

### См. также

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


