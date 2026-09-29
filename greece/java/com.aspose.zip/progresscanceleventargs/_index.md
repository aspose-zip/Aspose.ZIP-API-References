---
title: "ProgressCancelEventArgs"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Κλάση για δεδομένα ακυρώσιμου γεγονότος που περιέχει τον αριθμό των επεξεργασμένων byte."
type: docs
weight: 95
url: /el/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

Κλάση για δεδομένα ακυρώσιμου γεγονότος που περιέχει τον αριθμό των επεξεργασμένων byte.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCancel()](#getCancel--) | Λαμβάνει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός. |
| [setCancel(boolean value)](#setCancel-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| proceededBytes | long | Ο αριθμός των byte που έχουν προχωρήσει. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός.

**Returns:**
boolean - Αληθές εάν το γεγονός πρέπει να ακυρωθεί· διαφορετικά, ψευδές.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να ακυρωθεί το γεγονός.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | boolean | μια τιμή που υποδεικνύει εάν το γεγονός πρέπει να ακυρωθεί. |

