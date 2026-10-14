---
title: "SelfExtractorOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές για τη δημιουργία αυτοεξαγώγιμου εκτελέσιμου αρχείου."
type: docs
weight: 102
url: /el/java/com.aspose.zip/selfextractoroptions/
---

**Inheritance:**
java.lang.Object
```
public class SelfExtractorOptions
```

Επιλογές για τη δημιουργία αυτοεξαγώγιμου εκτελέσιμου αρχείου.

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


