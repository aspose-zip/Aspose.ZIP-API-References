---
title: "SelfExtractorOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options pour la création d'une archive exécutable auto-extractible."
type: docs
weight: 102
url: /fr/java/com.aspose.zip/selfextractoroptions/
---

**Inheritance:**
java.lang.Object
```
public class SelfExtractorOptions
```

Options pour la création d'une archive exécutable auto-extractible.

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


