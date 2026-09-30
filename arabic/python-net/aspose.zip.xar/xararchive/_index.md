---
title: "XarArchive"
second_title: "Aspose.Zip for Python via .NET مرجع API"
description: 
type: docs
weight: 40
url: /ar/python-net/aspose.zip.xar/xararchive/
---

## XarArchive class

هذه الفئة تمثل ملف أرشيف xar.

يعرض نوع XarArchive الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| XarArchive(default_compression_settings) | ينشئ مثلاً جديدًا من الفئة [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) class. |
| XarArchive(source_stream, load_options) | ينشئ مثلاً جديدًا من الفئة [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) class ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| XarArchive(path, load_options) | ينشئ مثلاً جديدًا من الفئة [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) class ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| entries | يحصل على الإدخالات من النوع [XarEntry](/zip/python-net/aspose.zip.xar/xarentry/) التي تشكل الأرشيف. |
| file_entries | يسترجع الإدخالات من نوع [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) التي تشكل الأرشيف. |
| الصيغة | يحصل على صيغة الأرشيف. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| create_entries(source_directory, include_root_directory, compression_settings) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المحدد. |
| create_entries(directory, include_root_directory, compression_settings) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المحدد. |
| create_entry(name, file_info, open_immediately, compression_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, source_path, open_immediately, compression_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, source, compression_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| save(destination_file_name, save_options) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| save(output, save_options) | يحفظ الأرشيف إلى الدفق المقدم. |
| extract_to_directory(destination_directory) | يستخرج جميع الملفات في الأرشيف إلى الدليل المقدم. |
| delete_entry(entry) | يزيل أول ظهور لإدخال محدد من قائمة الإدخالات. |

### انظر أيضًا

* namespace [aspose.zip.xar](/zip/python-net/aspose.zip.xar/)
* assembly [Aspose.Zip](/zip/python-net/)

