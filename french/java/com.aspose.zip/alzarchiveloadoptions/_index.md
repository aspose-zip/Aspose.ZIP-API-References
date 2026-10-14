---
title: "AlzArchiveLoadOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options avec lesquelles une archive ALZ est chargée à partir d'un fichier compressé."
type: docs
weight: 12
url: /fr/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

Options avec lesquelles une archive ALZ est chargée à partir d'un fichier compressé.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Obtient le mot de passe utilisé pour déchiffrer les entrées. |
| [getEncoding()](#getEncoding--) | Obtient l'encodage utilisé pour les noms d'entrée. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Obtient si la vérification du checksum des entrées ALZ est ignorée. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Définit un drapeau d'annulation utilisé pour annuler l'extraction. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Définit le mot de passe utilisé pour déchiffrer les entrées. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Définit l'encodage utilisé pour les noms d'entrée. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Définit si la vérification du checksum des entrées ALZ est ignorée. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Obtient le mot de passe utilisé pour déchiffrer les entrées.

**Returns:**
java.lang.String - mot de passe utilisé pour déchiffrer les entrées, ou `null` lorsqu'aucun n'est configuré
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Obtient l'encodage utilisé pour les noms d'entrée. La valeur par défaut est la page de code Windows coréenne 949 (CP949). Les archives ALZ stockent historiquement les noms de fichiers en utilisant la page de code ANSI Windows coréenne.

**Returns:**
java.nio.charset.Charset - encodage utilisé pour les noms d'entrée
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


Obtient si la vérification du checksum des entrées ALZ est ignorée. La valeur par défaut est `false`.

**Returns:**
boolean - si la vérification du checksum est ignorée
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Définit un drapeau d'annulation utilisé pour annuler l'extraction.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | drapeau d'annulation, ou `null` pour désactiver l'annulation |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Définit le mot de passe utilisé pour déchiffrer les entrées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | mot de passe utilisé pour déchiffrer les entrées |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Définit l'encodage utilisé pour les noms d'entrée. Les archives ALZ stockent historiquement les noms de fichiers en utilisant la page de code ANSI Windows coréenne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.nio.charset.Charset | encodage utilisé pour les noms d'entrée |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


Définit si la vérification du checksum des entrées ALZ est ignorée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | si la vérification du checksum est ignorée |

