---
title: "XzLoadOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры загрузки ."
type: docs
weight: 152
url: /ru/java/com.aspose.zip/xzloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XzLoadOptions
```

Параметры загрузки [XzArchive](../../com.aspose.zip/xzarchive).

В .NET Framework 4.0 и выше может использоваться для отмены извлечения.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [XzLoadOptions()](#XzLoadOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Устанавливает флаг отмены, используемый для отмены операции извлечения. |
### XzLoadOptions() {#XzLoadOptions--}
```
public XzLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Устанавливает флаг отмены, используемый для отмены операции извлечения.

Отменить извлечение lzip-архива после определённого времени.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
XzLoadOptions options = new XzLoadOptions();
options.setCancellationFlag(cf);
try (XzArchive a = new XzArchive(\"big.xz\", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println(\"Extraction was cancelled after 60 seconds\");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

