---
title: "GzipArchive"
second_title: "Aspose.Zip for Python via .NET مرجع API"
description: 
type: docs
weight: 10
url: /ar/python-net/aspose.zip.gzip/gziparchive/
---

## GzipArchive class

هذه الفئة تمثل ملف أرشيف gzip. استخدمها لإنشاء أو استخراج أرشيفات gzip.

يُظهر نوع GzipArchive الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| GzipArchive() | يُنشئ مثلاً جديدًا من الفئة [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) المُعدة للضغط. |
| GzipArchive(source_stream, parse_header) | يُنشئ مثلاً جديدًا من الفئة [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) المُعدة للفك. |
| GzipArchive(source_stream, options) | يُنشئ مثلاً جديدًا من الفئة [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) المُعدة للفك. |
| GzipArchive(path, options) | يُنشئ مثلاً جديدًا من الفئة [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) المُعدة للفك. |
| GzipArchive(path, parse_header) | يُنشئ مثلاً جديدًا من الفئة [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) المُعدة للفك. |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| uncompressed_size | يحصل على حجم الملف الأصلي. |
| name | اسم الملف الأصلي. |
| file_entries | يسترجع الإدخالات من نوع [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) التي تشكل الأرشيف. |
| الصيغة | يحصل على صيغة الأرشيف. |
| length | يحصل على طول العنصر بالبايت. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| set_source(source) | يضبط المحتوى لضغطه داخل الأرشيف. |
| set_source(file_info) | يضبط المحتوى لضغطه داخل الأرشيف. |
| set_source(path) | يضبط المحتوى لضغطه داخل الأرشيف. |
| set_source(tar_archive) | يضبط المحتوى لضغطه داخل الأرشيف. |
| extract(destination) | يستخرج الأرشيف إلى الدفق المقدم. |
| extract(path) | يستخرج محتوى الأرشيف إلى الدليل المقدم. |
| save(output_stream) | يحفظ الأرشيف إلى الدفق المقدم. |
| save(destination_file_name) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| open() | يفتح الأرشيف للاستخراج ويوفر تدفقًا بمحتوى الأرشيف. |
| extract_to_directory(destination_directory) | يستخرج محتوى الأرشيف إلى الدليل المقدم. |

### انظر أيضًا

* namespace [aspose.zip.gzip](/zip/python-net/aspose.zip.gzip/)
* assembly [Aspose.Zip](/zip/python-net/)

