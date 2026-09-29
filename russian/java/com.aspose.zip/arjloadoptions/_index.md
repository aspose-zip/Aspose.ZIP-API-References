---
title: "ArjLoadOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры, с помощью которых архив загружается из сжатого файла."
type: docs
weight: 39
url: /ru/java/com.aspose.zip/arjloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArjLoadOptions
```

Параметры, с помощью которых архив загружается из сжатого файла.

В .NET Framework 4.0 и выше может использоваться для отмены извлечения.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ArjLoadOptions()](#ArjLoadOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Устанавливает флаг отмены, используемый для отмены операции извлечения. |
### ArjLoadOptions() {#ArjLoadOptions--}
```
public ArjLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Устанавливает флаг отмены, используемый для отмены операции извлечения.

Отменить извлечение ARJ‑архива после определённого времени.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
ArjLoadOptions options = new ArjLoadOptions();
options.setCancellationFlag(cf);
try (ArjArchive a = new ArjArchive("big.arj", options)) {
try {
a.getEntries().get(0).extract("data.bin");
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

