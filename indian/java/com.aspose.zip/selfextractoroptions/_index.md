---
title: "SelfExtractorOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "स्वयं-निकालने योग्य निष्पादन योग्य अभिलेख बनाने के विकल्प।"
type: docs
weight: 102
url: /hi/java/com.aspose.zip/selfextractoroptions/
---

**Inheritance:**
java.lang.Object
```
public class SelfExtractorOptions
```

स्वयं-निकालने योग्य निष्पादन योग्य अभिलेख बनाने के विकल्प।

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


