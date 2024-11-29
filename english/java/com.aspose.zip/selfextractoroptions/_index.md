---
title: SelfExtractorOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for creation of self-extracting executable archive.
type: docs
weight: 65
url: /java/com.aspose.zip/selfextractoroptions/
---

**Inheritance:**
java.lang.Object
```
public class SelfExtractorOptions
```

Options for creation of self-extracting executable archive.

```

     try (FileOutputStream zipFile = new FileOutputStream("archive.exe")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("entry.bin", "data.bin");
             ArchiveSaveOptions options = new ArchiveSaveOptions();
             options.setSelfExtractorOptions(new SelfExtractorOptions());
             archive.save(zipFile, options);
         }
     } catch (IOException ex) {
     }
 
```


## Constructors

| Constructor | Description |
| --- | --- |
| [SelfExtractorOptions()](#SelfExtractorOptions--) |  |
### SelfExtractorOptions() {#SelfExtractorOptions--}
```
public SelfExtractorOptions()
```


