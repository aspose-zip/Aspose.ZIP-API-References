---
title: "SevenZipEncryptionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Βασική κλάση για τις ρυθμίσεις πολλών μεθόδων κρυπτογράφησης 7z."
type: docs
weight: 112
url: /el/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

Βασική κλάση για τις ρυθμίσεις πολλών μεθόδων κρυπτογράφησης 7z.

Το AES-256 είναι η μόνη δυνατή μέθοδος κρυπτογράφησης για το αρχείο 7z. Έτσι το [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) είναι η μοναδική υλοποίηση.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | Λαμβάνει μια τιμή που υποδεικνύει κρυπτογράφηση της κεφαλίδας. |
| [getPassword()](#getPassword--) | Λαμβάνει τον κωδικό πρόσβασης για κρυπτογράφηση ή αποκρυπτογράφηση. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | Ορίζει μια τιμή που υποδεικνύει κρυπτογράφηση της κεφαλίδας. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Ορίζει τον κωδικό πρόσβασης για κρυπτογράφηση ή αποκρυπτογράφηση. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


Λαμβάνει μια τιμή που υποδεικνύει κρυπτογράφηση της κεφαλίδας.

Αυτή η ρύθμιση είναι ισοδύναμη με τη μεταβλητή `-mhe=on` του εργαλείου 7-Zip. Προς το παρόν, είναι ασύμβατη με τη συμπίεση κεφαλίδας.

**Returns:**
boolean - μια τιμή που υποδεικνύει κρυπτογράφηση της κεφαλίδας
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Λαμβάνει τον κωδικό πρόσβασης για κρυπτογράφηση ή αποκρυπτογράφηση.

**Returns:**
java.lang.String - κωδικός πρόσβασης για κρυπτογράφηση ή αποκρυπτογράφηση
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει κρυπτογράφηση της κεφαλίδας.

Αυτή η ρύθμιση είναι ισοδύναμη με τη μεταβλητή `-mhe=on` του εργαλείου 7-Zip. Προς το παρόν, είναι ασύμβατη με τη συμπίεση κεφαλίδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | boolean | μια τιμή που υποδεικνύει κρυπτογράφηση της κεφαλίδας |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Ορίζει τον κωδικό πρόσβασης για κρυπτογράφηση ή αποκρυπτογράφηση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.lang.String | κωδικός πρόσβασης για κρυπτογράφηση ή αποκρυπτογράφηση |

