---
title: "ParallelCompressionMode"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές χρήσης της δυνατότητας παράλληλης συμπίεσης."
type: docs
weight: 166
url: /el/java/com.aspose.zip/parallelcompressionmode/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ParallelCompressionMode extends Enum<ParallelCompressionMode>
```

Επιλογές χρήσης της δυνατότητας παράλληλης συμπίεσης.
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
| [Always](#Always) | Συμπιέστε παράλληλα. |
| [Auto](#Auto) | Αποφασίστε αν θα χρησιμοποιηθεί παράλληλη συμπίεση βάσει των καταχωρήσεων. |
| [Never](#Never) | Μην συμπιέζετε παράλληλα. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ParallelCompressionMode Always
```


Συμπιέστε παράλληλα. Προσέξτε την κατανάλωση μνήμης.

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


Μην συμπιέζετε παράλληλα.

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
