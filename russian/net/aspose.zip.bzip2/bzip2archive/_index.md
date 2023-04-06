---
title: Class Bzip2Archive
second_title: Aspose.ZIP для справочника API .NET
description: Aspose.Zip.Bzip2.Bzip2Archive сорт. Этот класс представляет файл архива bzip2. Используйте его для создания или извлечения архивов bzip2.
type: docs
weight: 100
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
| [Bzip2Archive](bzip2archive/#constructor)() | Инициализирует новый экземпляр`Bzip2Archive` класс подготовлен к сжатию. |
| [Bzip2Archive](bzip2archive/#constructor_1)(Stream) | Инициализирует новый экземпляр`Bzip2Archive` класс подготовлен к распаковке. |
| [Bzip2Archive](bzip2archive/#constructor_2)(string) | Инициализирует новый экземпляр`Bzip2Archive` класс подготовлен к распаковке. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../aspose.zip.bzip2/bzip2archive/dispose/)() | Выполняет определяемые приложением задачи, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/)(Stream) | Извлекает архив в указанный поток. |
| [Open](../../aspose.zip.bzip2/bzip2archive/open/)() | Открывает архив для извлечения и предоставляет поток с содержимым архива. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save)(Stream, Bzip2SaveOptions) | Сохраняет архив в указанный поток. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save_1)(string, Bzip2SaveOptions) | Сохраняет архив в указанный файл назначения. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_2)(FileInfo) | Задает сжатие содержимого внутри архива. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_3)(Stream) | Задает сжатие содержимого внутри архива. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_4)(string) | Задает сжатие содержимого внутри архива. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource)(CpioArchive, CpioFormat) | Задает сжатие содержимого внутри архива. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_1)(TarArchive, TarFormat) | Задает сжатие содержимого внутри архива. |

### Примечания

bzip2 сжимает файлы, используя алгоритм сжатия текста с блочной сортировкой Берроуза-Уилера и кодирование Хаффмана. Подробнее: https://en.wikipedia.org/wiki/Bzip2

### Смотрите также

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* пространство имен [Aspose.Zip.Bzip2](../../aspose.zip.bzip2/)
* сборка [Aspose.Zip](../../)


