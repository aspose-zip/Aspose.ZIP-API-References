---
title: "Lz4ArchiveSetting"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη σύνθεση του αρχείου LZ4."
type: docs
weight: 81
url: /el/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

Ρυθμίσεις για τη σύνθεση του αρχείου LZ4.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | Αρχικοποιεί μια νέα παρουσία της [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) με προεπιλεγμένες παραμέτρους. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το συμπιεσμένο xxh32 hash στο τέλος του συμπιεσμένου μπλοκ. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το xxh32 hash του περιεχομένου στο τέλος του αρχείου LZ4. |
| [getIncludeContentSize()](#getIncludeContentSize--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το μέγεθος του περιεχομένου στο πλαίσιο. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το συμπιεσμένο xxh32 hash στο τέλος του συμπιεσμένου μπλοκ. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το xxh32 hash του περιεχομένου στο τέλος του αρχείου LZ4. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το μέγεθος του περιεχομένου στο πλαίσιο. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


Αρχικοποιεί μια νέα παρουσία της [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) με προεπιλεγμένες παραμέτρους.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το συμπιεσμένο xxh32 hash στο τέλος του συμπιεσμένου μπλοκ.

Η προεπιλογή είναι ψευδής.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το συμπιεσμένο xxh32 hash στο τέλος του συμπιεσμένου μπλοκ.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το xxh32 hash του περιεχομένου στο τέλος του αρχείου LZ4.

Η προεπιλογή είναι αληθής.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το hash xxh32 του περιεχομένου στο τέλος του αρχείου LZ4.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το μέγεθος του περιεχομένου στο πλαίσιο.

Η προεπιλογή είναι false. Εφαρμόζεται όταν η πηγή ροής είναι αναζητήσιμη.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το μέγεθος του περιεχομένου στο πλαίσιο.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το συμπιεσμένο xxh32 hash στο τέλος του συμπιεσμένου μπλοκ.

Η προεπιλογή είναι ψευδής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | boolean | μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το συμπιεσμένο hash xxh32 στο τέλος του συμπιεσμένου μπλοκ. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το xxh32 hash του περιεχομένου στο τέλος του αρχείου LZ4.

Η προεπιλογή είναι αληθής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | boolean | μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το hash xxh32 του περιεχομένου στο τέλος του αρχείου LZ4. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το μέγεθος του περιεχομένου στο πλαίσιο.

Η προεπιλογή είναι false. Εφαρμόζεται όταν η πηγή ροής είναι αναζητήσιμη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | boolean | μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το μέγεθος του περιεχομένου στο πλαίσιο. |

