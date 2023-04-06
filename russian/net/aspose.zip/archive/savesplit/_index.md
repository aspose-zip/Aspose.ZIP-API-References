---
title: Archive.SaveSplit
second_title: Aspose.ZIP для справочника API .NET
description: Archive метод. Сохраняет многотомный архив в указанный каталог назначения.
type: docs
weight: 100
url: /ru/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

Сохраняет многотомный архив в указанный каталог назначения.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | String | Путь к каталогу, в котором будут создаваться сегменты архива. |
| options | SplitArchiveSaveOptions | Варианты сохранения архива, включая имя файла. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Этот архив был открыт из существующего источника. |
| NotSupportedException | Этот архив сжат методом XZ и зашифрован. |
| ArgumentNullException | *destinationDirectory* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения для доступа к каталогу. |
| ArgumentException | *destinationDirectory* содержит недопустимые символы, такие как ", &gt;, &lt; или &#x7C;. |
| PathTooLongException | Указанный путь превышает максимальную длину, определенную системой. |

### Примечания

Этот метод состоит из нескольких (`н`) файлы имя_файла.z01, имя_файла.z02, ..., имя_файла.z(n-1), имя_файла.zip.

Невозможно сделать существующий архив многотомным.

### Примеры

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Смотрите также

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* пространство имен [Aspose.Zip](../../archive/)
* сборка [Aspose.Zip](../../../)


