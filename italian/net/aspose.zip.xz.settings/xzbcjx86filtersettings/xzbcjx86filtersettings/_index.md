---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: XzBcjX86FilterSettings costruttore. Inizializza una nuova istanza diXzBcjX86FilterSettings . Usalo per comprimere file eseguibili e librerie allinternoXzArchive .
type: docs
weight: 10
url: /it/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Inizializza una nuova istanza di[`XzBcjX86FilterSettings`](../) . Usalo per comprimere file eseguibili e librerie all'interno[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### Esempi

```csharp
XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
using (XzArchive archive = new XzArchive(settings))
{
    archive.SetSource("data.bin");
    archive.Save("archive.xz");
}
```

### Guarda anche

* class [XzBcjX86FilterSettings](../)
* spazio dei nomi [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* assemblea [Aspose.Zip](../../../)


