---
title: "EncryptionMethod"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Les méthodes de chiffrement/déchiffrement peuvent être utilisées avec une archive ZIP."
type: docs
weight: 165
url: /fr/java/com.aspose.zip/encryptionmethod/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum EncryptionMethod extends Enum<EncryptionMethod>
```

Les méthodes de chiffrement/déchiffrement peuvent être utilisées avec une archive ZIP.
## Champs

| Champ | Description |
| --- | --- |
| [AES128](#AES128) | Advanced Encryption Standard avec une longueur de clé de 128 bits. |
| [AES192](#AES192) | Standard de chiffrement avancé avec une longueur de clé de 192 bits. |
| [AES256](#AES256) | Standard de chiffrement avancé avec une longueur de clé de 256 bits. |
| [Traditional](#Traditional) | Chiffrement PKWARE traditionnel. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### AES128 {#AES128}
```
public static final EncryptionMethod AES128
```


Advanced Encryption Standard avec une longueur de clé de 128 bits.

### AES192 {#AES192}
```
public static final EncryptionMethod AES192
```


Standard de chiffrement avancé avec une longueur de clé de 192 bits.

### AES256 {#AES256}
```
public static final EncryptionMethod AES256
```


Standard de chiffrement avancé avec une longueur de clé de 256 bits.

### Traditional {#Traditional}
```
public static final EncryptionMethod Traditional
```


Chiffrement PKWARE traditionnel.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static EncryptionMethod valueOf(String name)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[EncryptionMethod](../../com.aspose.zip/encryptionmethod)
### values() {#values--}
```
public static EncryptionMethod[] values()
```




**Returns:**
com.aspose.zip.EncryptionMethod[]
