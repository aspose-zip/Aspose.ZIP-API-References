---
title: "AppleArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод AppleArchive. Сохраняет архив в предоставленный поток."
type: docs
weight: 90
url: /ru/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

Сохраняет архив в предоставленный поток.

```csharp
public void Save(Stream output)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Архив был освобождён. |
| ArgumentNullException | *output* равен `null`. |
| ArgumentException | *output* не доступен для записи. |
| ArgumentOutOfRangeException | Настроенный размер блока LZ4 или Zlib не является положительным. |
| NotSupportedException | Настройки сжатия отсутствуют или не поддерживаются, прямая компоновка использует поток без возможности перемещения, либо размер записи/архива превышает текущие ограничения Apple Archive. |

## Примечания

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### См. также

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к архиву, который будет создан. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Архив был освобождён. |
| ArgumentException | *destinationFileName* недействителен. |
| ArgumentNullException | *destinationFileName* равен `null`. |
| ArgumentOutOfRangeException | Настроенный размер блока LZ4 или Zlib не является положительным. |
| NotSupportedException | Настройки сжатия отсутствуют или не поддерживаются, прямая компоновка использует поток без возможности перемещения, либо размер записи/архива превышает текущие ограничения Apple Archive. |

### См. также

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


