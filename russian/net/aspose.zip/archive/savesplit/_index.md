---
title: "Archive.SaveSplit"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод Archive. Сохраняет многотомный архив в указанную директорию назначения."
type: docs
weight: 110
url: /ru/net/aspose.zip/archive/savesplit/
---
## SaveSplit(string, SplitArchiveSaveOptions) {#savesplit_1}

Сохраняет многотомный архив в указанный каталог назначения.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | String | Путь к директории, в которой будут создаваться сегменты архива. |
| параметры | SplitArchiveSaveOptions | Параметры сохранения архива, включая имя файла. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Этот архив был открыт из существующего источника. |
| NotSupportedException | Этот архив одновременно сжат методом XZ и зашифрован. |
| ArgumentNullException | *destinationDirectory* равно null. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к директории. |
| ArgumentException | *destinationDirectory* содержит недопустимые символы, такие как \", &gt;, &lt;, или &#x7C;. |
| PathTooLongException | Указанный путь превышает системно определённую максимальную длину. |
| ObjectDisposedException | Архив освобождён. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |

## Примечания

Этот метод собирает несколько (`n`) файлов filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

Невозможно сделать существующий архив многотомным.

## Примеры

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### См. также

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## SaveSplit(IVolumeStreamProvider, SplitArchiveSaveOptions) {#savesplit}

Сохраняет многотомный архив в потоки, предоставленные поставщиком томов.

```csharp
public void SaveSplit(IVolumeStreamProvider volumeStreamProvider, SplitArchiveSaveOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| volumeStreamProvider | IVolumeStreamProvider | Поставщик потоков назначения для томов архива. |
| options | SplitArchiveSaveOptions | Параметры сохранения архива. [`FileName`](../../../aspose.zip.saving/splitarchivesaveoptions/filename/) игнорируется. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *volumeStreamProvider* или *options* равно null. |
| InvalidOperationException | Этот архив был открыт из существующего источника, либо поставщик возвращает null или поток, не поддерживающий запись. |
| NotSupportedException | Архив использует сжатие XZ. |
| ObjectDisposedException | Архив освобождён. |

## Примечания

Предоставленные потоки не обязаны поддерживать перемещение.

Каждый завершённый том сбрасывается, передаётся в [`VolumeCompleted`](../../../aspose.zip.saving/ivolumestreamprovider/volumecompleted/), а затем освобождается.

Невозможно сделать существующий архив многотомным. Сжатие XZ не поддерживается этой перегрузкой, так как требует перемещения.

## Примеры

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(provider,  new SplitArchiveSaveOptions("volume", 65536));
}
```

### См. также

* interface [IVolumeStreamProvider](../../../aspose.zip.saving/ivolumestreamprovider/)
* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


