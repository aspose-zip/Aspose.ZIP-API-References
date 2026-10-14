---
title: "SelfExtractorOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "创建自解压可执行存档的选项。"
type: docs
weight: 102
url: /zh/java/com.aspose.zip/selfextractoroptions/
---

**Inheritance:**
java.lang.Object
```
public class SelfExtractorOptions
```

创建自解压可执行存档的选项。

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


