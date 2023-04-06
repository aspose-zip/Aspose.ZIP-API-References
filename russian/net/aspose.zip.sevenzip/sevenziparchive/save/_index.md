---
title: SevenZipArchive.Save
second_title: Aspose.ZIP для справочника API .NET
description: SevenZipArchive метод. Сохраняет архив 7z в указанный поток.
type: docs
weight: 80
url: /ru/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

Сохраняет архив 7z в указанный поток.

```csharp
public void Save(Stream output)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Целевой поток. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *output* не поддерживает поиск. |
| ArgumentNullException | *output* нулевой. |
| InvalidOperationException | Кодеру не удалось сжать данные. |

### Примечания

*output* должен быть доступен для поиска.

### Примеры

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

### Смотрите также

* class [SevenZipArchive](../)
* пространство имен [Aspose.Zip.SevenZip](../../sevenziparchive/)
* сборка [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь создаваемого архива. Если указанное имя файла указывает на существующий файл, он будет перезаписан. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *destinationFileName* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *destinationFileName* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*destinationFileName* отказано. |
| PathTooLongException | Указанный*destinationFileName*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*destinationFileName* содержит двоеточие (:) в середине строки. |

### Примечания

Архив можно сохранить по тому же пути, по которому он был загружен из . Однако делать это не рекомендуется, поскольку при таком подходе используется копирование во временный файл.

### Примеры

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

### Смотрите также

* class [SevenZipArchive](../)
* пространство имен [Aspose.Zip.SevenZip](../../sevenziparchive/)
* сборка [Aspose.Zip](../../../)


