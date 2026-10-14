---
title: "ParallelCompressionMode"
second_title: "Aspose.ZIP for Java API 参考"
description: "并行压缩功能的使用选项。"
type: docs
weight: 166
url: /zh/java/com.aspose.zip/parallelcompressionmode/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ParallelCompressionMode extends Enum<ParallelCompressionMode>
```

并行压缩功能的使用选项。
## 字段

| 字段 | 描述 |
| --- | --- |
| [Always](#Always) | 进行并行压缩。 |
| [Auto](#Auto) | 根据条目决定是否使用并行压缩。 |
| [Never](#Never) | 不进行并行压缩。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ParallelCompressionMode Always
```


进行并行压缩。请注意可能导致内存消耗。

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("filename.bin", "filename.bin");
archive.createEntry("filename1.bin", "filename1.bin");
archive.createEntry(\"filename2.bin\", \"filename2.bin\");
ParallelOptions parallelOptions = new ParallelOptions();
parallelOptions.setParallelCompressInMemory(ParallelCompressionMode.Always);
ArchiveSaveOptions archiveSaveOptions = new ArchiveSaveOptions();
archiveSaveOptions.setParallelOptions(parallelOptions);
archive.save(destination, archiveSaveOptions);
}
 
```



### Auto {#Auto}
```
public static final ParallelCompressionMode Auto
```


Decide whether parallel compression will be used based on the entries. This option may compress in parallel some entries only.

```

``````

    try (Archive archive = new Archive()) {
        archive.createEntry("filename.bin", "filename.bin");
        archive.createEntry("filename1.bin", "filename1.bin");
        archive.createEntry("filename2.bin", "filename2.bin");
        ParallelOptions parallelOptions = new ParallelOptions();
        parallelOptions.setParallelCompressInMemory(ParallelCompressionMode.Auto);
        ArchiveSaveOptions archiveSaveOptions = new ArchiveSaveOptions();
        archiveSaveOptions.setParallelOptions(parallelOptions);
        archive.save(destination, archiveSaveOptions);
    }
 
```



### Never {#Never}
```
public static final ParallelCompressionMode Never
```


不进行并行压缩。

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("filename.bin", "filename.bin");
archive.createEntry("filename1.bin", "filename1.bin");
archive.createEntry(\"filename2.bin\", \"filename2.bin\");
ParallelOptions parallelOptions = new ParallelOptions();
parallelOptions.setParallelCompressInMemory(ParallelCompressionMode.Never);
ArchiveSaveOptions archiveSaveOptions = new ArchiveSaveOptions();
archiveSaveOptions.setParallelOptions(parallelOptions);
archive.save(destination, archiveSaveOptions);
}
 
```



### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ParallelCompressionMode valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[ParallelCompressionMode](../../com.aspose.zip/parallelcompressionmode)
### values() {#values--}
```
public static ParallelCompressionMode[] values()
```




**Returns:**
com.aspose.zip.ParallelCompressionMode[]
