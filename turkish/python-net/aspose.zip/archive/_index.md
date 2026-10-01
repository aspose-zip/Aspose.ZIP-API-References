---
title: "Archive"
second_title: "Aspose.Zip Python için .NET API Referansı"
description: 
type: docs
weight: 10
url: /tr/python-net/aspose.zip/archive/
---

## Archive class

Bu sınıf bir zip arşiv dosyasını temsil eder. Zip arşivlerini oluşturmak, çıkarmak veya güncellemek için kullanın.

Archive türü aşağıdaki üyeleri gösterir:
## Yapıcılar
| Ad | Açıklama |
| :- | :- |
| Archive(new_entry_settings) | Girdileri için isteğe bağlı ayarlarla [Archive](/zip/python-net/aspose.zip/archive/) sınıfının yeni bir örneğini başlatır. |
| Archive(source_stream, load_options, new_entry_settings) | Arşivden çıkarılabilecek bir giriş listesi oluşturan [Archive](/zip/python-net/aspose.zip/archive/) sınıfının yeni bir örneğini başlatır. |
| Archive(path, load_options, new_entry_settings) | Arşivden çıkarılabilecek bir giriş listesi oluşturan [Archive](/zip/python-net/aspose.zip/archive/) sınıfının yeni bir örneğini başlatır. |
| Archive(main_segment, segments_in_order, load_options) | Çok bölümlü ZIP arşivinden yeni bir [Archive](/zip/python-net/aspose.zip/archive/) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Özellikler
| Ad | Açıklama |
| :- | :- |
| new_entry_settings | Yeni eklenen [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/) öğeleri için kullanılan sıkıştırma ve şifreleme ayarları. |
| comment | Tüm arşiv için yorumu alır. |
| entries | Arşivi oluşturan [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/) tipindeki girişleri alır. |
| file_entries | [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) türündeki arşivi oluşturan girişleri alır. |
| biçim | Arşiv biçimini alır. |
## Yöntemler
| Ad | Açıklama |
| :- | :- |
| create_entry(name, path, open_immediately, new_entry_settings) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, source, new_entry_settings) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, file_info, open_immediately, new_entry_settings) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, source, new_entry_settings, file_info) | Arşiv içinde tek bir giriş oluşturur. |
| create_entries(directory, include_root_directory) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| create_entries(source_directory, include_root_directory) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| delete_entry(entry) | Belirli girişin giriş listesindeki ilk oluşumunu kaldırır. |
| delete_entry(entry_index) |  |
| save(output_stream, save_options) | Arşivi sağlanan akışa kaydeder. |
| save(destination_file_name, save_options) | Arşivi sağlanan hedef dosyaya kaydeder. |
| save_split(destination_directory, options) | Çok bölümlü arşivi sağlanan hedef dizine kaydeder. |
| extract_to_directory(destination_directory) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |

### İlgili

* namespace [aspose.zip](/zip/python-net/aspose.zip/)
* assembly [Aspose.Zip](/zip/python-net/)

