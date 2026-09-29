---
title: "Peristiwa"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Sebuah peristiwa."
type: docs
weight: 160
url: /id/java/com.aspose.zip/event/
---
```
public interface Event<TArgs>
```

Sebuah peristiwa.

`TArgs`: argumen peristiwa.

TArgs :
## Metode

| Metode | Deskripsi |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Metode ini dipanggil ketika peristiwa dipancarkan. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Metode ini dipanggil ketika peristiwa dipancarkan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pengirim | java.lang.Object | sebuah objek yang memulai peristiwa ini. |
| argumen | TArgs | argumen khusus. |

