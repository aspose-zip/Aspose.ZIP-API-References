---
title: "SelfExtractorOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "خيارات لإنشاء أرشيف تنفيذي ذاتي الاستخراج."
type: docs
weight: 102
url: /ar/java/com.aspose.zip/selfextractoroptions/
---

**Inheritance:**
java.lang.Object
```
public class SelfExtractorOptions
```

خيارات لإنشاء أرشيف تنفيذي ذاتي الاستخراج.

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


