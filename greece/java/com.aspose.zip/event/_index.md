---
title: "Γεγονός"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ένα συμβάν."
type: docs
weight: 160
url: /el/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

Ένα συμβάν.

`TArgs`: επιχειρήματα γεγονότος.

TArgs :
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Αυτή η μέθοδος καλείται όταν εκδίδεται το γεγονός. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Αυτή η μέθοδος καλείται όταν εκδίδεται το γεγονός.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| αποστολέας | java.lang.Object | ένα αντικείμενο που ενεργοποιεί αυτό το γεγονός. |
| ορίσματα | TArgs | προσαρμοσμένα ορίσματα. |

