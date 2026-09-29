---
title: "ZipDataDescriptorPolicy"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni per la presenza del Data Descriptor."
type: docs
weight: 171
url: /it/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Opzioni per la presenza del Data Descriptor.
## Campi

| Campo | Descrizione |
| --- | --- |
| [Always](#Always) | Il Data Descriptor è sempre presente per tutte le voci zip. |
| [ForAllFileEntries](#ForAllFileEntries) | Il Data Descriptor è presente solo per le voci con dati file; omesso per le directory. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Il Data Descriptor è sempre presente per tutte le voci zip.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Il Data Descriptor è presente solo per le voci con dati file; omesso per le directory. L'uso di questa opzione è sconsigliato.

Può essere applicato solo ad archivi non crittografati.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
