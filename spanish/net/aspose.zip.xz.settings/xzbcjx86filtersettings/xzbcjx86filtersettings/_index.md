---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: XzBcjX86FilterSettings constructor. Inicializa una nueva instancia delXzBcjX86FilterSettings . Úselo para comprimir archivos ejecutables y bibliotecas dentroXzArchive .
type: docs
weight: 10
url: /es/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Inicializa una nueva instancia del[`XzBcjX86FilterSettings`](../) . Úselo para comprimir archivos ejecutables y bibliotecas dentro[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### Ejemplos

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

### Ver también

* class [XzBcjX86FilterSettings](../)
* espacio de nombres [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* asamblea [Aspose.Zip](../../../)


