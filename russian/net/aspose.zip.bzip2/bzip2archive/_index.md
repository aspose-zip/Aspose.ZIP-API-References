---
title: "Класс Bzip2Archive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Bzip2.Bzip2Archive. Этот класс представляет файл архива bzip2. Используйте его для создания или извлечения архивов bzip2"
type: docs
weight: 280
url: /ru/net/aspose.zip.bzip2/bzip2archive/
---
## Bzip2Archive class

Этот класс представляет файл архива bzip2. Используйте его для создания или извлечения архивов bzip2.

```csharp
public class Bzip2Archive : IArchive, IArchiveFileEntry
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Bzip2Archive](bzip2archive/#constructor)() | Инициализирует новый экземпляр класса `Bzip2Archive`, подготовленный для сжатия. |
| [Bzip2Archive](bzip2archive/#constructor_1)(Stream, Bzip2LoadOptions) | Инициализирует новый экземпляр класса `Bzip2Archive`, подготовленный для распаковки. |
| [Bzip2Archive](bzip2archive/#constructor_2)(string, Bzip2LoadOptions) | Инициализирует новый экземпляр класса `Bzip2Archive`, подготовленный для распаковки. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../aspose.zip.bzip2/bzip2archive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/#extract_1)(Stream) | Извлекает архив в предоставленный поток. |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/#extract)(string) | Извлекает архив в файл по указанному пути. |
| [ExtractToDirectory](../../aspose.zip.bzip2/bzip2archive/extracttodirectory/)(string) | Извлекает содержимое архива в указанную директорию. |
| [Open](../../aspose.zip.bzip2/bzip2archive/open/)() | Открывает архив для извлечения и предоставляет поток с содержимым архива. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save)(Stream, Bzip2SaveOptions) | Сохраняет архив в предоставленный поток. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save_1)(string, Bzip2SaveOptions) | Сохраняет архив в указанный файл назначения. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_2)(FileInfo) | Устанавливает содержимое, которое будет сжато в архиве. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_3)(Stream) | Устанавливает содержимое, которое будет сжато в архиве. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_4)(string) | Устанавливает содержимое, которое будет сжато в архиве. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource)(CpioArchive, CpioFormat) | Устанавливает содержимое, которое будет сжато в архиве. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_1)(TarArchive, TarFormat) | Устанавливает содержимое, которое будет сжато в архиве. |

## Примечания

bzip2 сжимает файлы, используя алгоритм сортировки блоков текста Burrows-Wheeler и кодирование Хаффмана. Подробнее: https://en.wikipedia.org/wiki/Bzip2

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Bzip2](../../aspose.zip.bzip2/)
* assembly [Aspose.Zip](../../)


