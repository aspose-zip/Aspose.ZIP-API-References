---
title: "TarArchive"
second_title: "Aspose.Zip for Python via .NET مرجع API"
description: 
type: docs
weight: 10
url: /ar/python-net/aspose.zip.tar/tararchive/
---

## TarArchive class

هذه الفئة تمثل ملف أرشيف tar. استخدمها لإنشاء أو استخراج أو تحديث أرشيفات tar.

يعرض نوع TarArchive الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| TarArchive() | يُهيئ مثيلاً جديدًا من الفئة [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) . |
| TarArchive(source_stream) | ينشئ مثيلًا جديدًا من الفئة [Archive](/zip/python-net/aspose.zip/archive/) ويُكوّن قائمة عناصر يمكن استخراجها من الأرشيف. |
| TarArchive(path) | يُهيئ مثيلاً جديدًا من الفئة [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) ويُنشئ قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| entries | يحصل على إدخالات من نوع [TarEntry](/zip/python-net/aspose.zip.tar/tarentry/) التي تُكوّن الأرشيف. |
| file_entries | يسترجع الإدخالات من نوع [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) التي تشكل الأرشيف. |
| الصيغة | يحصل على صيغة الأرشيف. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| create_entry(name, source, file_info) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, file_info, open_immediately) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entry(name, path, open_immediately) | إنشاء إدخال واحد داخل الأرشيف. |
| create_entries(directory, include_root_directory) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المحدد. |
| create_entries(source_directory, include_root_directory) | يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المحدد. |
| delete_entry(entry) | يزيل أول ظهور لإدخال محدد من قائمة الإدخالات. |
| delete_entry(entry_index) |  |
| save(output, format) |  |
| save(destination_file_name, format) |  |
| save_gzipped(output, format) |  |
| save_gzipped(path, format) |  |
| save_zstandard(output, format) |  |
| save_zstandard(path, format) |  |
| save_lzipped(output, format) |  |
| save_lzipped(path, format) |  |
| save_lzma_compressed(output, format) |  |
| save_lzma_compressed(path, format) |  |
| save_lz4_compressed(output, format) |  |
| save_lz4_compressed(path, format) |  |
| save_xz_compressed(output, format, settings) |  |
| save_xz_compressed(path, format, settings) |  |
| save_z_compressed(output, format) |  |
| save_z_compressed(path, format) |  |
| from_g_zip(source) | يستخرج الأرشيف gzip المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_g_zip(path) | يستخرج الأرشيف gzip المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_zstandard(source) | يستخرج الأرشيف Zstandard المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_zstandard(path) | يستخرج الأرشيف Zstandard المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_l_zip(source) | يستخرج الأرشيف lzip المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_l_zip(path) | يستخرج الأرشيف lzip المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_lzma(source) | يستخرج الأرشيف LZMA المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_lzma(path) | يستخرج الأرشيف LZMA المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_lz4(path) | يستخرج الأرشيف LZ4 المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_lz4(source) | يستخرج الأرشيف LZ4 المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_xz(source) | يستخرج الأرشيف بصيغة xz المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_xz(path) | يستخرج الأرشيف بصيغة xz المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_z(source) | يستخرج الأرشيف Zstandard المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| from_z(path) | يستخرج الأرشيف Zstandard المقدم ويكوّن [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) من البيانات المستخرجة. |
| extract_to_directory(destination_directory) | يستخرج جميع الملفات في الأرشيف إلى الدليل المقدم. |

### انظر أيضًا

* namespace [aspose.zip.tar](/zip/python-net/aspose.zip.tar/)
* assembly [Aspose.Zip](/zip/python-net/)

