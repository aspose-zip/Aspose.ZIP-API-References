---
title: "ZipDataDescriptorPolicy"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options pour la présence du Data Descriptor."
type: docs
weight: 171
url: /fr/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Options pour la présence du Data Descriptor.
## Champs

| Champ | Description |
| --- | --- |
| [Always](#Always) | Le Data Descriptor est toujours présent pour toutes les entrées zip. |
| [ForAllFileEntries](#ForAllFileEntries) | Le Data Descriptor est présent uniquement pour les entrées contenant des données de fichier ; il est omis pour les répertoires. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Le Data Descriptor est toujours présent pour toutes les entrées zip.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Le Data Descriptor est présent uniquement pour les entrées contenant des données de fichier ; il est omis pour les répertoires. L'utilisation de cette option est découragée.

Ne peut être appliqué qu'aux archives non chiffrées.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
