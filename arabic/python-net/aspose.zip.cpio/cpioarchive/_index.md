---
title: "CpioArchive"
second_title: "Aspose.Zip for Python via .NET مرجع API"
description: 
type: docs
weight: 10
url: /ar/python-net/aspose.zip.cpio/cpioarchive/
---

## CpioArchive class

هذه الفئة تمثل ملف أرشيف cpio.

يعرض نوع CpioArchive الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| CpioArchive() | ينشئ مثيلاً جديدًا من الفئة [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/). |
| CpioArchive(source_stream) | ينشئ مثيلاً جديدًا من الفئة [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
| CpioArchive(path) | ينشئ مثيلاً جديدًا من الفئة [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) ويُكوّن قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| entries | يحصل على الإدخالات من النوع [CpioEntry](/zip/python-net/aspose.zip.cpio/cpioentry/) التي تشكل الأرشيف. |
| file_entries | يسترجع الإدخالات من نوع [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) التي تشكل الأرشيف. |
| الصيغة | يحصل على صيغة الأرشيف. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| create_entries(source_directory, include_root_directory) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المحدد. |
| create_entries(directory, include_root_directory) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المحدد. |
| create_entry(name, file_info, open_immediately) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, source_path, open_immediately) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, source) | إنشاء إدخال واحد داخل الأرشيف. |
| delete_entry(entry) | يزيل أول ظهور لإدخال محدد من قائمة الإدخالات. |
| delete_entry(entry_index) |  |
| save(destination_file_name, cpio_format) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| save(output, cpio_format) | يحفظ الأرشيف إلى الدفق المقدم. |
| save_gzipped(output, cpio_format) | يحفظ الأرشيف إلى الدفق مع ضغط gzip. |
| save_gzipped(path, cpio_format) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط gzip. |
| save_lzipped(output, cpio_format) | يحفظ الأرشيف إلى الدفق مع ضغط lzip. |
| save_lzipped(path, cpio_format) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط lzip. |
| save_lzma_compressed(output, cpio_format) | يحفظ الأرشيف إلى الدفق مع ضغط LZMA. |
| save_lzma_compressed(path, cpio_format) | يحفظ الأرشيف إلى الملف بالمسار مع ضغط lzma. |
| save_xz_compressed(output, cpio_format, settings) | يحفظ الأرشيف إلى الدفق مع ضغط xz. |
| save_xz_compressed(path, cpio_format, settings) | يحفظ الأرشيف إلى المسار بالمسار مع ضغط xz. |
| save_z_compressed(output, cpio_format) | يحفظ الأرشيف إلى الدفق مع ضغط Z. |
| save_z_compressed(path, cpio_format) | يحفظ الأرشيف إلى المسار باستخدام ضغط Z. |
| save_zstandard(output, cpio_format) | يحفظ الأرشيف إلى الدفق باستخدام ضغط Zstandard. |
| save_zstandard(path, cpio_format) | يحفظ الأرشيف إلى الملف حسب المسار باستخدام ضغط Zstandard. |
| extract_to_directory(destination_directory) | يستخرج جميع الملفات في الأرشيف إلى الدليل المقدم. |

### انظر أيضًا

* namespace [aspose.zip.cpio](/zip/python-net/aspose.zip.cpio/)
* assembly [Aspose.Zip](/zip/python-net/)

