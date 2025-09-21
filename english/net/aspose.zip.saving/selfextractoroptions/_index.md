---
title: Class SelfExtractorOptions
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Saving.SelfExtractorOptions class. Options for creation of selfextracting executable archive
type: docs
weight: 740
url: /net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

Options for creation of self-extracting executable archive.

```csharp
public class SelfExtractorOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | Gets or sets a value indicating whether an extractor window must be closed upon extraction or not. |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | Gets or sets the title of extractor's window. |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | Gets or sets a program to be executed after the archive extraction is completed. |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | Gets or sets the path to title icon for main windows of extractor application. |

## Examples

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictogram.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### See Also

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


