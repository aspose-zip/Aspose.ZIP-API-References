---
title: "XarArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод XarArchive. Сохраняет архив в указанный файл назначения"
type: docs
weight: 80
url: /ru/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| saveOptions | XarSaveOptions | Параметры для сохранения xar‑архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *destinationFileName* равно null. |
| InvalidOperationException | Невозможно изменить архив xar. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |
| UnauthorizedAccessException | *destinationFileName* указывает файл, который доступен только для чтения. -or- *destinationFileName* указывает каталог. -or- У вызывающего нет необходимого разрешения. |

### См. также

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

Сохраняет архив в предоставленный поток.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |
| saveOptions | XarSaveOptions | Параметры для сохранения xar‑архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* равен null. |
| ArgumentException | *output* недоступен для записи/чтения или не поддерживает позиционирование. |
| InvalidOperationException | Невозможно изменить архив xar. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

### См. также

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


