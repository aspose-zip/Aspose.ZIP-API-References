---
title: "ParallelCompressionMode"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "समांतर संपीड़न सुविधा के उपयोग के विकल्प।"
type: docs
weight: 166
url: /hi/java/com.aspose.zip/parallelcompressionmode/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ParallelCompressionMode extends Enum<ParallelCompressionMode>
```

समांतर संपीड़न सुविधा के उपयोग के विकल्प।
## Fields

| Field | विवरण |
| --- | --- |
| [Always](#Always) | समानांतर में संपीड़न करें। |
| [Auto](#Auto) | एंट्रीज़ के आधार पर तय करें कि समानांतर संपीड़न उपयोग किया जाएगा या नहीं। |
| [Never](#Never) | समानांतर में संपीड़न न करें। |
## Methods

| Method | विवरण |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ParallelCompressionMode Always
```


समानांतर में संपीड़न करें। मेमोरी के अत्यधिक उपयोग से सावधान रहें।

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("filename.bin", "filename.bin");
archive.createEntry("filename1.bin", "filename1.bin");
archive.createEntry("filename2.bin", "filename2.bin");
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


समानांतर में संपीड़न न करें।

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("filename.bin", "filename.bin");
archive.createEntry("filename1.bin", "filename1.bin");
archive.createEntry("filename2.bin", "filename2.bin");
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
