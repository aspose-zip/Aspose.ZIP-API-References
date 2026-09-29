---
title: "CancelEntryEventArgsXar"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Παράμετροι συμβάντος για ακυρώσιμα συμβάντα σχετιζόμενα με καταχώρηση."
type: docs
weight: 53
url: /el/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

Παράμετροι συμβάντος για ακυρώσιμα συμβάντα σχετιζόμενα με καταχώρηση.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | Δημιουργεί μια νέα παρουσία της κλάσης [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCancel()](#getCancel--) | Λαμβάνει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός. |
| [setCancel(boolean value)](#setCancel-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός. |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


Δημιουργεί μια νέα παρουσία της κλάσης [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | το στοιχείο του αρχείου για το οποίο ενεργοποιείται το συμβάν |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός.

**Returns:**
boolean - true εάν το συμβάν πρέπει να ακυρωθεί· διαφορετικά, false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | boolean | true εάν το συμβάν πρέπει να ακυρωθεί· διαφορετικά, false |

