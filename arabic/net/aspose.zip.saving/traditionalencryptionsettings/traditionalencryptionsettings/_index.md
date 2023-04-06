---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Aspose.ZIP لمرجع .NET API
description: TraditionalEncryptionSettings البناء. يقوم بتهيئة مثيل جديد لملفTraditionalEncryptionSettings فئة .
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`TraditionalEncryptionSettings`](../) فئة .

```csharp
public TraditionalEncryptionSettings(string password)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| password | String | كلمة السر للتشفير. |

### أمثلة

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### أنظر أيضا

* class [TraditionalEncryptionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* المجسم [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`TraditionalEncryptionSettings`](../) فئة مع ترميز يحدده المستخدم.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| password | String | كلمة السر للتشفير. |
| encoding | Encoding | ترميز أحرف كلمة المرور. |

### ملاحظات

استخدام هذا المنشئ غير مستحسن. قد يتعارض إعداد الترميز مع المعيار وينتج أرشيفًا غير متوافق.

### أمثلة

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### أنظر أيضا

* class [TraditionalEncryptionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* المجسم [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`TraditionalEncryptionSettings`](../)فئة بدون كلمة مرور.

```csharp
public TraditionalEncryptionSettings()
```

### أنظر أيضا

* class [TraditionalEncryptionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* المجسم [Aspose.Zip](../../../)


