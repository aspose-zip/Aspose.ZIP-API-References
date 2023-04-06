---
title: LzipArchive.LzipArchive
second_title: Aspose.ZIP для справочника API .NET
description: LzipArchive строитель. Инициализирует новый экземплярLzipArchive .
type: docs
weight: 10
url: /ru/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Инициализирует новый экземпляр[`LzipArchive`](../) .

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| settings | LzipArchiveSettings | Настройка конкретного lzip-архива с определением размера словаря. |

### Смотрите также

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* пространство имен [Aspose.Zip.Lzip](../../lziparchive/)
* сборка [Aspose.Zip](../../../)

---

## LzipArchive(Stream) {#constructor_1}

Инициализирует новый экземпляр[`LzipArchive`](../) класс подготовлен к распаковке.

```csharp
public LzipArchive(Stream sourceStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *sourceStream* не доступен для поиска. |
| ArgumentNullException | *sourceStream* нулевой. |
| InvalidDataException | Заголовки не соответствуют типу архива lzip. |

### Примечания

Этот конструктор не распаковывается. Видеть[`Extract`](../extract/) метод распаковки.

### Смотрите также

* class [LzipArchive](../)
* пространство имен [Aspose.Zip.Lzip](../../lziparchive/)
* сборка [Aspose.Zip](../../../)

---

## LzipArchive(string) {#constructor_2}

Инициализирует новый экземпляр[`LzipArchive`](../) класс подготовлен к распаковке.

```csharp
public LzipArchive(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к источнику архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *path* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path* отказано. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*path* содержит двоеточие (:) в середине строки. |
| InvalidDataException | Заголовки не соответствуют типу архива lzip. |

### Примечания

Этот конструктор не распаковывается. Видеть[`Extract`](../extract/) метод распаковки.

### Примеры

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### Смотрите также

* class [LzipArchive](../)
* пространство имен [Aspose.Zip.Lzip](../../lziparchive/)
* сборка [Aspose.Zip](../../../)


