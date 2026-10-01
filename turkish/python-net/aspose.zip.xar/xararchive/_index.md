---
title: "XarArchive"
second_title: "Aspose.Zip Python için .NET API Referansı"
description: 
type: docs
weight: 40
url: /tr/python-net/aspose.zip.xar/xararchive/
---

## XarArchive class

Bu sınıf bir xar arşiv dosyasını temsil eder.

XarArchive türü aşağıdaki üyeleri gösterir:
## Yapıcılar
| Ad | Açıklama |
| :- | :- |
| XarArchive(default_compression_settings) | Yeni bir [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) sınıfı örneği başlatır. |
| XarArchive(source_stream, load_options) | Yeni bir [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| XarArchive(path, load_options) | Yeni bir [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Özellikler
| Ad | Açıklama |
| :- | :- |
| entries | Arşivi oluşturan [XarEntry](/zip/python-net/aspose.zip.xar/xarentry/) tipindeki girişleri alır. |
| file_entries | [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) türündeki arşivi oluşturan girişleri alır. |
| biçim | Arşiv biçimini alır. |
## Yöntemler
| Ad | Açıklama |
| :- | :- |
| create_entries(source_directory, include_root_directory, compression_settings) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| create_entries(directory, include_root_directory, compression_settings) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| create_entry(name, file_info, open_immediately, compression_settings) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, source_path, open_immediately, compression_settings) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, source, compression_settings) | Arşiv içinde tek bir giriş oluşturur. |
| save(destination_file_name, save_options) | Arşivi sağlanan hedef dosyaya kaydeder. |
| save(output, save_options) | Arşivi sağlanan akışa kaydeder. |
| extract_to_directory(destination_directory) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |
| delete_entry(entry) | Giriş listesinden belirli bir girişin ilk oluşumunu kaldırır. |

### İlgili

* namespace [aspose.zip.xar](/zip/python-net/aspose.zip.xar/)
* assembly [Aspose.Zip](/zip/python-net/)

