---
title: "AppleArchive.AppleArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор AppleArchive. Инициализирует новый экземпляр класса AppleArchive с настройками, используемыми для составленных записей"
type: docs
weight: 10
url: /ru/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

Инициализирует новый экземпляр класса [`AppleArchive`](../) с настройками, используемыми для составленных записей.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | Настройки, используемые при создании нового Apple Archive. |

### См. также

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`AppleArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| loadOptions | AppleArchiveLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* имеет значение null. |
| ArgumentException | *sourceStream* не поддерживает перемещение. |
| InvalidDataException | *sourceStream* не является действительным Apple Archive. |
| EndOfStreamException | Поток неожиданно заканчивается во время разбора записей архива. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. методы [`ExtractToDirectory`](../extracttodirectory/) и [`Open`](../../applearchiveentry/open/) для распаковки.

### См. также

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`AppleArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Полный или относительный путь к файлу архива. |
| loadOptions | AppleArchiveLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| FileNotFoundException | Файл не найден. |
| InvalidDataException | *path* не является действительным Apple Archive. |
| EndOfStreamException | Поток неожиданно заканчивается во время разбора записей архива. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. методы [`ExtractToDirectory`](../extracttodirectory/) и [`Open`](../../applearchiveentry/open/) для распаковки.

### См. также

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


