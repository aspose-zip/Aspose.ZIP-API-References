---
title: "AlzArchiveLoadOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры, с помощью которых архив ALZ загружается из сжатого файла."
type: docs
weight: 12
url: /ru/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

Параметры, с помощью которых архив ALZ загружается из сжатого файла.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Получает пароль, используемый для расшифровки записей. |
| [getEncoding()](#getEncoding--) | Получает кодировку, используемую для имён записей. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Получает, пропускается ли проверка контрольной суммы записей ALZ. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Устанавливает флаг отмены, используемый для прерывания извлечения. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Устанавливает пароль, используемый для расшифровки записей. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Устанавливает кодировку, используемую для имён записей. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Устанавливает, пропускается ли проверка контрольной суммы записей ALZ. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Получает пароль, используемый для расшифровки записей.

**Returns:**
java.lang.String — пароль, используемый для расшифровки записей, или `null`, если не настроен.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Получает кодировку, используемую для имён записей. По умолчанию используется корейская кодовая страница Windows 949 (CP949). Архивы ALZ исторически хранят имена файлов, используя корейскую ANSI‑кодировку Windows.

**Returns:**
java.nio.charset.Charset — кодировка, используемая для имён записей
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


Получает, пропускается ли проверка контрольной суммы записей ALZ. По умолчанию `false`.

**Returns:**
boolean — пропускается ли проверка контрольной суммы
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Устанавливает флаг отмены, используемый для прерывания извлечения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | флаг отмены, или `null` для отключения отмены |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Устанавливает пароль, используемый для расшифровки записей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | пароль, используемый для расшифровки записей |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Устанавливает кодировку, используемую для имён записей. Архивы ALZ исторически хранят имена файлов, используя корейскую ANSI‑кодировку Windows.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.nio.charset.Charset | кодировка, используемая для имён записей |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


Устанавливает, пропускается ли проверка контрольной суммы записей ALZ.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | пропускается ли проверка контрольной суммы |

