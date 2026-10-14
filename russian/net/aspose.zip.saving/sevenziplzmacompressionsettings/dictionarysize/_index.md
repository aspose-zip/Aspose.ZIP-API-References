---
title: "SevenZipLZMACompressionSettings.DictionarySize"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "SevenZipLZMACompressionSettings свойство. Размер буфера истории словаря указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти. Если не задан, будет выбран в соответствии с размером записи. Должен быть между 4096 и 1073741824 или равен нулю для автоматического определения на основе размера записи"
type: docs
weight: 20
url: /ru/net/aspose.zip.saving/sevenziplzmacompressionsettings/dictionarysize/
---
## SevenZipLZMACompressionSettings.DictionarySize property

Размер словаря (буфера истории) указывает, сколько байт недавно обработанных несжатых данных хранится в памяти. Если не задан, будет выбран в соответствии с размером записи. Должен быть от 4096 до 1073741824, либо равен нулю для автоматического определения на основе размера записи.

```csharp
public int DictionarySize { get; set; }
```

## Примечания

Чем больше словарь, тем обычно лучше коэффициент сжатия — но словари, превышающие размер несжатых данных, являются пустой тратой ОЗУ.

### См. также

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


