---
title: "IsoArchive"
second_title: "Aspose.Zip Python için .NET API Referansı"
description: 
type: docs
weight: 30
url: /tr/python-net/aspose.zip.iso/isoarchive/
---

## IsoArchive class

ISO arşivini (ISO 9660) temsil eder.

IsoArchive türü aşağıdaki üyeleri sunar:
## Yapıcılar
| Ad | Açıklama |
| :- | :- |
| IsoArchive() | Yeni bir [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) sınıfı örneği başlatır ve yeni dosyalar ve dizinler eklemek için boş bir ISO arşivi oluşturur<br/>             . |
| IsoArchive(source_stream, load_options) | Yeni bir [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| IsoArchive(path, load_options) | Yeni bir [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Özellikler
| Ad | Açıklama |
| :- | :- |
| entries | [IsoEntry](/zip/python-net/aspose.zip.iso/isoentry/) türündeki arşivi oluşturan girişleri alır. |
| file_entries | [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) türündeki arşivi oluşturan girişleri alır. |
| biçim | Arşiv biçimini alır. |
## Yöntemler
| Ad | Açıklama |
| :- | :- |
| create_entry(name, file_path) | ISO görüntüsüne bir dosya ekler. |
| create_entry(name, source) | ISO görüntüsüne bir dosya ekler. |
| create_entry(name) | ISO görüntüsüne bir dosya ekler. |
| save(path, save_options) | ISO görüntüsünü belirtilen yola kaydeder. |
| save(stream, save_options) | ISO görüntüsünü belirtilen akışa kaydeder. |
| create_directory(name) | ISO görüntüsüne bir dizin ekler. |
| extract_to_directory(destination_directory) | Tüm girişleri belirtilen dizine çıkarır. |

### İlgili

* namespace [aspose.zip.iso](/zip/python-net/aspose.zip.iso/)
* assembly [Aspose.Zip](/zip/python-net/)

