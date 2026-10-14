---
title: "AppleArchiveEntry.Extract"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод AppleArchiveEntry. Извлекает запись в файловую систему по указанному пути"
type: docs
weight: 50
url: /ru/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

Извлекает запись в файловую систему по указанному пути.

```csharp
public FileInfo Extract(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidDataException | Контрольная сумма или дайджест, сохранённые для записи, не соответствуют извлечённым данным. |
| InvalidOperationException | Запись принадлежит архиву, подготовленному для композиции, либо данные записи нельзя открыть из не‑перемещаемого (non-seekable) потока архива. |
| NotSupportedException | Запись принадлежит сплошному (solid) Apple Archive или использует неподдерживаемый метод сжатия. |
| ObjectDisposedException | Исходный поток был освобождён. |
| IOException | Произошла ошибка ввода/вывода. |

### См. также

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Извлекает запись в предоставленный поток.

```csharp
public void Extract(Stream destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | Stream | Поток назначения. Должен поддерживать запись. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *destination* равно `null`. |
| ArgumentException | *destination* не поддерживает запись. |
| InvalidDataException | Контрольная сумма или дайджест, сохранённые для записи, не соответствуют извлечённым данным. |
| InvalidOperationException | Запись принадлежит архиву, подготовленному для композиции, либо данные записи нельзя открыть из не‑перемещаемого (non-seekable) потока архива. |
| NotSupportedException | Запись принадлежит сплошному (solid) Apple Archive или использует неподдерживаемый метод сжатия. |
| ObjectDisposedException | Исходный поток был освобождён. |
| IOException | Произошла ошибка ввода/вывода. |

### См. также

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


