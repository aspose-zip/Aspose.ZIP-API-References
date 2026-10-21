---
title: "CabArchive"
second_title: "Aspose.Zip Python için .NET API Referansı"
description: 
type: docs
weight: 10
url: /tr/python-net/aspose.zip.cab/cabarchive/
---

## CabArchive class

Bu sınıf bir CAB arşiv dosyasını temsil eder.

CabArchive türü aşağıdaki üyeleri gösterir:
## Yapıcılar
| Ad | Açıklama |
| :- | :- |
| CabArchive(settings) | Sıkıştırma için hazırlanmış [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) sınıfının yeni bir örneğini başlatır. |
| CabArchive(source_stream, load_options) | [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| CabArchive(path, load_options) | [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Özellikler
| Ad | Açıklama |
| :- | :- |
| entries | [CabEntry](/zip/python-net/aspose.zip.cab/cabentry/) türündeki arşivi oluşturan girişleri alır. |
| file_entries | [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) türündeki arşivi oluşturan girişleri alır. |
| biçim | Arşiv biçimini alır. |
## Yöntemler
| Ad | Açıklama |
| :- | :- |
| create_entry(name, path, new_entry_settings) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, source, new_entry_settings) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, file_info, new_entry_settings) | Arşiv içinde tek bir giriş oluşturur. |
| create_entries(directory, include_root_directory) | Belirtilen dizinden tüm dosyaları, özyinelemeli olarak, arşive ekler. |
| create_entries(source_directory, include_root_directory) | Belirtilen dizin yolundan tüm dosyaları özyinelemeli olarak arşive ekler. |
| save(output_stream, save_options) | Arşivi sağlanan akışa kaydeder. |
| save(destination_file_name, save_options) | Arşivi sağlanan hedef dosyaya kaydeder. |
| extract_to_directory(destination_directory) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |

### İlgili

* namespace [aspose.zip.cab](/zip/python-net/aspose.zip.cab/)
* assembly [Aspose.Zip](/zip/python-net/)

