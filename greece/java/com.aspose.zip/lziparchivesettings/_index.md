---
title: "LzipArchiveSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Η κλάση περιέχει ρυθμίσεις ενός συγκεκριμένου αρχείου lzip."
type: docs
weight: 84
url: /el/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

Η κλάση περιέχει ρυθμίσεις ενός συγκεκριμένου αρχείου lzip.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | Αρχικοποιεί ένα νέο παράδειγμα του [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με συγκεκριμένο μέγεθος λεξικού. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | Αρχικοποιεί ένα νέο παράδειγμα του [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με συγκεκριμένο μέγεθος λεξικού. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Λαμβάνει τον αριθμό των νημάτων συμπίεσης. |
| [getDictionarySize()](#getDictionarySize--) | Λαμβάνει το μέγεθος του λεξικού που χρησιμοποιείται από τη συμπίεση LZMA. |
| [getFastSpeed()](#getFastSpeed--) | Λαμβάνει το παράδειγμα της κλάσης [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με μέγεθος λεξικού ίσο με 1 megabyte στο φίλτρο LZMA. |
| [getFastestSpeed()](#getFastestSpeed--) | Λαμβάνει το παράδειγμα της κλάσης [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με μέγεθος λεξικού ίσο με 65536 bytes στο φίλτρο LZMA. |
| [getHighCompression()](#getHighCompression--) | Λαμβάνει το παράδειγμα της κλάσης [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με μέγεθος λεξικού ίσο με 32 megabytes στο φίλτρο LZMA. |
| [getMaxMemberSize()](#getMaxMemberSize--) | Λαμβάνει το μέγιστο μέγεθος ενός μέλους στο αρχείο lzip, εκφρασμένο σε bytes. |
| [getMaximumCompression()](#getMaximumCompression--) | Λαμβάνει το παράδειγμα της κλάσης [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με μέγεθος λεξικού ίσο με 64 megabytes στο φίλτρο LZMA. |
| [getNormal()](#getNormal--) | Λαμβάνει το παράδειγμα της κλάσης [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με μέγεθος λεξικού ίσο με 16 megabytes στο φίλτρο LZMA. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Ορίζει τον αριθμό των νημάτων συμπίεσης. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


Αρχικοποιεί ένα νέο παράδειγμα του [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με συγκεκριμένο μέγεθος λεξικού.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dictionarySize | int | μέγεθος λεξικού για τη συμπίεση LZMA σε bytes |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


Αρχικοποιεί ένα νέο παράδειγμα του [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με συγκεκριμένο μέγεθος λεξικού.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dictionarySize | int | μέγεθος λεξικού για τη συμπίεση LZMA σε bytes |
| maxMemberSize | int | Μέγιστο μέγεθος ενός μέλους στο αρχείο lzip, εκφρασμένο σε bytes. Η προεπιλεγμένη τιμή είναι 60 MB. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Λαμβάνει τον αριθμό των νημάτων συμπίεσης. Εάν η τιμή είναι μεγαλύτερη από 1, θα χρησιμοποιηθεί συμπίεση πολλαπλών νημάτων.

**Returns:**
int - αριθμός νημάτων συμπίεσης
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Λαμβάνει το μέγεθος του λεξικού που χρησιμοποιείται από τη συμπίεση LZMA.

**Returns:**
int - το μέγεθος του λεξικού που χρησιμοποιείται από τη συμπίεση LZMA
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


Λαμβάνει το παράδειγμα της κλάσης [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με μέγεθος λεξικού ίσο με 1 megabyte στο φίλτρο LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


Λαμβάνει το παράδειγμα της κλάσης [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με μέγεθος λεξικού ίσο με 65536 bytes στο φίλτρο LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


Λαμβάνει το παράδειγμα της κλάσης [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με μέγεθος λεξικού ίσο με 32 megabytes στο φίλτρο LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


Λαμβάνει το μέγιστο μέγεθος ενός μέλους στο αρχείο lzip, εκφρασμένο σε bytes.

**Returns:**
long - το μέγιστο μέγεθος ενός μέλους στο αρχείο lzip, εκφρασμένο σε bytes
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


Λαμβάνει το παράδειγμα της κλάσης [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με μέγεθος λεξικού ίσο με 64 megabytes στο φίλτρο LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


Λαμβάνει το παράδειγμα της κλάσης [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) με μέγεθος λεξικού ίσο με 16 megabytes στο φίλτρο LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Ορίζει τον αριθμό των νημάτων συμπίεσης. Εάν η τιμή είναι μεγαλύτερη από 1, θα χρησιμοποιηθεί συμπίεση πολυνηματική.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | int | αριθμός νημάτων συμπίεσης |

