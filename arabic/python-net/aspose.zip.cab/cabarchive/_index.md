---
title: "CabArchive"
second_title: "Aspose.Zip for Python via .NET مرجع API"
description: 
type: docs
weight: 10
url: /ar/python-net/aspose.zip.cab/cabarchive/
---

## CabArchive class

هذه الفئة تمثل ملف أرشيف CAB.

يعرض نوع CabArchive الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| CabArchive(settings) | يُنشئ مثلاً جديداً من الفئة [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) المُعد للضغط. |
| CabArchive(source_stream, load_options) | يُنشئ مثلاً جديداً من الفئة [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| CabArchive(path, load_options) | يُنشئ مثلاً جديداً من الفئة [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| entries | يحصل على الإدخالات من نوع [CabEntry](/zip/python-net/aspose.zip.cab/cabentry/) التي تُكوّن الأرشيف. |
| file_entries | يسترجع الإدخالات من نوع [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) التي تشكل الأرشيف. |
| الصيغة | يحصل على صيغة الأرشيف. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| create_entry(name, path, new_entry_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, source, new_entry_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, file_info, new_entry_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entries(directory, include_root_directory) | يضيف إلى الأرشيف جميع الملفات، بشكل متكرر، من الدليل المحدد. |
| create_entries(source_directory, include_root_directory) | يضيف إلى الأرشيف جميع الملفات بشكل متكرر من مسار الدليل المحدد. |
| save(output_stream, save_options) | يحفظ الأرشيف إلى الدفق المقدم. |
| save(destination_file_name, save_options) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| extract_to_directory(destination_directory) | يستخرج جميع الملفات في الأرشيف إلى الدليل المقدم. |

### انظر أيضًا

* namespace [aspose.zip.cab](/zip/python-net/aspose.zip.cab/)
* assembly [Aspose.Zip](/zip/python-net/)

