---
title: "SevenZipArchive"
second_title: "Aspose.Zip Python için .NET API Referansı"
description: 
type: docs
weight: 10
url: /tr/python-net/aspose.zip.sevenzip/sevenziparchive/
---

## SevenZipArchive class

Bu sınıf 7z arşiv dosyasını temsil eder. 7z arşivlerini oluşturmak ve çıkarmak için kullanın.

SevenZipArchive türü aşağıdaki üyeleri ortaya çıkar:
## Yapıcılar
| Ad | Açıklama |
| :- | :- |
| SevenZipArchive(new_entry_settings) | [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) sınıfının, girdileri için isteğe bağlı ayarlarla yeni bir örneğini başlatır. |
| SevenZipArchive(source_stream, password) | [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| SevenZipArchive(path, password) | [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| SevenZipArchive(source_stream, options) | [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| SevenZipArchive(path, options) | [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| SevenZipArchive(parts, password) | Çok bölümlü 7z arşivinden [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Özellikler
| Ad | Açıklama |
| :- | :- |
| new_entry_settings | Yeni eklenen [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) öğeleri için kullanılan sıkıştırma ve şifreleme ayarları. |
| entries | Arşivi oluşturan [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) türündeki girişleri alır. |
| file_entries | [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) türündeki arşivi oluşturan girişleri alır. |
| biçim | Arşiv biçimini alır. |
## Yöntemler
| Ad | Açıklama |
| :- | :- |
| create_entry(name, file_info, open_immediately, new_entry_settings) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, source, new_entry_settings, file_info) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, source, new_entry_settings) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, path, open_immediately, new_entry_settings) | Arşiv içinde tek bir giriş oluşturur. |
| create_entries(directory, include_root_directory) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| create_entries(source_directory, include_root_directory) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| save(output, save_options) | 7z arşivini sağlanan akışa kaydeder. |
| save(destination_file_name, save_options) | Arşivi sağlanan hedef dosyaya kaydeder. |
| extract_to_directory(destination_directory, password) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |
| extract_to_directory(destination_directory) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |
| save_split(destination_directory, options) | Çok bölümlü arşivi sağlanan hedef dizine kaydeder. |

### İlgili

* namespace [aspose.zip.sevenzip](/zip/python-net/aspose.zip.sevenzip/)
* assembly [Aspose.Zip](/zip/python-net/)

