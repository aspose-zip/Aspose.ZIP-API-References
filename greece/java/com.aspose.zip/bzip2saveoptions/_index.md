---
title: "Bzip2SaveOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές για αποθήκευση ενός αρχείου bzip2."
type: docs
weight: 43
url: /el/java/com.aspose.zip/bzip2saveoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2SaveOptions
```

Επιλογές για αποθήκευση ενός αρχείου bzip2.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Bzip2SaveOptions(int blockSize)](#Bzip2SaveOptions-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions). |
| [Bzip2SaveOptions()](#Bzip2SaveOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) με προεπιλεγμένο μέγεθος μπλοκ, ίσο με 9 εκατοντάδες kilobytes. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Μέγεθος μπλοκ σε εκατοντάδες kilobytes. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται. |
| [getCompressionThreads()](#getCompressionThreads--) | Λαμβάνει τον αριθμό των νημάτων συμπίεσης. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Ορίζει τον αριθμό των νημάτων συμπίεσης. |
### Bzip2SaveOptions(int blockSize) {#Bzip2SaveOptions-int-}
```
public Bzip2SaveOptions(int blockSize)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions).

```

``````

try (FileOutputStream result = new FileOutputStream("archive.bz2")) {
try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource("data.bin");
archive.save(result, new Bzip2SaveOptions(9));
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2SaveOptions() {#Bzip2SaveOptions--}
```
public Bzip2SaveOptions()
```


Initializes a new instance of the [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (FileOutputStream result = new FileOutputStream("archive.bz2")) {
         try (Bzip2Archive archive = new Bzip2Archive()) {
             archive.setSource("data.bin");
             archive.save(result, new Bzip2SaveOptions());
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Μέγεθος μπλοκ σε εκατοντάδες kilobytes.

**Returns:**
int - μέγεθος μπλοκ σε εκατοντάδες kilobytes
### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται.

```

``````

File source = new File("huge.bin");
Bzip2SaveOptions settings = new Bzip2SaveOptions();
settings.setCompressionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / source.length());
});
 
```

This event won't be raised when compressing in multithreaded mode.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

     File source = new File("huge.bin");
     Bzip2SaveOptions settings = new Bzip2SaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```

Αυτό το γεγονός δεν θα ενεργοποιηθεί όταν γίνεται συμπίεση σε πολυνηματική λειτουργία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ένα συμβάν που ενεργοποιείται όταν συμπιέζεται ένα τμήμα της ακατέργαστης ροής |

### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Ορίζει τον αριθμό των νημάτων συμπίεσης. Εάν η τιμή είναι μεγαλύτερη από 1, θα χρησιμοποιηθεί συμπίεση πολυνηματική.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | int | αριθμός νημάτων συμπίεσης. |

