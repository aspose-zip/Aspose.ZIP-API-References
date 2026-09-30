---
title: "AlzArchive.AlzArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор AlzArchive. Инициализирует новый экземпляр класса AlzArchive из потока"
type: docs
weight: 10
url: /ru/net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

Инициализирует новый экземпляр класса [`AlzArchive`](../) из потока.

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток архива ALZ. Поток должен поддерживать чтение и перемещение. |
| loadOptions | AlzArchiveLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | Поток равен null. |

### См. также

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`AlzArchive`](../) из пути к файлу.

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу архива ALZ. |
| loadOptions | AlzArchiveLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | filePath равен null. |
| FileNotFoundException | Файл не существует. |

### См. также

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


