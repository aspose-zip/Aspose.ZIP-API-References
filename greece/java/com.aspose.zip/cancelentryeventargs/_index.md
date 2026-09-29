---
title: "CancelEntryEventArgs"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Παράμετροι συμβάντος για ακυρώσιμα συμβάντα σχετιζόμενα με καταχώρηση."
type: docs
weight: 52
url: /el/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

Παράμετροι συμβάντος για ακυρώσιμα συμβάντα σχετιζόμενα με καταχώρηση.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | Δημιουργεί μια νέα παρουσία της κλάσης [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCancel()](#getCancel--) | Λαμβάνει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός. |
| [setCancel(boolean value)](#setCancel-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


Δημιουργεί μια νέα παρουσία της κλάσης [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Καταχώρηση αρχείου για την οποία ενεργοποιείται το γεγονός. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός.

**Returns:**
boolean - true εάν πρέπει να ακυρωθεί το γεγονός· διαφορετικά, false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | boolean | true εάν πρέπει να ακυρωθεί το γεγονός· διαφορετικά, false. |

