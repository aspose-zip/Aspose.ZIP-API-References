---
title: "AlzArchiveLoadOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni con cui un archivio ALZ viene caricato da un file compresso."
type: docs
weight: 12
url: /it/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

Opzioni con cui un archivio ALZ viene caricato da un file compresso.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Ottiene la password usata per decrittare le voci. |
| [getEncoding()](#getEncoding--) | Ottiene la codifica usata per i nomi delle voci. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Ottiene se la verifica del checksum delle voci ALZ è saltata. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Imposta un flag di cancellazione usato per annullare l'estrazione. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Imposta la password usata per decrittare le voci. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Imposta la codifica usata per i nomi delle voci. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Imposta se la verifica del checksum delle voci ALZ è saltata. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Ottiene la password usata per decrittare le voci.

**Returns:**
java.lang.String - password usata per decrittare le voci, o `null` quando non è configurata
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Ottiene la codifica usata per i nomi delle voci. Il valore predefinito è la pagina di codice Windows coreana 949 (CP949). Gli archivi ALZ memorizzano storicamente i nomi dei file usando la pagina di codice ANSI di Windows coreano.

**Returns:**
java.nio.charset.Charset - codifica usata per i nomi delle voci
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


Ottiene se la verifica del checksum delle voci ALZ è saltata. Il valore predefinito è `false`.

**Returns:**
boolean - se la verifica del checksum è saltata
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Imposta un flag di cancellazione usato per annullare l'estrazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | flag di cancellazione, o `null` per disabilitare la cancellazione |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Imposta la password usata per decrittare le voci.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | password usata per decrittare le voci |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Imposta la codifica usata per i nomi delle voci. Gli archivi ALZ memorizzano storicamente i nomi dei file usando la pagina di codice ANSI di Windows coreano.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.nio.charset.Charset | codifica usata per i nomi delle voci |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


Imposta se la verifica del checksum delle voci ALZ è saltata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | se la verifica del checksum è saltata |

