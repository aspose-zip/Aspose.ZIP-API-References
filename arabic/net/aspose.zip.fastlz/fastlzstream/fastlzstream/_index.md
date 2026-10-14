---
title: "FastLZStream.FastLZStream"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "منشئ FastLZStream. يهيئ نسخة جديدة من الفئة FastLZStream المُعدة للضغط"
type: docs
weight: 10
url: /ar/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

يهيئ نسخة جديدة من الفئة [`FastLZStream`](../) المُعدة للضغط.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تيار | تيار | التيار لحفظ البيانات المضغوطة. |
| compressionLevel | Int32 | استخدم 1 لضغط أسرع، واستخدم 2 لنسبة ضغط أفضل. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *stream* فارغ. |
| ArgumentException | *stream* لا يدعم الكتابة. |
| ArgumentOutOfRangeException | *compressionLevel* أكبر من 2 أو أصغر من 1. |

### انظر أيضًا

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


