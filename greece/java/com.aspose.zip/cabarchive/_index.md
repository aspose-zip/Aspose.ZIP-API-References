---
title: "CabArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο CAB."
type: docs
weight: 44
url: /el/java/com.aspose.zip/cabarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.zip.ICompressionArchive, java.lang.AutoCloseable
```
public class CabArchive implements ICompressionArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο CAB.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CabArchive(CabEntrySettings settings)](#CabArchive-com.aspose.zip.CabEntrySettings-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CabArchive](../../com.aspose.zip/cabarchive) προετοιμασμένο για συμπίεση. |
| [CabArchive(InputStream sourceStream)](#CabArchive-java.io.InputStream-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CabArchive](../../com.aspose.zip/cabarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [CabArchive(InputStream sourceStream, CabLoadOptions loadOptions)](#CabArchive-java.io.InputStream-com.aspose.zip.CabLoadOptions-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CabArchive](../../com.aspose.zip/cabarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [CabArchive(String path)](#CabArchive-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CabArchive](../../com.aspose.zip/cabarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [CabArchive(String path, CabLoadOptions loadOptions)](#CabArchive-java.lang.String-com.aspose.zip.CabLoadOptions-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CabArchive](../../com.aspose.zip/cabarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Προσθέτει στο αρχείο όλα τα αρχεία, αναδρομικά, από τον καθορισμένο φάκελο. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Προσθέτει στο αρχείο όλα τα αρχεία, αναδρομικά, από τον καθορισμένο φάκελο. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Προσθέτει στο αρχείο όλα τα αρχεία αναδρομικά από τη διαδρομή του καθορισμένου φακέλου. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Προσθέτει στο αρχείο όλα τα αρχεία αναδρομικά από τη διαδρομή του καθορισμένου φακέλου. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Δημιουργήστε μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-com.aspose.zip.CabEntrySettings-) | Δημιουργήστε μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Δημιουργήστε μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, InputStream source, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.CabEntrySettings-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο με συγκεκριμένες ρυθμίσεις. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Δημιουργήστε μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, String path, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-com.aspose.zip.CabEntrySettings-) | Δημιουργήστε μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | Δημιουργήστε μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.CabEntrySettings-) | Δημιουργήστε μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία του αρχείου στον παρεχόμενο κατάλογο. |
| [getEntries()](#getEntries--) | Αποκτά καταχωρήσεις τύπου [CabEntry](../../com.aspose.zip/cabentry) που αποτελούν το αρχείο. |
| [getFileEntries()](#getFileEntries--) | Αποκτά καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο cab. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη δοθείσα ροή. |
| [save(OutputStream outputStream, CabSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.CabSaveOptions-) | Αποθηκεύει το αρχείο στη ροή που παρέχεται με συγκεκριμένες επιλογές. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [save(String destinationFileName, CabSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.CabSaveOptions-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
### CabArchive(CabEntrySettings settings) {#CabArchive-com.aspose.zip.CabEntrySettings-}
```
public CabArchive(CabEntrySettings settings)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CabArchive](../../com.aspose.zip/cabarchive) προετοιμασμένο για συμπίεση.

Συμπιέζει ένα αρχείο χρησιμοποιώντας συγκεκριμένες ρυθμίσεις συμπίεσης.

```

``````

CabEntrySettings settings = new CabEntrySettings(new CabStoreCompressionSettings()));
try (CabArchive archive = new CabArchive(settings))
{
archive.createEntry("entry.bin", "data.bin");
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| settings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | the source of the archive |

### CabArchive(InputStream sourceStream) {#CabArchive-java.io.InputStream-}
```
public CabArchive(InputStream sourceStream)
```


Initializes a new instance of the [CabArchive](../../com.aspose.zip/cabarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CabArchive archive = new CabArchive(new FileInputStream("archive.cab"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | η πηγή του αρχείου |

### CabArchive(InputStream sourceStream, CabLoadOptions loadOptions) {#CabArchive-java.io.InputStream-com.aspose.zip.CabLoadOptions-}
```
public CabArchive(InputStream sourceStream, CabLoadOptions loadOptions)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CabArchive](../../com.aspose.zip/cabarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

Το παρακάτω παράδειγμα δείχνει πώς να εξαχθούν όλες οι καταχωρήσεις σε έναν κατάλογο.

```

``````

try (CabArchive archive = new CabArchive(new FileInputStream("archive.cab"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [CabLoadOptions](../../com.aspose.zip/cabloadoptions) | Options to load existing archive with. |

### CabArchive(String path) {#CabArchive-java.lang.String-}
```
public CabArchive(String path)
```


Initializes a new instance of the [CabArchive](../../com.aspose.zip/cabarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου |

### CabArchive(String path, CabLoadOptions loadOptions) {#CabArchive-java.lang.String-com.aspose.zip.CabLoadOptions-}
```
public CabArchive(String path, CabLoadOptions loadOptions)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CabArchive](../../com.aspose.zip/cabarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

Το παρακάτω παράδειγμα δείχνει πώς να εξαχθούν όλες οι καταχωρήσεις σε έναν κατάλογο.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [CabLoadOptions](../../com.aspose.zip/cabloadoptions) | Options to load existing archive with. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final CabArchive createEntries(File directory)
```


Adds to the archive all files, recursively, from the specified directory.

```

``````

 try (var archive = new CabArchive())
 {
     File directory = new File("C:/Logs");
     archive.createEntries(directory);
     archive.save("logs.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | java.io.File | Κατάλογος προς συμπίεση. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final CabArchive createEntries(File directory, boolean includeRootDirectory)
```


Προσθέτει στο αρχείο όλα τα αρχεία, αναδρομικά, από τον καθορισμένο φάκελο.

```

``````

try (var archive = new CabArchive())
{
File directory = new File("C:/Logs");
archive.createEntries(directory, false);
archive.save("logs.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory name in entry paths. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final CabArchive createEntries(String sourceDirectory)
```


Adds to the archive all files recursively from the specified directory path.

```

``````

 try (var archive = new CabArchive())
 {
     archive.createEntries("C:/Logs");
     archive.save("logs.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Διαδρομή καταλόγου προς συμπίεση. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final CabArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Προσθέτει στο αρχείο όλα τα αρχεία αναδρομικά από τη διαδρομή του καθορισμένου φακέλου.

```

``````

try (var archive = new CabArchive())
{
archive.createEntries("C:/Logs", false);
archive.save("logs.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory path to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory name in entry paths. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final CabEntry createEntry(String name, File fileInfo)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     var sourceFile = new java.io.File("logs\\log.txt");
     archive.createEntry("log.txt", sourceFile);
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
|  | fileInfo | java.io.File | Τα μεταδεδομένα του αρχείου προς συμπίεση. |

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο `name`. Το όνομα αρχείου που παρέχεται στην παράμετρο `fileInfo` δεν επηρεάζει το όνομα της καταχώρησης. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings)
```


Δημιουργήστε μια μοναδική καταχώρηση μέσα στο αρχείο.

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
File sourceFile = new File("logs\\log.txt");
archive.createEntry("log.txt", sourceFile, settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| fileInfo | java.io.File | The metadata of file to be compressed. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item.

The entry name is solely set within `name` parameter. The file name provided in `fileInfo` parameter does not affect the entry name. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final CabEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive(); FileInputStream stream = new FileInputStream("stream-entry.bin"))
 {
     archive.createEntry("stream-entry.bin", stream);
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
| source | java.io.InputStream | Η ροή εισόδου για το στοιχείο. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, InputStream source, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, InputStream source, CabEntrySettings newEntrySettings)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο με συγκεκριμένες ρυθμίσεις.

```

``````

try (CabArchive archive = new CabArchive(); FileInputStream stream = new FileInputStream("stream-entry.bin"))
{
CabEntrySettings settings = new CabEntrySettings(new CabStoreCompressionSettings());
archive.createEntry("stream-entry.bin", stream, settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final CabEntry createEntry(String name, String path)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     archive.createEntry("entry.bin", "data.bin");
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
|  | path | java.lang.String | Το πλήρως προσδιορισμένο όνομα του νέου αρχείου ή το σχετικό όνομα αρχείου που θα συμπιεστεί. |

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο `name`. Το όνομα αρχείου που παρέχεται στην παράμετρο `path` δεν επηρεάζει το όνομα της καταχώρησης. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, String path, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, String path, CabEntrySettings newEntrySettings)
```


Δημιουργήστε μια μοναδική καταχώρηση μέσα στο αρχείο.

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
archive.createEntry(\"entry.bin\", \"data.bin\", settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item.

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final CabEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     archive.createEntry("log.txt", () -> new FileInputStream("log.txt"));
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | Η μέθοδος που παρέχει ροή εισόδου για την καταχώρηση. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, Supplier<InputStream> streamProvider, CabEntrySettings newEntrySettings)
```


Δημιουργήστε μια μοναδική καταχώρηση μέσα στο αρχείο.

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
archive.createEntry(\"log.txt\", () -> new FileInputStream(\"log.txt\"), settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | The method providing input stream for the entry. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία. |

Εάν ο φάκελος δεν υπάρχει, θα δημιουργηθεί |

### getEntries() {#getEntries--}
```
public final List<CabEntry> getEntries()
```


Αποκτά καταχωρήσεις τύπου [CabEntry](../../com.aspose.zip/cabentry) που αποτελούν το αρχείο.

**Returns:**
java.util.List&lt;com.aspose.zip.CabEntry&gt; - καταχωρήσεις τύπου [CabEntry](../../com.aspose.zip/cabentry) που αποτελούν το αρχείο.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Αποκτά καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο cab.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το cab αρχείο.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Αποκτά τη μορφή του αρχείου.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Αποθηκεύει το αρχείο στη δοθείσα ροή.

```

``````

try (CabArchive archive = new CabArchive(); FileOutputStream cabFile = new FileOutputStream(\"archive.cab\"))
{
archive.createEntry("entry.bin", "data.bin");
archive.save(cabFile);
} catch (IOException ex) {
}
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream.

`outputStream` must be writable. |

### save(OutputStream outputStream, CabSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.CabSaveOptions-}
```
public final void save(OutputStream outputStream, CabSaveOptions saveOptions)
```


Saves archive to the stream provided with specific options.

```

``````

  try (CabArchive archive = new CabArchive(); FileOutputStream cabFile = new FileOutputStream("archive.cab"))
  {
      CabSaveOptions options = new CabSaveOptions();
      options.setSkipChecksumCalculation(true);
      archive.createEntry("entry.bin", "data.bin");
      archive.save(cabFile, options);
  } catch (IOException ex) {
  }
  
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Ροή προορισμού. |
|  | saveOptions | [CabSaveOptions](../../com.aspose.zip/cabsaveoptions) | Επιλογές για την αποθήκευση του αρχείου. |

`outputStream` πρέπει να είναι εγγράψιμο. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε.

```

``````

try (CabArchive archive = new CabArchive())
{
archive.createEntry("entry.bin", "data.bin");
archive.save("archive.cab");
} catch (IOException ex) {
}
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file. |

### save(String destinationFileName, CabSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.CabSaveOptions-}
```
public final void save(String destinationFileName, CabSaveOptions saveOptions)
```


Saves archive to the destination file provided.

```

``````

  try (CabArchive archive = new CabArchive())
  {
      CabSaveOptions options = new CabSaveOptions();
      options.setSkipChecksumCalculation(true);
      archive.createEntry("entry.bin", "data.bin");
      archive.save("archive.cab", options);
  } catch (IOException ex) {
  }
  
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | java.lang.String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
|  | saveOptions | [CabSaveOptions](../../com.aspose.zip/cabsaveoptions) | Επιλογές για την αποθήκευση του αρχείου. |

Είναι δυνατόν να αποθηκεύσετε ένα αρχείο σε συμπίεση στην ίδια διαδρομή από την οποία φορτώθηκε. Ωστόσο, αυτό δεν συνιστάται επειδή αυτή η προσέγγιση χρησιμοποιεί αντιγραφή σε προσωρινό αρχείο. |

