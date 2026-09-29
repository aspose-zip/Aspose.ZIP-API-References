---
title: "TarFormat"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Énumération des formats pris en charge de ."
type: docs
weight: 169
url: /fr/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

Énumération des formats pris en charge de [TarArchive](../../com.aspose.zip/tararchive).
## Champs

| Champ | Description |
| --- | --- |
| [Gnu](#Gnu) | GNU tar est basé sur le premier brouillon de POSIX.1. |
| [Pax](#Pax) | Format défini dans la norme POSIX.1-2001. |
| [UsTar](#UsTar) | Le format étend le bloc d’en-tête du format v7. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar est basé sur le premier brouillon de POSIX.1. Ce format est implémenté comme format tar par défaut dans de nombreux systèmes Linux.

### Pax {#Pax}
```
public static final TarFormat Pax
```


Format défini dans la norme POSIX.1-2001.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


Le format étend le bloc d’en-tête du format v7. Il est largement répandu et pris en charge dans de nombreuses utilitaires pour Windows.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
