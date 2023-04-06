---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: XzBcjX86FilterSettings κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουXzBcjX86FilterSettings . Χρησιμοποιήστε το για να συμπιέσετε εκτελέσιμα αρχεία και βιβλιοθήκες μέσαXzArchive .
type: docs
weight: 10
url: /el/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Αρχικοποιεί μια νέα παρουσία του[`XzBcjX86FilterSettings`](../) . Χρησιμοποιήστε το για να συμπιέσετε εκτελέσιμα αρχεία και βιβλιοθήκες μέσα[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### Παραδείγματα

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

### Δείτε επίσης

* class [XzBcjX86FilterSettings](../)
* χώρος ονομάτων [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* συνέλευση [Aspose.Zip](../../../)


