---
title: "इवेंट"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "एक इवेंट।"
type: docs
weight: 160
url: /hi/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

एक इवेंट।

`TArgs`: इवेंट तर्क।

TArgs :
## Methods

| Method | विवरण |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | यह विधि तब बुलाई जाती है जब इवेंट उत्सर्जित होता है। |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


यह विधि तब बुलाई जाती है जब इवेंट उत्सर्जित होता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रेषक | java.lang.Object | एक वस्तु जो इस इवेंट को शुरू करती है। |
| तर्क | TArgs | कस्टम तर्क। |

