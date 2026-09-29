---
title: "SevenZipEncryptionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Classe de base pour les paramètres de plusieurs méthodes de chiffrement 7z."
type: docs
weight: 112
url: /fr/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

Classe de base pour les paramètres de plusieurs méthodes de chiffrement 7z.

L'AES-256 est la seule méthode de chiffrement possible pour les archives 7z. Ainsi, le [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) est la seule implémentation.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | Obtient une valeur indiquant le chiffrement de l'en-tête. |
| [getPassword()](#getPassword--) | Obtient le mot de passe pour le chiffrement ou le déchiffrement. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | Définit une valeur indiquant le chiffrement de l'en-tête. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Définit le mot de passe pour le chiffrement ou le déchiffrement. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


Obtient une valeur indiquant le chiffrement de l'en-tête.

Ce paramètre est équivalent à l'option `-mhe=on` de l'outil 7-Zip. Actuellement, il est incompatible avec la compression de l'en-tête.

**Returns:**
boolean - une valeur indiquant le chiffrement de l'en-tête
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Obtient le mot de passe pour le chiffrement ou le déchiffrement.

**Returns:**
java.lang.String - mot de passe pour le chiffrement ou le déchiffrement
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


Définit une valeur indiquant le chiffrement de l'en-tête.

Ce paramètre est équivalent à l'option `-mhe=on` de l'outil 7-Zip. Actuellement, il est incompatible avec la compression de l'en-tête.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant le chiffrement de l'en-tête |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Définit le mot de passe pour le chiffrement ou le déchiffrement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | mot de passe pour le chiffrement ou le déchiffrement |

