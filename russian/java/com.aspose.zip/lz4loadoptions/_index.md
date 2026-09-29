---
title: "Lz4LoadOptions"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры загрузки ."
type: docs
weight: 82
url: /ru/java/com.aspose.zip/lz4loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Lz4LoadOptions
```

Опции загрузки [Lz4Archive](../../com.aspose.zip/lz4archive).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Lz4LoadOptions()](#Lz4LoadOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Устанавливает флаг отмены, используемый для отмены операции извлечения. |
### Lz4LoadOptions() {#Lz4LoadOptions--}
```
public Lz4LoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Устанавливает флаг отмены, используемый для отмены операции извлечения.

Отменить извлечение lz4-архива после определённого времени.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
Lz4LoadOptions options = new Lz4LoadOptions();
options.setCancellationFlag(cf);
try (Lz4Archive a = new Lz4Archive("big.lz4", options)) {
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

