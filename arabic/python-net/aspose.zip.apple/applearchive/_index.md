---
title: "AppleArchive"
second_title: "Aspose.Zip for Python via .NET مرجع API"
description: 
type: docs
weight: 10
url: /ar/python-net/aspose.zip.apple/applearchive/
---

## AppleArchive class

هذه الفئة تمثل ملف Apple Archive (.aar). استخدمها لإنشاء ملفات Apple Archive.

يعرض نوع AppleArchive الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| AppleArchive(new_entry_settings) | يُهيئ مثلاً جديداً من فئة [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) مع الإعدادات المستخدمة للمدخلات المركبة. |
| AppleArchive(source_stream, load_options) | يُهيئ مثلاً جديداً من فئة [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) ويُنشئ قائمة مدخلات يمكن استخراجها من الأرشيف. |
| AppleArchive(path, load_options) | يُهيئ مثلاً جديداً من فئة [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) ويُنشئ قائمة مدخلات يمكن استخراجها من الأرشيف. |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| المدخلات | يحصل على المدخلات التي تشكل الأرشيف. |
| is_solid | يحصل على قيمة تشير إلى ما إذا كان الأرشيف يستخدم ضغطًا صلبًا.<br/>            في الوضع الصلب، يتم ضغط جميع بيانات الإدخالات كتيار واحد و<br/>            لا يتوفر استخراج إدخال فردي. استخدم |
| new_entry_settings | يحصل على الإعدادات المستخدمة للإدخالات التي تم إنشاؤها حديثًا. |
| file_entries | يسترجع الإدخالات من نوع [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) التي تشكل الأرشيف. |
| الصيغة | يحصل على صيغة الأرشيف. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| create_entry(name, path, open_immediately) | ينشئ إدخالًا واحدًا داخل الأرشيف. |
| create_entry(name, source) | ينشئ إدخالًا واحدًا داخل الأرشيف. |
| create_entry(name, file_info, open_immediately) | ينشئ إدخالًا واحدًا داخل الأرشيف. |
| save(output) | يحفظ الأرشيف إلى الدفق المقدم. |
| save(destination_file_name) | يحفظ الأرشيف إلى ملف الوجهة المقدم. |
| create_entries(directory, include_root_directory) | يضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر داخل الدليل المعطى. |
| extract_to_directory(destination_directory) | يستخرج جميع الملفات في الأرشيف إلى الدليل المقدم. |

### انظر أيضًا

* namespace [aspose.zip.apple](/zip/python-net/aspose.zip.apple/)
* assembly [Aspose.Zip](/zip/python-net/)

