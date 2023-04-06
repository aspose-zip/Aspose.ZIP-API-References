---
title: Class SevenZipCipher
second_title: Aspose.ZIP لمرجع .NET API
description: Aspose.Zip.Crypto.SevenZipCipher فصل. الفئة الأساسية لشفرات AES المستخدمة لتشفير 7zip .
type: docs
weight: 190
url: /ar/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

الفئة الأساسية لشفرات AES المستخدمة لتشفير 7-zip .

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## الخصائص

| اسم | وصف |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | يحصل على قيمة تشير إلى إمكانية إعادة استخدام التحويل الحالي. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | يحصل على قيمة تشير إلى إمكانية تحويل الكتل المتعددة. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | الحصول على حجم كتلة الإدخال. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | الحصول على حجم كتلة الإخراج. |

## طُرق

| اسم | وصف |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | تنفيذ مهام محددة بواسطة التطبيق مرتبطة بتحرير الموارد غير المُدارة أو تحريرها أو إعادة تعيينها. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | تحويل المنطقة المحددة لصفيف بايت الإدخال ونسخ التحويل الناتج إلى المنطقة المحددة لصفيف بايت الإخراج. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | يحول المنطقة المحددة لصفيف البايت المحدد. |

### أنظر أيضا

* مساحة الاسم [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* المجسم [Aspose.Zip](../../)


