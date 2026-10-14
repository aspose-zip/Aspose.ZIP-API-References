---
title: "IsoArchive"
second_title: "Aspose.Zip for Python via .NET مرجع API"
description: 
type: docs
weight: 30
url: /ar/python-net/aspose.zip.iso/isoarchive/
---

## IsoArchive class

يمثل أرشيف ISO (ISO 9660).

يعرض نوع IsoArchive الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| IsoArchive() | يقوم بإنشاء نسخة جديدة من الفئة [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) ويُنشئ أرشيف ISO فارغ<br/> لإضافة ملفات ودلائل جديدة. |
| IsoArchive(source_stream, load_options) | يقوم بإنشاء نسخة جديدة من الفئة [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) ويُنشئ قائمة إدخالات يمكن استخراجها من الأرشيف. |
| IsoArchive(path, load_options) | يقوم بإنشاء نسخة جديدة من الفئة [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) ويُنشئ قائمة إدخالات يمكن استخراجها من الأرشيف. |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| entries | يسترجع الإدخالات من نوع [IsoEntry](/zip/python-net/aspose.zip.iso/isoentry/) التي تشكل الأرشيف. |
| file_entries | يسترجع الإدخالات من نوع [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) التي تشكل الأرشيف. |
| الصيغة | يحصل على صيغة الأرشيف. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| create_entry(name, file_path) | يضيف ملفًا إلى صورة ISO. |
| create_entry(name, source) | يضيف ملفًا إلى صورة ISO. |
| create_entry(name) | يضيف ملفًا إلى صورة ISO. |
| save(path, save_options) | يحفظ صورة ISO إلى المسار المحدد. |
| save(stream, save_options) | يحفظ صورة ISO إلى الدفق المحدد. |
| create_directory(name) | يضيف دليلًا إلى صورة ISO. |
| extract_to_directory(destination_directory) | يستخرج جميع الإدخالات إلى الدليل المحدد. |

### انظر أيضًا

* namespace [aspose.zip.iso](/zip/python-net/aspose.zip.iso/)
* assembly [Aspose.Zip](/zip/python-net/)

