---
title: "IsoArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод IsoArchive. Сохраняет ISO‑образ по указанному пути."
type: docs
weight: 70
url: /ru/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

Сохраняет ISO‑образ по указанному пути.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь, по которому будет сохранён ISO‑образ. |
| saveOptions | IsoSaveOptions | Параметры сохранения ISO‑архива. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Выбрасывается, когда архив не находится в режиме редактирования. |
| ArgumentNullException | Выбрасывается, когда *path* равен null. |
| DirectoryNotFoundException | Выбрасывается, когда указанный путь недействителен, например, находится на нераспределённом диске. |
| IOException | Выбрасывается, когда файл уже открыт. |
| UnauthorizedAccessException | Выбрасывается, когда доступ к файлу *path* отклонён. |
| PathTooLongException | Выбрасывается, когда указанный *path* превышает системно определённую максимальную длину. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

В следующем примере показано, как сохранить ISO‑архив в файл:

```csharp
// Создать новый пустой ISO‑архив
using(IsoArchive isoArchive = new IsoArchive())
{
    // Добавить файлы в ISO‑архив
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Сохранить ISO‑архив в файл
    isoArchive.Save("new_archive.iso");
}
```

### См. также

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

Сохраняет ISO‑образ в указанный поток.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток, в который будет сохранён образ ISO. |
| saveOptions | IsoSaveOptions | Параметры сохранения ISO‑архива. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Выбрасывается, когда архив не находится в режиме редактирования. |
| ArgumentNullException | Выбрасывается, когда *stream* имеет значение null. |
| ArgumentException | Выбрасывается, когда *stream* не доступен для записи. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| IOException | Произошла ошибка ввода/вывода. |

## Примеры

В следующем примере показано, как сохранить ISO‑архив в поток памяти:

```csharp

 // Создать новый пустой ISO‑архив
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // Добавить файлы в ISO‑архив
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // Сохранить ISO‑архив в поток памяти
     isoArchive.Save(memoryStream);
 }
```

### См. также

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


