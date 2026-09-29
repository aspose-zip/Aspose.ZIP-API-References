---
title: "ParallelCompressionMode"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni di utilizzo della funzionalità di compressione parallela."
type: docs
weight: 166
url: /it/java/com.aspose.zip/parallelcompressionmode/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ParallelCompressionMode extends Enum<ParallelCompressionMode>
```

Opzioni di utilizzo della funzionalità di compressione parallela.
## Campi

| Campo | Descrizione |
| --- | --- |
| [Always](#Always) | Esegui la compressione in parallelo. |
| [Auto](#Auto) | Decidi se utilizzare la compressione parallela in base alle voci. |
| [Never](#Never) | Non comprimere in parallelo. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ParallelCompressionMode Always
```


Esegui la compressione in parallelo. Attenzione a un consumo elevato di memoria.

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


Non comprimere in parallelo.

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
