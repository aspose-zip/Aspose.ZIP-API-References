---
title: "SevenZipArchive"
second_title: "Aspose.Zip for Python via .NET مرجع API"
description: 
type: docs
weight: 10
url: /ar/python-net/aspose.zip.sevenzip/sevenziparchive/
---

## SevenZipArchive class

هذه الفئة تمثل ملف أرشيف 7z. استخدمها لإنشاء واستخراج أرشيفات 7z.

يعرض نوع SevenZipArchive الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| SevenZipArchive(new_entry_settings) | ينشئ مثيلًا جديدًا للفئة [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) مع إعدادات اختيارية لمدخلاتها. |
| SevenZipArchive(source_stream, password) | ينشئ مثيلًا جديدًا للفئة [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف. |
| SevenZipArchive(path, password) | ينشئ مثيلًا جديدًا للفئة [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف. |
| SevenZipArchive(source_stream, options) | ينشئ مثيلًا جديدًا للفئة [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف. |
| SevenZipArchive(path, options) | ينشئ مثيلًا جديدًا للفئة [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف. |
| SevenZipArchive(parts, password) | ينشئ مثيلًا جديدًا للفئة [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) من أرشيف 7z متعدد الأحجام ويكوّن قائمة مدخلات يمكن استخراجها من الأرشيف. |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| new_entry_settings | إعدادات الضغط والتشفير المستخدمة للعناصر [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) المضافة حديثًا. |
| entries | يحصل على المدخلات من نوع [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) التي تشكل الأرشيف. |
| file_entries | يسترجع الإدخالات من نوع [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) التي تشكل الأرشيف. |
| الصيغة | يحصل على صيغة الأرشيف. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| create_entry(name, file_info, open_immediately, new_entry_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, source, new_entry_settings, file_info) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, source, new_entry_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, path, open_immediately, new_entry_settings) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entries(directory, include_root_directory) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر داخل الدليل المعطى. |
| create_entries(source_directory, include_root_directory) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر داخل الدليل المعطى. |
| save(output, save_options) | يحفظ أرشيف 7z إلى الدفق المقدم. |
| save(destination_file_name, save_options) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| extract_to_directory(destination_directory, password) | يستخرج جميع الملفات في الأرشيف إلى الدليل المقدم. |
| extract_to_directory(destination_directory) | يستخرج جميع الملفات في الأرشيف إلى الدليل المقدم. |
| save_split(destination_directory, options) | يحفظ الأرشيف متعدد الأحجام إلى دليل الوجهة المقدم. |

### انظر أيضًا

* namespace [aspose.zip.sevenzip](/zip/python-net/aspose.zip.sevenzip/)
* assembly [Aspose.Zip](/zip/python-net/)

