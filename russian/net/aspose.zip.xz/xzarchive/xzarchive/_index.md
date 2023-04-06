---
title: XzArchive.XzArchive
second_title: Aspose.ZIP для справочника API .NET
description: XzArchive строитель. Инициализирует новый экземплярXzArchive class и составляет архив в формате xz.
type: docs
weight: 10
url: /ru/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Инициализирует новый экземпляр[`XzArchive`](../) class и составляет архив в формате xz.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| settings | XzArchiveSettings | Набор настроек конкретного архива xz: размер словаря, размер блока, тип проверки. |

### Смотрите также

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* пространство имен [Aspose.Zip.Xz](../../xzarchive/)
* сборка [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

Инициализирует новый экземпляр[`XzArchive`](../) класс подготовлен к распаковке.

```csharp
public XzArchive(Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Источник архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *source* не доступен для поиска. |
| ArgumentNullException | *source* нулевой. |

### Примечания

Этот конструктор не распаковывается. Видеть[`Extract`](../extract/) метод распаковки.

### Смотрите также

* class [XzArchive](../)
* пространство имен [Aspose.Zip.Xz](../../xzarchive/)
* сборка [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

Инициализирует новый экземпляр[`XzArchive`](../) класс подготовлен к распаковке.

```csharp
public XzArchive(string path)
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

### Примечания

Этот конструктор не распаковывается. Видеть[`Extract`](../extract/) метод распаковки.

### Смотрите также

* class [XzArchive](../)
* пространство имен [Aspose.Zip.Xz](../../xzarchive/)
* сборка [Aspose.Zip](../../../)


