---
title: "SevenZipEntrySettings.Solid"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство SevenZipEntrySettings. Возвращает или задает значение, указывающее, следует ли объединять элементы и рассматривать их как один блок данных."
type: docs
weight: 50
url: /ru/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

Получает или задает значение, указывающее, следует ли конкатенировать записи и рассматривать их как один блок данных.

```csharp
public bool Solid { get; set; }
```

## Примечания

Предоставьте `SevenZipEntrySettings` для сплошного 7z‑архива при создании архива.

## Примеры

В следующем примере показано, как сжать каталог в сплошной 7z‑архив с компрессией LZMA2 без шифрования.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### См. также

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


