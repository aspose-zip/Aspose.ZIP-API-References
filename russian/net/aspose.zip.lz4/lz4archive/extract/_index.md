---
title: "Lz4Archive.Extract"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод Lz4Archive. Извлекает архив в файл по указанному пути."
type: docs
weight: 30
url: /ru/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

Извлекает архив в файл по указанному пути.

```csharp
public FileInfo Extract(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

### Возвращаемое значение

Информация о извлечённом файле.

### Исключения

| исключение | условие |
| --- | --- |
| EndOfStreamException | Исходный поток слишком короткий. |
| InvalidDataException | Обнаружены неверные байты при декодировании. |
| NotSupportedException | Эта версия LZ4 не поддерживается. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Архив подготовлен для компоновки. |

### См. также

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Извлекает архив в предоставленный поток.

```csharp
public void Extract(Stream destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | Stream | Поток назначения. Должен поддерживать запись. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *destination* не поддерживает запись. |
| EndOfStreamException | Исходный поток слишком короткий. |
| InvalidDataException | Обнаружены неверные байты при декодировании. |
| NotSupportedException | Эта версия LZ4 не поддерживается. |
| InvalidOperationException | Архив подготовлен для компоновки. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### См. также

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


