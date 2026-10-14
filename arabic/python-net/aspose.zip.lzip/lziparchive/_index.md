---
title: "LzipArchive"
second_title: "Aspose.Zip for Python via .NET مرجع API"
description: 
type: docs
weight: 10
url: /ar/python-net/aspose.zip.lzip/lziparchive/
---

## LzipArchive class

هذه الفئة تمثل ملف أرشيف Lzip. استخدمها لإنشاء أو استخراج أرشيفات Lzip.

يعرض نوع LzipArchive الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| LzipArchive(settings) | ينشئ مثيلاً جديداً من [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/). |
| LzipArchive(source_stream, options) | ينشئ مثيلاً جديداً من الفئة [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/) المُعد لفك الضغط. |
| LzipArchive(path, options) | ينشئ مثيلاً جديداً من الفئة [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/) المُعد لفك الضغط. |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| uncompressed_size | الحجم غير المضغوط لبيانات الملف بالبايت. |
| settings | يحصل على إعداد أرشيف lzip معين. |
| file_entries | يسترجع الإدخالات من نوع [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) التي تشكل الأرشيف. |
| الصيغة | يحصل على صيغة الأرشيف. |
| name | يحصل على اسم العنصر. |
| length | يحصل على طول العنصر بالبايت. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| extract(destination) | يستخرج أرشيف lzip إلى تدفق. |
| extract(file_info) | يستخرج أرشيف lzip إلى ملف. |
| extract(path) | يستخرج أرشيف lzip إلى ملف حسب المسار. |
| save(output_stream) | يحفظ أرشيف lzip إلى الدفق المقدم. |
| save(destination_file_name) | يحفظ أرشيف lzip إلى ملف الوجهة المقدم. |
| save(destination) | يحفظ أرشيف lzip إلى ملف الوجهة المقدم. |
| set_source(source) | يضبط المحتوى لضغطه داخل الأرشيف. |
| set_source(file_info) | يضبط المحتوى لضغطه داخل الأرشيف. |
| set_source(path) | يضبط المحتوى لضغطه داخل الأرشيف. |
| extract_to_directory(destination_directory) | يستخرج محتوى الأرشيف إلى الدليل المقدم. |

### انظر أيضًا

* namespace [aspose.zip.lzip](/zip/python-net/aspose.zip.lzip/)
* assembly [Aspose.Zip](/zip/python-net/)

