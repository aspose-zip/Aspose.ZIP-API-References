---
title: AlzArchiveLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which an ALZ archive is loaded from a compressed file.
type: docs
weight: 12
url: /java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

Options with which an ALZ archive is loaded from a compressed file.
## Constructors

| Constructor | Description |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Gets the password used to decrypt entries. |
| [getEncoding()](#getEncoding--) | Gets the encoding used for entry names. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Gets whether checksum verification of ALZ entries is skipped. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel extraction. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Sets the password used to decrypt entries. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Sets the encoding used for entry names. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Sets whether checksum verification of ALZ entries is skipped. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Gets the password used to decrypt entries.

**Returns:**
java.lang.String - password used to decrypt entries, or `null` when none is configured
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Gets the encoding used for entry names. The default is Korean Windows code page 949 (CP949). ALZ archives historically store file names using the Korean Windows ANSI code page.

**Returns:**
java.nio.charset.Charset - encoding used for entry names
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


Gets whether checksum verification of ALZ entries is skipped. The default is `false`.

**Returns:**
boolean - whether checksum verification is skipped
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | cancellation flag, or `null` to disable cancellation |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Sets the password used to decrypt entries.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | password used to decrypt entries |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets the encoding used for entry names. ALZ archives historically store file names using the Korean Windows ANSI code page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.nio.charset.Charset | encoding used for entry names |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


Sets whether checksum verification of ALZ entries is skipped.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | whether checksum verification is skipped |

