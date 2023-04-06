---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP لمرجع .NET API
description: SevenZipLZMA2CompressionSettings البناء. يثبّت إعدادات طريقة ضغط LZMA2 داخل أرشيف 7z .
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

يثبّت إعدادات طريقة ضغط LZMA2 داخل أرشيف 7z .

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| dictionarySize | Int32 | يجب أن يكون حجم مخزن المحفوظات المؤقت بين 4096 و 1073741824. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* كبير جدًا أو صغير جدًا. |

### ملاحظات

كلما كان القاموس أكبر ، كانت نسبة الضغط أفضل عادةً ، لكن القواميس الأكبر من البيانات غير المضغوطة تضيع ذاكرة الوصول العشوائي.

### أنظر أيضا

* class [SevenZipLZMA2CompressionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* المجسم [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

يثبّت إعدادات طريقة ضغط LZMA2 داخل أرشيف 7z .

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| dictionarySize | Int32 | يجب أن يكون حجم مخزن المحفوظات المؤقت بين 4096 و 1073741824. |
| fastBytes | Int32 | يتحكم في عدد البايتات السريعة التي تستخدمها ضواغط LZMA2. يمكن أن يوفر عدد أكبر من البايتات السريعة نسبة ضغط أفضل على حساب سرعة الضغط. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* كبير جدًا أو صغير جدًا ، أو*fastBytes* كبير جدًا أو صغير جدًا. |

### ملاحظات

كلما كان القاموس أكبر ، كانت نسبة الضغط أفضل عادةً ، لكن القواميس الأكبر من البيانات غير المضغوطة تضيع ذاكرة الوصول العشوائي.

### أنظر أيضا

* class [SevenZipLZMA2CompressionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* المجسم [Aspose.Zip](../../../)


