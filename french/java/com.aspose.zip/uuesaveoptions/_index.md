---
title: "UueSaveOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options pour enregistrer un fichier uuencoded."
type: docs
weight: 129
url: /fr/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

Options pour enregistrer un fichier uuencoded.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | Initialise les options avec le nom de fichier fourni par l'utilisateur et une nouvelle ligne. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | Initialise les options avec le nom de fichier fourni par l'utilisateur et la nouvelle ligne par défaut. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getFileName()](#getFileName--) | Obtient le nom de fichier à utiliser lors de la recréation des données décodées. |
| [getNewLine()](#getNewLine--) | Obtient le caractère terminant chaque ligne, généralement "\n" ou "\r\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | Obtient les permissions Unix du fichier. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | Définit les autorisations Unix du fichier. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


Initialise les options avec le nom de fichier fourni par l'utilisateur et une nouvelle ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | le nom de fichier à utiliser lors de la recréation des données décodées |
| newLine | java.lang.String | le caractère terminant chaque ligne |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


Initialise les options avec le nom de fichier fourni par l'utilisateur et la nouvelle ligne par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | le nom de fichier à utiliser lors de la recréation des données décodées |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Obtient le nom de fichier à utiliser lors de la recréation des données décodées.

**Returns:**
java.lang.String - le nom de fichier à utiliser lors de la recréation des données décodées
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


Obtient le caractère terminant chaque ligne, généralement "\n" ou "\r\n".

**Returns:**
java.lang.String - le caractère terminant chaque ligne, généralement "\\n" ou "\\r\\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


Obtient les permissions Unix du fichier.

La valeur par défaut est 644.

**Returns:**
java.lang.String - les autorisations Unix du fichier
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


Définit les autorisations Unix du fichier.

La valeur par défaut est 644.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | les autorisations Unix du fichier |

