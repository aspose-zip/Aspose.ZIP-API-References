---
title: "SelfExtractorOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "自己解凍実行可能アーカイブの作成オプション。"
type: docs
weight: 102
url: /ja/java/com.aspose.zip/selfextractoroptions/
---

**Inheritance:**
java.lang.Object
```
public class SelfExtractorOptions
```

自己解凍実行可能アーカイブの作成オプション。

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.exe\")) {
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


