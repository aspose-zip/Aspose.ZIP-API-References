---
title: "Olay"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bir olay."
type: docs
weight: 160
url: /tr/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

Bir olay.

`TArgs`: olay argümanları.

TArgs :
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Bu yöntem, olay yayılınca çağrılır. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Bu yöntem, olay yayılınca çağrılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| gönderici | java.lang.Object | bu olayı başlatan bir nesne. |
| argümanlar | TArgs | özel argümanlar. |

