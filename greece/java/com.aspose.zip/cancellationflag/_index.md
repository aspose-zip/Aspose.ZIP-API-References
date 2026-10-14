---
title: "CancellationFlag"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Η σημαία που επιτρέπει την ακύρωση των λειτουργιών."
type: docs
weight: 54
url: /el/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

Η σημαία που επιτρέπει την ακύρωση των λειτουργιών.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | Δημιουργεί μια παρουσία του CancellationFlag. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [cancel()](#cancel--) | Ακυρώνει τη λειτουργία που σχετίζεται με αυτήν την παρουσία του [CancellationFlag](../../com.aspose.zip/cancellationflag). |
| [cancelAfter(long delay)](#cancelAfter-long-) | Ακυρώνει τη λειτουργία μετά από καθορισμένη καθυστέρηση σε χιλιοστά του δευτερολέπτου. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | Ακυρώνει τη λειτουργία μετά από καθορισμένη καθυστέρηση στη δεδομένη μονάδα χρόνου. |
| [close()](#close--) | Κλείνει την παρουσία του [CancellationFlag](../../com.aspose.zip/cancellationflag) και απελευθερώνει τυχόν πόρους που σχετίζονται με αυτήν. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


Δημιουργεί μια παρουσία του CancellationFlag.

### cancel() {#cancel--}
```
public void cancel()
```


Ακυρώνει τη λειτουργία που σχετίζεται με αυτήν την παρουσία του [CancellationFlag](../../com.aspose.zip/cancellationflag).

Εάν η λειτουργία έχει ήδη ακυρωθεί, αυτή η μέθοδος δεν κάνει τίποτα.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


Ακυρώνει τη λειτουργία μετά από καθορισμένη καθυστέρηση σε χιλιοστά του δευτερολέπτου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| delay | long | Η καθυστέρηση σε χιλιοστά του δευτερολέπτου μετά την οποία η λειτουργία θα ακυρωθεί. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


Ακυρώνει τη λειτουργία μετά από καθορισμένη καθυστέρηση στη δεδομένη μονάδα χρόνου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| delay | long | Η καθυστέρηση μετά την οποία η λειτουργία θα ακυρωθεί. |
| unit | java.util.concurrent.TimeUnit | Η μονάδα χρόνου της παραμέτρου καθυστέρησης. |

### close() {#close--}
```
public void close()
```


Κλείνει την παρουσία του [CancellationFlag](../../com.aspose.zip/cancellationflag) και απελευθερώνει τυχόν πόρους που σχετίζονται με αυτήν.

