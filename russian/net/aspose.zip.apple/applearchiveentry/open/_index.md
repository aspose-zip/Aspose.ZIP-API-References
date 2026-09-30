---
title: "AppleArchiveEntry.Open"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод AppleArchiveEntry. Открывает запись для извлечения и предоставляет поток с содержимым записи"
type: docs
weight: 60
url: /ru/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

Открывает запись для извлечения и предоставляет поток с содержимым записи.

```csharp
public Stream Open()
```

### Возвращаемое значение

Читаемый поток, содержащий извлечённые данные записи.

### Исключения

| исключение | условие |
| --- | --- |
| NotSupportedException | Запись принадлежит сплошному (solid) Apple Archive или использует неподдерживаемый метод сжатия. |
| InvalidDataException | Контрольная сумма или дайджест, сохранённые для записи, не соответствуют извлечённым данным. |
| InvalidOperationException | Запись принадлежит архиву, подготовленному для композиции, либо данные записи нельзя открыть из не‑перемещаемого (non-seekable) потока архива. |
| ObjectDisposedException | Исходный поток был освобождён. |
| IOException | Произошла ошибка ввода/вывода. |

## Примечания

Чтение из возвращённого потока позволяет получить оригинальное содержимое записи. Если архив содержит поля контрольных сумм, контрольная сумма проверяется во время чтения возвращённого потока.

### См. также

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


