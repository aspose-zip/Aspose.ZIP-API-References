---
title: "SevenZipEncryptionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Classe base per le impostazioni di diversi metodi di crittografia 7z."
type: docs
weight: 112
url: /it/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

Classe base per le impostazioni di diversi metodi di crittografia 7z.

L'AES-256 è l'unico metodo di crittografia possibile per gli archivi 7z. Quindi il [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) è l'unica implementazione.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | Ottiene un valore che indica la crittografia dell'intestazione. |
| [getPassword()](#getPassword--) | Ottiene la password per la crittografia o la decrittazione. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | Imposta un valore che indica la crittografia dell'intestazione. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Imposta la password per la crittografia o la decrittazione. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


Ottiene un valore che indica la crittografia dell'intestazione.

Questa impostazione è equivalente all'opzione `-mhe=on` dello strumento 7-Zip. Attualmente, è incompatibile con la compressione dell'intestazione.

**Returns:**
boolean - un valore che indica la crittografia dell'intestazione
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Ottiene la password per la crittografia o la decrittazione.

**Returns:**
java.lang.String - password per la crittografia o la decrittazione
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


Imposta un valore che indica la crittografia dell'intestazione.

Questa impostazione è equivalente all'opzione `-mhe=on` dello strumento 7-Zip. Attualmente, è incompatibile con la compressione dell'intestazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica la crittografia dell'intestazione |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Imposta la password per la crittografia o la decrittazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | password per la crittografia o la decrittazione |

