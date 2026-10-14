---
title: "Archive"
second_title: "Aspose.Zip for Python via .NET مرجع API"
description: 
type: docs
weight: 10
url: /ar/python-net/aspose.zip/archive/
---

## Archive class

هذه الفئة تمثل ملف أرشيف zip. استخدمها لإنشاء أو استخراج أو تحديث أرشيفات zip.

نوع Archive يعرض الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| Archive(new_entry_settings) | ينشئ مثيلًا جديدًا من الفئة [Archive](/zip/python-net/aspose.zip/archive/) مع إعدادات اختيارية لعناصره. |
| Archive(source_stream, load_options, new_entry_settings) | ينشئ مثيلًا جديدًا من الفئة [Archive](/zip/python-net/aspose.zip/archive/) ويُكوّن قائمة عناصر يمكن استخراجها من الأرشيف. |
| Archive(path, load_options, new_entry_settings) | ينشئ مثيلًا جديدًا من الفئة [Archive](/zip/python-net/aspose.zip/archive/) ويُكوّن قائمة عناصر يمكن استخراجها من الأرشيف. |
| Archive(main_segment, segments_in_order, load_options) | يُنشئ مثيلاً جديدًا من الفئة [Archive](/zip/python-net/aspose.zip/archive/) من أرشيف ZIP متعدد الأحجام ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| new_entry_settings | إعدادات الضغط والتشفير المستخدمة للعناصر [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/) المضافة حديثًا. |
| comment | يحصل على التعليق الخاص بالأرشيف بأكمله. |
| entries | يحصل على إدخالات من نوع [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/) التي تشكل الأرشيف. |
| file_entries | يسترجع الإدخالات من نوع [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) التي تشكل الأرشيف. |
| الصيغة | يحصل على صيغة الأرشيف. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| create_entry(name, path, open_immediately, new_entry_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, source, new_entry_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, file_info, open_immediately, new_entry_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, source, new_entry_settings, file_info) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entries(directory, include_root_directory) | إضافة جميع الملفات والدلائل إلى الأرشيف بشكل متكرر داخل الدليل المحدد. |
| create_entries(source_directory, include_root_directory) | إضافة جميع الملفات والدلائل إلى الأرشيف بشكل متكرر داخل الدليل المحدد. |
| delete_entry(entry) | يزيل أول ظهور للإدخال المحدد من قائمة الإدخالات. |
| delete_entry(entry_index) |  |
| save(output_stream, save_options) | يحفظ الأرشيف إلى الدفق المقدم. |
| save(destination_file_name, save_options) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| save_split(destination_directory, options) | يحفظ الأرشيف متعدد الأحجام إلى دليل الوجهة المقدم. |
| extract_to_directory(destination_directory) | يستخرج جميع الملفات في الأرشيف إلى الدليل المقدم. |

### انظر أيضًا

* namespace [aspose.zip](/zip/python-net/aspose.zip/)
* assembly [Aspose.Zip](/zip/python-net/)

