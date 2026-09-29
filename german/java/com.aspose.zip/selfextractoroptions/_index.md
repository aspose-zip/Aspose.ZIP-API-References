---
title: "SelfExtractorOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen für die Erstellung eines selbstextrahierenden ausführbaren Archivs."
type: docs
weight: 102
url: /de/java/com.aspose.zip/selfextractoroptions/
---

**Inheritance:**
java.lang.Object
```
public class SelfExtractorOptions
```

Optionen für die Erstellung eines selbstextrahierenden ausführbaren Archivs.

```

``````

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


