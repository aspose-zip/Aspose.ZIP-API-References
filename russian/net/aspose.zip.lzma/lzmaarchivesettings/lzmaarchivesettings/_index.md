---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Aspose.ZIP для справочника API .NET
description: LzmaArchiveSettings строитель. Инициализирует новый экземплярLzmaArchiveSettingsclass с размером словаря по умолчанию равным 16 мегабайтам.
type: docs
weight: 10
url: /ru/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Инициализирует новый экземпляр[`LzmaArchiveSettings`](../)class с размером словаря по умолчанию, равным 16 мегабайтам.

```csharp
public LzmaArchiveSettings()
```

### Примеры

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### Смотрите также

* class [LzmaArchiveSettings](../)
* пространство имен [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* сборка [Aspose.Zip](../../../)


