---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP لمرجع .NET API
description: SevenZipPPMdCompressionSettings البناء. يثبّت إعدادات طريقة ضغط PPMd داخل أرشيف 7z.
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

يثبّت إعدادات طريقة ضغط PPMd داخل أرشيف 7z.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| maxOrder | Byte | الحد الأقصى للطلب. |
| suballocatorSize | Int32 | قد يتم استهلاك حجم الذاكرة بالميجابايت الفرعي. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* ليس بين 2 و 32 ، أو*suballocatorSize* ليس بين 1 و 1024. |

### ملاحظات

تؤدي طلبات النماذج الأكبر بشكل شبه مؤكد إلى ضغط أفضل واستخدام ذاكرة أكبر ووحدة المعالجة المركزية بالتأكيد.

قد تحتاج خوارزمية PPMd إلى قدر كبير من الذاكرة ، خاصة عند استخدامها في ملفات كبيرة و / أو استخدامها بترتيب طراز كبير . إذا احتاج ppmd إلى ذاكرة أكبر مما تعطيه ، فسيكون الضغط أسوأ.

### أمثلة

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### أنظر أيضا

* class [SevenZipPPMdCompressionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* المجسم [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

يتم إنشاء إعدادات طريقة ضغط PPMd داخل أرشيف 7z بترتيب النموذج الافتراضي وحجم المخصص الفرعي.

```csharp
public SevenZipPPMdCompressionSettings()
```

### ملاحظات

ترتيب النموذج الافتراضي هو 6 وحجم المخصص الفرعي هو 16 ميجا بايت .

### أمثلة

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### أنظر أيضا

* class [SevenZipPPMdCompressionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* المجسم [Aspose.Zip](../../../)


