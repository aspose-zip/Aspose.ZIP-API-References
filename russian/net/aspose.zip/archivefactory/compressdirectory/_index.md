---
title: "ArchiveFactory.CompressDirectory"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ArchiveFactory. Сжимает указанный каталог в файл архива, используя заданный формат архива"
type: docs
weight: 10
url: /ru/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

Сжимает указанную директорию в файл архива, используя предоставленный формат архива.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к каталогу, который будет сжат. |
| outputFileName | String | Имя файла назначения. |
| archiveFormat | ArchiveFormat | Формат архива для создания (например, zip, rar, tar и т.д.). |

### Исключения

| исключение | условие |
| --- | --- |
| DirectoryNotFoundException | Выбрасывается, если каталог, указанный в *path*, не существует. |
| ArgumentException | Выбрасывается, если *path* равно null или пустой строке. |
| NotSupportedException | Выбрасывается, если указанный *archiveFormat* не поддерживается или не распознан. |
| ArgumentNullException | *path* равно `null`. |

## Примечания

Этот метод создаст файл архива в месте, указанном параметром *path*. Обычно имя файла архива будет соответствовать имени каталога, к которому добавляется соответствующее расширение файла на основе *archiveFormat*. Сам каталог не изменяется и не удаляется.

## Примеры

Вот пример того, как использовать метод CompressDirectory:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// Это создаст ZIP‑файл с содержимым каталога по указанному пути.
```

### См. также

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


