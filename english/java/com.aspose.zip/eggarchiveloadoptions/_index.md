---
title: EggArchiveLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which an EGG archive is loaded from a compressed file.
type: docs
weight: 60
url: /java/com.aspose.zip/eggarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class EggArchiveLoadOptions
```

Options with which an EGG archive is loaded from a compressed file.
## Constructors

| Constructor | Description |
| --- | --- |
| [EggArchiveLoadOptions()](#EggArchiveLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Gets the password used to decrypt encrypted EGG entry contents. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel extraction operations. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Sets the password used to decrypt encrypted EGG entry contents. |
### EggArchiveLoadOptions() {#EggArchiveLoadOptions--}
```
public EggArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Gets the password used to decrypt encrypted EGG entry contents.

**Returns:**
java.lang.String - The decryption password, or `null` if no password was specified.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public final void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel extraction operations.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | cancellation flag. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Sets the password used to decrypt encrypted EGG entry contents.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The decryption password. |

